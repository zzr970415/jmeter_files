FROM rn.api.xiaoyuanhao.com:56109/nbugs/jmeter_base:latest
MAINTAINER zzr

RUN sed -r -i '/\<client.rmi.localport\>/s/0/60000/g' /jmeter/apache-jmeter-5.1/bin/jmeter.properties \
    && sed -r -i '/\<client.rmi.localport\>/s/#//g' /jmeter/apache-jmeter-5.1/bin/jmeter.properties
RUN sed -i -r '/\<remote_hosts=128\>/s/127.0.0.1/172.21.0.11:1099,172.21.0.12:1099/g' /jmeter/apache-jmeter-5.1/bin/jmeter.properties

EXPOSE 60000
