FROM centos/systemd

MAINTAINER "ALEX"

#Update packages and install epel and nginx
RUN yum -y update; yum install -y epel-release; yum install -y nginx; systemctl enable nginx

EXPOSE 80

CMD ["nginx", "-g daemon off;"]


