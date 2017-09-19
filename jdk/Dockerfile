FROM registry.cn-hangzhou.aliyuncs.com/luhaoyuan/oracle-jdk8:latest
MAINTAINER Luhaoyuan <luhy1@uyunsoft.cn>

ENV TZ "Asia/Shanghai"

COPY CentOS-Base.repo /etc/yum.repos.d/

RUN yum clean all && yum makecache fast

RUN yum install sudo -y && \
    adduser kb && \
    echo "kb ALL=(root) NOPASSWD:ALL" > /etc/sudoers.d/user && \
    chmod 0440 /etc/sudoers.d/user

