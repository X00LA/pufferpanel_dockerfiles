# Dockerfile for running a Java based Minecraft server using pufferd.
FROM adoptopenjdk/openjdk11:ubi

RUN mkdir /opt/app
COPY japp.jar /opt/app
CMD ["java", "-jar", "/opt/app/japp.jar"]

RUN adduser -D -h /server pufferd
WORKDIR /server

RUN apk add --no-cache --virtual=.run-deps git
# Add any additional commands here

USER pufferd
ENV HOME /server
