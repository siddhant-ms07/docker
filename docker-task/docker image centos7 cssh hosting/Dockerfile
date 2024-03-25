FROM centos:7

LABEL centos_demo = "siddhant"

RUN yum install httpd -y

RUN yum install unzip -y

RUN rm -rf /var/www/html/index.html

ADD https://www.free-css.com/assets/files/free-css-templates/download/page296/neogym.zip /var/www/html/

WORKDIR /var/www/html/

RUN unzip neogym.zip
RUN mv neogym-html/* .

EXPOSE 80

CMD httpd -DFOREGROUND