#Begin with a base image containing the Java runtime
FROM openjdk:17-slim as build

# we have information with regards who maintains the image
MAINTAINER ls3iac.com

# We are going to add the application's jar to the container
COPY target/cards-0.0.1-SNAPSHOT.jar cards-0.0.1-SNAPSHOT.jar

# Here we execute the application
ENTRYPOINT ["java","-jar","/cards-0.0.1-SNAPSHOT.jar"]