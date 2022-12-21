# youtube project Link: https://www.youtube.com/playlist?list=PLLu1bCv5AByGUZUl4N2fhZdtHg0pd7G8E
FROM centos:latest
MAINTAINER gbiping@gmail.com
RUN yum install -y httpd zip unzip
ADD https://www.free-css.com/assets/files/free-css-templates/download/page254/photogenic.zip /var/www/html/
WORKDIR /var/www/html/
RUN unzip photogenic.zip
RUN cp -rvf photogenic/* .
RUN rm -rf photogenic photogenic.zip
CMD ["/usr/sbin/httpd", -D."FOREGROUND"]
EXPOSE 80
