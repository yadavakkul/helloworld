FROM centos 
MAINTAINER akkul 
RUN yum clean all && yum install -y
RUN yum install httpd -y
EXPOSE 80 
WORKDIR /root 
VOLUME /data 
