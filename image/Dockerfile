FROM ubuntu:18.04  
LABEL maintainer="crismcr@gmail.com" 
RUN  apt-get -y update && apt-get -y install nginx
COPY files/default /etc/image/sites-available/default
COPY files/index.html /usr/share/image/html/index.html
EXPOSE 80
CMD ["/usr/sbin/nginx", "-g", "daemon off;"]