# Dockerfile for running a Java based Minecraft server using pufferd.
FROM adoptopenjdk/openjdk11:x86_64-ubi-jre-11.0.10_9

RUN adduser -D -h /server pufferd
WORKDIR /server

RUN apk add --no-cache --virtual=.run-deps git
# Add any additional commands here

USER pufferd
ENV HOME /server
