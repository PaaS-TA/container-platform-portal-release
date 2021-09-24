FROM openjdk:8-jdk-alpine
ARG JAR_FILE=*.war
COPY ${JAR_FILE} container-platform-webuser.war
COPY application.yml /application.yml
ENTRYPOINT ["java","-jar","-Dspring.config.location=application.yml","-Dspring.profiles.active=prod","/container-platform-webuser.war"]

