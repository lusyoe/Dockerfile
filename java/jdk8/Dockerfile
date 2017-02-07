#
# Dockerfile by luhaoyuan: build a docker image for jdk8
# usage: docker build -t="lusyoe/jdk8" .
#
FROM debian
MAINTAINER luhaoyuan <lusyoe@163.com>

ENV JDK_VERSION 1.8.0_11

RUN mkdir -p /opt
WORKDIR /opt

# Using real url to replace
ADD http://192.168.1.2/file/language/jdk-8u11-linux-x64-without-src.tar.gz /opt/jdk-8u11-linux-x64-without-src.tar.gz
RUN tar zxf jdk-8u11-linux-x64-without-src.tar.gz && rm *.tar.gz

ENV JAVA_HOME /opt/jdk$JDK_VERSION
ENV JRE_HOME $JAVA_HOME/jre
ENV CLASSPATH $JAVA_HOME/lib/tools.jar:$JAVA_HOME/lib/dt.jar:.
ENV PATH $JAVA_HOME/bin:$PATH

ENV TZ "Asia/Shanghai"


