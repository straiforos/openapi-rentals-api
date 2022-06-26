Generated Spring Boot Controller, and Models Using a one time setup mvn archetype:generate:
```
mvn archetype:generate   -DgroupId="openapi.rentals.api"   -DartifactId="openapi-rentals-api"   -Dopenapi_app_contract_uri="https://app.swaggerhub.com/apis/TeamAang/Rentals_Entity_API/1.0.1#/default/get_rentals"   -DarchetypeGroupId="com.redhat.consulting"   -DarchetypeArtifactId="openapi-springboot-archetype"   -DarchetypeVersion="1.0.3"   -DinteractiveMode=false 
```
Regenerates API via:
```
mvn package
```

Install for reference implementation:
```
mvn install
```

Clean the project to regenerate controller and models based on openapi.yaml changes.
```
mvn clean
```