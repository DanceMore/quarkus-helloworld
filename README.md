# quarkus-helloworld

bootstrapping....

```
# launch a Java+Maven environment...
docker run --rm -it -v $(pwd):/app maven:3.9.5-amazoncorretto-21 /bin/bash

# install Quarkus
mvn io.quarkus.platform:quarkus-maven-plugin:3.5.1:create \
    -DprojectGroupId=io.github.dancemore\
    -DprojectArtifactId=quarkus-helloworld \
    -Dextensions="resteasy-reactive, resteasy-reactive-jackson, smallrye-openapi"

./mvnw quarkus:add-extension -Dextensions='jdbc-postgresql, hibernate-orm-panache'
```
