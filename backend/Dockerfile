FROM openjdk:22-slim

LABEL maintainer="chaimabt"
LABEL version="1.0"
LABEL description="Application Spring Boot"

WORKDIR /app

COPY target/ .

EXPOSE 8080



CMD ["java", "-jar", "spring-boot-data-jpa-0.0.1-SNAPSHOT.jar", "--spring.config.location=classes/application.properties"]

