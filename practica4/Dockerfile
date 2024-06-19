FROM centos:7

RUN yum update -y

RUN yum install httpd -y

COPY ./web /var/www/html

EXPOSE 80

CMD ["apachectl", "-D", "FOREGROUND"]
