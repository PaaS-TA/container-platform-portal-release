FROM openjdk:8-jdk-alpine
ARG JAR_FILE=*.jar
COPY ${JAR_FILE} container-platform-admin-service-broker.jar
COPY application.yml /application.yml
ENTRYPOINT ["java","-jar","/container-platform-admin-service-broker.jar"]