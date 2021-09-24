FROM openjdk:8-jdk-alpine
ARG JAR_FILE=*.jar
COPY ${JAR_FILE} container-platform-common-api.jar
COPY application.yml /application.yml
ENTRYPOINT ["java","-jar","-Dspring.config.location=application.yml","-Dspring.profiles.active=prod","/container-platform-common-api.jar"]

