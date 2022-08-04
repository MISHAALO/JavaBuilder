FROM ubuntu:16.04

RUN apt update -y
RUN apt install default-jdk -y && apt install maven git -y && apt install git -y && cd .. && mkdir builder
RUN cd builder && git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello && cd boxfuse-sample-java-war-hello/ && mvn package 
RUN cp /builder/boxfuse-sample-java-war-hello/target/hello-1.0.war /builder 

