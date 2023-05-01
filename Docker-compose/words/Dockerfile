FROM ubuntu:latest as build
RUN mkdir /docker
WORKDIR /docker
COPY pom.xml .
COPY src ./src

RUN apt-get update
RUN apt-get install maven openjdk-8-jdk --yes

RUN mvn verify
RUN apt remove maven --yes