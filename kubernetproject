FROM centos:latest
MAINTAINER anilmavarkar@gmail.com
RUN yum install -y httpd \
zip \
unzip
ADD https://www.free-css.com/asset/files/free-css-templates/download/page258/loxury.zip /var/www/html
WORKDIR /var/www/html
RUN unzip loxury.zip
RUN cp -rvf loxury/*
RUN rm -rvf loxury.zip
CMD ["/usr/sbin/httpd, "-D", "FOREGROUND"]
EXPOSE 80
