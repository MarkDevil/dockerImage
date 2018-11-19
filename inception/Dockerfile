FROM centos:7
MAINTAINER mamingfeng007@gmail.com

ADD inception.tar /opt
WORKDIR /opt
RUN chmod u+x /opt/inception/bin/Inception && cp /opt/inception/bin/Inception /usr/bin/Inception \
    && cp /opt/inception/bin/mysql /usr/bin/mysql
VOLUME [ "/opt" ]
EXPOSE 6669
ENTRYPOINT [ "/opt/inception/bin/Inception","--defaults-file=/opt/inception/bin/inc.cnf" ]