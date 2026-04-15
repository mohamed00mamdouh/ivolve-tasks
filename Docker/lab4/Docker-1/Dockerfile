FROM maven:3.9.14-eclipse-temurin-17-alpine
WORKDIR /app
RUN adduser -D appuser && chown -R appuser:appuser /app
USER appuser
COPY . .
RUN mvn package
CMD [ "java","-jar","target/demo-0.0.1-SNAPSHOT.jar" ]
EXPOSE 8080