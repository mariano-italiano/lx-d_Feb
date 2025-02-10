FROM nginx:1.19.2 

COPY index.html /usr/share/nginx/html/index.html 
COPY default.conf /etc/nginx/conf.d/default.conf
COPY .htpasswd /etc/nginx/conf.d/.htpasswd

RUN apt-get update && apt-get install vim curl -y 
