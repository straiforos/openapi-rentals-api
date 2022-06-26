# OpenAPI Rental Entity API
This repository is a public reference, free to use on my idea of rental REST service. It will evolve over time as I find moments to invest in it. It uses HATEOAS, and Spring boot generation to give a lift off point.

The main version of this repo lives in gitlab under my consulting firms name: Traiforce Group LLC.
https://gitlab.com/traiforce-group-development-team/openapi-rentals-api.git

I will ensure they are kept in sync. I prefer Gitlab due to their integrity and private repos they offer free of charge but put this into my personal github profile as a record.

API first development has interested me and I got to see it used live in an enterprise project. It cut down on a lot of boilerplate, specifically Enums. I prefer mixin interface composition so these classes wont be the actual way I develop but a jumping off point that enforces my API contract: Open API v3.0 within my more organized codebase.

Stay tuned for the reference implementation product release!!

The public artifact should be accessible at the gitlab project packages section:
https://gitlab.com/traiforce-group-development-team/openapi-rentals-api/-/packages/76476


# How I made this project

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