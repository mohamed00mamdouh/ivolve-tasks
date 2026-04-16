FROM openjdk:17-ea-jdk-alpine
WORKDIR /app
RUN adduser -D appuser && chown -R appuser:appuser /app
USER appuser
COPY target/demo-0.0.1-SNAPSHOT.jar .
CMD [ "java","-jar","demo-0.0.1-SNAPSHOT.jar" ]
EXPOSE 8080