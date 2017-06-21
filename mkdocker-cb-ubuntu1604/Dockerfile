#Dockerfile
FROM ubuntu:16.04
MAINTAINER weixin store6
#更新apt-get源 使用aliyun的源
RUN     mv /etc/apt/sources.list /etc/apt/sources.list.bak 
RUN     echo "deb http://mirrors.aliyun.com/ubuntu/ trusty main multiverse restricted universe " >/etc/apt/sources.list
RUN     echo "deb http://mirrors.aliyun.com/ubuntu/ trusty-backports main multiverse restricted universe " >>/etc/apt/sources.list
RUN     echo "deb http://mirrors.aliyun.com/ubuntu/ trusty-proposed main multiverse restricted universe " >>/etc/apt/sources.list
RUN     echo "deb http://mirrors.aliyun.com/ubuntu/ trusty-security main multiverse restricted universe " >>/etc/apt/sources.list
RUN     echo "deb http://mirrors.aliyun.com/ubuntu/ trusty-updates main multiverse restricted universe " >>/etc/apt/sources.list
RUN     echo "deb-src http://mirrors.aliyun.com/ubuntu/ trusty main multiverse restricted universe " >>/etc/apt/sources.list
RUN     echo "deb-src http://mirrors.aliyun.com/ubuntu/ trusty-backports main multiverse restricted universe " >>/etc/apt/sources.list
RUN     echo "deb-src http://mirrors.aliyun.com/ubuntu/ trusty-proposed main multiverse restricted universe " >>/etc/apt/sources.list
RUN     echo "deb-src http://mirrors.aliyun.com/ubuntu/ trusty-security main multiverse restricted universe " >>/etc/apt/sources.list
RUN     echo "deb-src http://mirrors.aliyun.com/ubuntu/ trusty-updates main multiverse restricted universe " >>/etc/apt/sources.list

RUN apt-get update && apt-get install net-tools -y
RUN apt-get update && apt-get install vim rsync  wget  curl lrzsz openssh-client openssh-server -y
RUN echo "Asia/Shanghai" >  /etc/timezone
RUN  cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime