FROM rn.api.xiaoyuanhao.com:56109/nbugs/centos7.1_jdk8:1.0
MAINTAINER zzr

RUN mkdir /jmeter
COPY ./apache-jmeter-5.1.tgz /jmeter/

RUN cd /jmeter/ \
    && tar -zxvf apache-jmeter-5.1.tgz \
    && rm -f apache-jmeter-5.1.tgz

ENV JMETER_HOME /jmeter/apache-jmeter-5.1/
ENV PATH $JMETER_HOME/bin:$PATH
