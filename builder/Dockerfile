FROM ubuntu:16.04

RUN apt update -y
RUN apt install default-jdk -y && apt install maven -y && apt install git -y && cd .. && mkdir builder
RUN cd builder && git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello && cd boxfuse-sample-java-war-hello/ && mvn package
