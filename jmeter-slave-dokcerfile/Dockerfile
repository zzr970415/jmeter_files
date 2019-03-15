FROM rn.api.xiaoyuanhao.com:56109/nbugs/jmeter_base:latest
MAINTAINER zzr

EXPOSE 1099 50000


ENTRYPOINT $JMETER_HOME/bin/jmeter-server \
                        -Dserver.rmi.localport=50000 \
                        -Dserver_port=1099
