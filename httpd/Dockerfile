FROM centos:centos7

MAINTAINER 0.1 lax34volvic@gmail.com

RUN ["yum", "-y", "update"]

RUN ["yum", "-y", "install", "httpd"]

RUN ["yum", "-y", "install", "epel-release"]

RUN ["rpm", "-Uvh", "http://rpms.famillecollet.com/enterprise/remi-release-7.rpm"]

RUN ["yum", "-y", "install", "--enablerepo=remi,remi-php70", "php", "php-devel", "php-mbstring", "php-pdo", "php-gd", "php-mysql", "php-mcrypt"]

EXPOSE 80

ADD run-httpd.sh /run-httpd.sh
RUN chmod -v +x /run-httpd.sh

CMD ["/run-httpd.sh"]