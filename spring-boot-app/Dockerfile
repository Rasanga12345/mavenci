# Java 17 runtime (matches Maven + Spring Boot 3)
FROM eclipse-temurin:17-jre-alpine

# Default JAR pattern (can be overridden at build time)
ARG ARTIFACT=target/*.jar

WORKDIR /opt/app

# Copy the built JAR into the container
COPY ${ARTIFACT} app.jar

# Run the application
ENTRYPOINT ["java","-jar","app.jar"]
