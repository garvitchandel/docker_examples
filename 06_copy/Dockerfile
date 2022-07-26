# example 6 - Copy

FROM ubuntu:latest

# webserver nginx

RUN apt-get -y update && apt-get -y install nginx

# PATH when using nginx image from docker hub /usr/share/nginx/html
# COPY --chown <user1>:<group1> SRC DEST

COPY index.html /var/www/html/index.nginx-debian.html

# EXPOSE THE PORT -HTTP (80)
EXPOSE 80/tcp

# EXPOSE THE PORT - HTTPS (443)
EXPOSE 443/tcp

# EXPOSE ON UDP
# EXPOSE 123/udp

# start the nginx server
CMD ["nginx", "-g", "daemon off;"]


