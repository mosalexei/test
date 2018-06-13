FROM centos/systemd

MAINTAINER "ALEX"

ADD mariadb.sql /root/mariadb.sql
ADD server.cnf  /etc/my.cnf.d/server.cnf
ADD mariadb.sh /root/mariadb.sh

#Update packages and install epel and mariadb
RUN yum -y update; yum install -y mariadb-client mariadb-server; systemctl enable mariadb
RUN yum clean all
RUN chmod +x /root/mariadb.sh

EXPOSE 3306

CMD ["/root/mariadb.sh"]


