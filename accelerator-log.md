# Accelerator Log

## Options
```json
{
  "deploymentType" : "workload",
  "postgresInstanceName" : "postgres-sample",
  "projectName" : "java-spring-boot",
  "storageClassName" : "standard"
}
```
## Log
```
┏ engine (Chain)
┃  Info Running Chain(Combo, UniquePath)
┃ ┏ engine.transformations[0] (Combo)
┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseLast))
┃ ┃ engine.transformations[0].merge (Chain)
┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┏ engine.transformations[0].merge.transformations[0] (Merge)
┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo, Combo, Combo, Combo)
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Exclude)
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[0].<combo> (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/MavenWrapperDownloader.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug database/postgres-instance.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug database/postgres-service-binding-rbac.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug logo-edds-red.753d123a.svg matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/MainController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/User.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/UserRepository.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/UsersApplication.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-postgresql.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/users/UsersApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0].<combo>.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃  Info Will exclude [pom.xml, database/**, config/**, catalog/**, README.md, DEPLOYING.md]
┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml, database/**, config/**, catalog/**, README.md, DEPLOYING.md] -> included
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/MavenWrapperDownloader.java didn't match [pom.xml, database/**, config/**, catalog/**, README.md, DEPLOYING.md] -> included
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [pom.xml, database/**, config/**, catalog/**, README.md, DEPLOYING.md] -> included
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml, database/**, config/**, catalog/**, README.md, DEPLOYING.md] -> included
┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md matched [pom.xml, database/**, config/**, catalog/**, README.md, DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml, database/**, config/**, catalog/**, README.md, DEPLOYING.md] -> included
┃ ┃ ┃ ┃ ┃ Debug README.md matched [pom.xml, database/**, config/**, catalog/**, README.md, DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [pom.xml, database/**, config/**, catalog/**, README.md, DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [pom.xml, database/**, config/**, catalog/**, README.md, DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ Debug database/postgres-instance.yaml matched [pom.xml, database/**, config/**, catalog/**, README.md, DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ Debug database/postgres-service-binding-rbac.yaml matched [pom.xml, database/**, config/**, catalog/**, README.md, DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ Debug logo-edds-red.753d123a.svg didn't match [pom.xml, database/**, config/**, catalog/**, README.md, DEPLOYING.md] -> included
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml, database/**, config/**, catalog/**, README.md, DEPLOYING.md] -> included
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml, database/**, config/**, catalog/**, README.md, DEPLOYING.md] -> included
┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml, database/**, config/**, catalog/**, README.md, DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/MainController.java didn't match [pom.xml, database/**, config/**, catalog/**, README.md, DEPLOYING.md] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/User.java didn't match [pom.xml, database/**, config/**, catalog/**, README.md, DEPLOYING.md] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/UserRepository.java didn't match [pom.xml, database/**, config/**, catalog/**, README.md, DEPLOYING.md] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/UsersApplication.java didn't match [pom.xml, database/**, config/**, catalog/**, README.md, DEPLOYING.md] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-postgresql.properties didn't match [pom.xml, database/**, config/**, catalog/**, README.md, DEPLOYING.md] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml, database/**, config/**, catalog/**, README.md, DEPLOYING.md] -> included
┃ ┃ ┃ ┗ ┗ Debug src/test/java/com/example/users/UsersApplicationTests.java didn't match [pom.xml, database/**, config/**, catalog/**, README.md, DEPLOYING.md] -> included
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[1].<combo> (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [pom.xml]
┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/MavenWrapperDownloader.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug database/postgres-instance.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug database/postgres-service-binding-rbac.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug logo-edds-red.753d123a.svg didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/MainController.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/User.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/UserRepository.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/UsersApplication.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-postgresql.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/users/UsersApplicationTests.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [spring-sql-jpa->java-spring-boot]
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'workload') evaluated to true
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[2].<combo> (Chain)
┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'workload') evaluated to true
┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[2].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [database/**]
┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [database/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/MavenWrapperDownloader.java didn't match [database/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [database/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [database/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md didn't match [database/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [database/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [database/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [database/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [database/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug database/postgres-instance.yaml matched [database/**] -> included
┃ ┃ ┃ ┃ ┃ Debug database/postgres-service-binding-rbac.yaml matched [database/**] -> included
┃ ┃ ┃ ┃ ┃ Debug logo-edds-red.753d123a.svg didn't match [database/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [database/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [database/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [database/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/MainController.java didn't match [database/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/User.java didn't match [database/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/UserRepository.java didn't match [database/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/UsersApplication.java didn't match [database/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-postgresql.properties didn't match [database/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [database/**] -> excluded
┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/users/UsersApplicationTests.java didn't match [database/**] -> excluded
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[2].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[2].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [postgres-sample->postgres-sample]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[2].<combo>.transformations[1].transformations[1] (ReplaceText)
┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [standard->standard]
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[3] (Combo)
┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'workload') evaluated to true
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[3].<combo> (Chain)
┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'workload') evaluated to true
┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[3].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [catalog/**]
┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [catalog/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/MavenWrapperDownloader.java didn't match [catalog/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [catalog/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [catalog/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md didn't match [catalog/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [catalog/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [catalog/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [catalog/**] -> included
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [catalog/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug database/postgres-instance.yaml didn't match [catalog/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug database/postgres-service-binding-rbac.yaml didn't match [catalog/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug logo-edds-red.753d123a.svg didn't match [catalog/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [catalog/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [catalog/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [catalog/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/MainController.java didn't match [catalog/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/User.java didn't match [catalog/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/UserRepository.java didn't match [catalog/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/UsersApplication.java didn't match [catalog/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-postgresql.properties didn't match [catalog/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [catalog/**] -> excluded
┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/users/UsersApplicationTests.java didn't match [catalog/**] -> excluded
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[3].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[3].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [spring-sql-jpa->java-spring-boot]
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[4] (Combo)
┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'workload') evaluated to true
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[4].<combo> (Chain)
┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'workload') evaluated to true
┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[4].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [config/**]
┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [config/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/MavenWrapperDownloader.java didn't match [config/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [config/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [config/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md didn't match [config/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [config/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [config/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [config/**] -> included
┃ ┃ ┃ ┃ ┃ Debug database/postgres-instance.yaml didn't match [config/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug database/postgres-service-binding-rbac.yaml didn't match [config/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug logo-edds-red.753d123a.svg didn't match [config/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [config/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [config/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [config/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/MainController.java didn't match [config/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/User.java didn't match [config/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/UserRepository.java didn't match [config/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/UsersApplication.java didn't match [config/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-postgresql.properties didn't match [config/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [config/**] -> excluded
┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/users/UsersApplicationTests.java didn't match [config/**] -> excluded
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[4].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[4].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [: spring-sql-jpa->: java-spring-boot]
┃ ┃ ┃ ┏ README (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(Append))
┃ ┃ ┃ ┃ README.merge (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┏ README.merge.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ ┃ ┃ README.merge.transformations[0].sources[0].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[0].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [README.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/MavenWrapperDownloader.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug database/postgres-instance.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug database/postgres-service-binding-rbac.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug logo-edds-red.753d123a.svg didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/MainController.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/User.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/UserRepository.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/UsersApplication.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-postgresql.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/users/UsersApplicationTests.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[0].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[0].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [spring-sql-jpa->java-spring-boot]
┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'workload') evaluated to true
┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ ┃ ┃ README.merge.transformations[0].sources[1].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'workload') evaluated to true
┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[1].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [DEPLOYING.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/MavenWrapperDownloader.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md matched [DEPLOYING.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug database/postgres-instance.yaml didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug database/postgres-service-binding-rbac.yaml didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug logo-edds-red.753d123a.svg didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/MainController.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/User.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/UserRepository.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/users/UsersApplication.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-postgresql.properties didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/users/UsersApplicationTests.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[1].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText, RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[1].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [spring-sql-jpa->java-spring-boot]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[1].<combo>.transformations[1].transformations[1] (RewritePath)
┃ ┃ ┃ ┃ ┗ ┗ ┗ ┗ Debug Path 'DEPLOYING.md' matched '^(?<folder>.*/)?(?<filename>([^/]+?|)(?=(?<ext>\.[^/.]*)?)$)' with groups {ext=.md, folder=null, filename=DEPLOYING.md, g0=DEPLOYING.md, g1=null, g2=DEPLOYING.md, g3=DEPLOYING.md, g4=.md} and was rewritten to 'README.md'
┃ ┃ ┃ ┃ ┏ README.merge.transformations[1] (UniquePath)
┃ ┃ ┗ ┗ ┗ Debug Multiple representations for path 'README.md', will concatenate them together
┃ ┗ ╺ engine.transformations[0].merge.transformations[1] (UniquePath)
┗ ╺ engine.transformations[1] (UniquePath)
```
