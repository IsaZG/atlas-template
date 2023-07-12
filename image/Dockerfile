FROM ubuntu:18.04  
LABEL maintainer="crismcr@gmail.com" 
RUN  apt-get -y update && apt-get -y install nginx
COPY files/default /etc/nginx/sites-available/default
COPY files/index.html /usr/share/nginx/html/index.html
COPY files/css /usr/share/nginx/html/css
COPY files/font-awesome-4.7.0 /usr/share/nginx/html/font-awesome-4.7.0
COPY files/img /usr/share/nginx/html/img
COPY files/js /usr/share/nginx/html/js
EXPOSE 80
CMD ["/usr/sbin/nginx", "-g", "daemon off;"]