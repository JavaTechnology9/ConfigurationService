FROM openjdk:8-jdk-alpine
RUN  apk update && apk upgrade && apk add netcat-openbsd && apk add curl
ADD target/ConfigurationService-0.0.1-SNAPSHOT.jar config.jar
ENTRYPOINT ["java","-jar","config.jar"]
EXPOSE 8888
