FROM openjdk:8-jdk-alpine
ARG JAR_FILE=paas-ta-caas-jenkins-broker.jar
COPY ${JAR_FILE} paas-ta-caas-jenkins-broker.jar
COPY application.yml /application.yml
COPY jenkins_deployment.yml /tmp/jenkins_deployment.yml
COPY jenkins_service.yml /tmp/jenkins_service.yml
COPY create-namespace.yml /tmp/create-namespace.yml
COPY docker-secret.yml /tmp/docker-secret.yml
ENTRYPOINT ["java","-jar","/paas-ta-caas-jenkins-broker.jar"]
