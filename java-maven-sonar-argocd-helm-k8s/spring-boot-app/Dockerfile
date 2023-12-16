# You can change this base image to anything else
# But make sure to use the correct version of Java
FROM adoptopenjdk/openjdk11:alpine-jre

# Simply the artifact path, here the path is given based on the artifact path, so change it according to your maven target path.
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

# copying the jar file to app.jar
COPY ${artifact} app.jar

# This should not be changed, here you are running the jar file
ENTRYPOINT ["java","-jar","app.jar"]
