FROM centos/systemd

MAINTAINER "ALEX"

#Update packages and install epel and mariadb
RUN yum -y update; yum install -y php php-fpm php-mysql php-cli php-mcrypt php-json; systemctl enable php-fpm
RUN yum clean all

EXPOSE 9000

CMD ["/usr/sbin/php-fpm"]


