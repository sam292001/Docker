FROM centos:7
RUN yum -y update
RUN yum -y install httpd
RUN echo "<h1>Hello All, Hope you are enjoying learning Docker!</h1>" > /var/www/html/index.html
EXPOSE 80
CMD httpd -D FOREGROUND
