FROM almalinux:8
RUN yum update -y
RUN yum install nginx -y
RUN rm -rf /usr/share/nginx/index.html
ONBUILD ADD index.html /urs/share/nginx/html/

ENTRYPOINT [ "nginx","-g", "daemon off;" ]
