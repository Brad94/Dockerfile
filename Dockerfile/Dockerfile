
FROM ubuntu:latest

RUN apt-get update -y
RUN apt-get install -y wget
RUN apt-get install -y tar
RUN apt-get install -y git-all

WORKDIR /opt

RUN wget --no-check-certificate --no-cookies --header "Cookie: oraclelicense=accept-securebackup-cookie" http://download.oracle.com/otn-pub/java/jdk/8u131-b11/d54c1d3a095b4ff2b6607d096fa80163/jdk-8u131-linux-x64.tar.gz
RUN tar zxvf jdk-8u131-linux-x64.tar.gz
RUN update-alternatives --install /usr/bin/java java /opt/jdk1.8.0_131/bin/java 100
RUN update-alternatives --install /usr/bin/javac javac /opt/jdk1.8.0_131/bin/javac 100
