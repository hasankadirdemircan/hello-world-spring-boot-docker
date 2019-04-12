#pull base image
FROM openjdk:8-jdk-alpine

#maintainer 
MAINTAINER hkdemircan06@gmail.com


ARG PACKAGED_JAR=target/hello-0.0.1-SNAPSHOT.jar

ADD ${PACKAGED_JAR} app.jar

ENTRYPOINT ["java","-jar","-Xdebug","-Xrunjdwp:server=y,transport=dt_socket,address=8001,suspend=n","/app.jar"]

EXPOSE 8080:8080
EXPOSE 8001:8001
