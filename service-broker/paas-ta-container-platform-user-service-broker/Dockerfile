FROM openjdk:8-jdk-alpine
ARG JAR_FILE=*.jar
COPY ${JAR_FILE} container-platform-user-service-broker.jar
COPY application.yml /application.yml
ENTRYPOINT ["java","-jar","/container-platform-user-service-broker.jar"]