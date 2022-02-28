# Spring Boot JPA application accessing an SQL database

## Introduction

This is a Spring Boot application that accesses an SQL database.  The data model is a `User` that has an id, name and email address.  There is one controller with two endpoints:

* `/demo/all` - lists all users  (GET REQUEST)
* `/demo/add` - add a user (POST REQUEST)

> This sample is based on the Spring [Accessing data with MySQL](https://spring.io/guides/gs/accessing-data-mysql/) guide, although we changed it to use a PostgreSQL database.

## Building and running locally

### Using HSQLDB

We can build and run this app locally using an embedded HSQL database.

To build the app as an uberjar run:

```
./mvnw clean package 
```

To start the application locally with an embedded database run:

```
./mvnw spring-boot:run
```

See [Accessing the app](#accessing-the-app) for commands to test the app.

### Using PostgreSQL with Docker

We can build and run this app locally using a PostgreSQL database running in a Docker container.

To start the PostgreSQL container run:

```
docker run --rm -it --name postgres -p 5432:5432 \
  -e POSTGRES_USER=tanzu -e POSTGRES_PASSWORD=s3cret -e POSTGRES_DB=test \
  -d postgres
```

To build the app as an uberjar run:

```
./mvnw clean package
```

To start the application locally with using the Docker PostgreSQL database run:

```
./mvnw spring-boot:run -Dspring-boot.run.profiles=postgresql
```

You can also use the built uberjar using:

```
java -jar target/java-spring-boot-0.0.1-SNAPSHOT.jar \
  --spring.profiles.active=postgresql
```

See [Accessing the app](#accessing-the-app) for commands to test the app.

### Accessing the app

To view the users run:

```
curl -w'\n' localhost:8080/demo/all
```

To add a user run:

```
curl -w'\n' localhost:8080/demo/add \
 -d name=First \
 -d email=someemail@someemailprovider.com
```

Test## Building and deploying to a Kubernetes cluster using a TAP workload

### Install VMware Tanzu SQL with Postgres for Kubernetes

Starting with version 1.5.0 _VMware Tanzu SQL with Postgres for Kubernetes_ supports _Tanzu Application Platform_ (TAP) with Service Binding. For more information on Service Binding, see [Service Binding Specification for Kubernetes](https://github.com/servicebinding/spec) in the Kubernetes documentation.

Install the _Tanzu Postgres Operator_ following directions in the [VMware Tanzu SQL with Postgres for Kubernetes documentation](https://docs.vmware.com/en/VMware-Tanzu-SQL-with-Postgres-for-Kubernetes/1.5/tanzu-postgres-k8s/GUID-install-operator.html).

### Create a Postgres Instance

> Note: Review the storage class requirements in the [Prerequisites](https://docs.vmware.com/en/VMware-Tanzu-SQL-with-Postgres-for-Kubernetes/1.5/tanzu-postgres-k8s/GUID-create-delete-postgres.html#prerequisites) section. 

Apply the `database/postgres-instance.yaml` manifest using `kubectl`:

```
kubectl apply -f database/postgres-instance.yaml
```

### Create RBAC role for service-binding support

The service-binding support needs to be able to access the Postgres instances so we create an RBAC Role and RoleBinding using `kubectl` to apply the `database\postgres-service-binding-rbac.yaml` file:

```
kubectl apply -f database/postgres-service-binding-rbac.yaml
```

### Deploying to Kubernetes as a TAP workload with Tanzu CLI

If you make modifications to the source and push to your own Git repository, then you can update the `spec.source.git` information in the `config/workload.yaml` file.

When you are done developing your database app, you can simply deploy it using:

```
tanzu apps workload apply -f config/workload.yaml
```

If you would like deploy the code from your local working directory you can use the following command:

```
tanzu apps workload create java-spring-boot -f config/workload.yaml \
  --local-path . \
  --source-image <REPOSITORY-PREFIX>/java-spring-boot-source \
  --type web
```

### Accessing the app deployed to your cluster

If you don't have `curl` installed it can be installed using downloads here: https://curl.se/download.html

> Note: This depends on the TAP installation having DNS configured for the Knative ingress.

Determine the URL to use for accessing the app by running:

```
tanzu apps workload get java-spring-boot
```

To view the users run:

```
curl -w'\n' <URL>/demo/all
```

To add a user run:

```
curl -w'\n' <URL>/demo/add \
 -d name=First \
 -d email=someemail@someemailprovider.com
```
