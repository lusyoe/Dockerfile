#FROM registry.cn-hangzhou.aliyuncs.com/luhaoyuan/oracle-jdk8:latest
FROM uyun/kb-jdk8:latest
MAINTAINER Luhaoyuan <luhy1@uyunsoft.cn>

COPY target/web-V2.0.R1-SNAPSHOT-bin.zip /opt/kb/

WORKDIR /opt/kb

RUN unzip web-V2.0.R1-SNAPSHOT-bin.zip

RUN ["chmod", "+x", "bin/kb-web.sh"]

RUN chown -R kb:kb /opt/kb

USER kb

CMD ["/opt/kb/bin/kb-web.sh", "start"]
