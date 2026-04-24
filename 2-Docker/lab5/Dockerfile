FROM maven:3.9.14-eclipse-temurin-17-alpine AS base
WORKDIR /app
COPY . .
RUN mvn package

FROM openjdk:17-ea-jdk-alpine
WORKDIR /app
RUN adduser -D appuser && chown -R appuser:appuser /app
USER appuser
COPY --from=base /app/target/demo-0.0.1-SNAPSHOT.jar .
CMD [ "java","-jar","demo-0.0.1-SNAPSHOT.jar" ]
EXPOSE 8080