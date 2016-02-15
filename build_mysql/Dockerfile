# Dockerfile for Mysql Server

FROM enakai00/centos:centos6
MAINTAINER Makoto Ootaku

ENV HOME /root
RUN yum -y clean all
RUN yum -y update
RUN yum -y install mysql-server
ADD init.sh /usr/local/bin/init.sh
RUN chmod u+x /usr/local/bin/init.sh

EXPOSE 3306
CMD ["/usr/local/bin/init.sh"]
