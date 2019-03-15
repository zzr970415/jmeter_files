FROM rn.api.xiaoyuanhao.com:56109/nbugs/centos:7.1
MAINTAINER zzr

COPY ./jdk-8u45-linux-x64.tar.gz /usr/
RUN tar -zxvf /usr/jdk-8u45-linux-x64.tar.gz 
RUN mv /usr/jdk1.8.0_45 /usr/jdk

ENV JAVA_HOME /usr/jdk
ENV PATH $JAVA_HOME/bin:$PATH
ENV CLASSPATH=$JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar
