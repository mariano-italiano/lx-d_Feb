FROM alpine AS helper
RUN apk add git
WORKDIR /src
ARG NGINX_CONTENT_BRANCH=develop
RUN git clone -b $NGINX_CONTENT_BRANCH https://github.com/mariano-italiano/lx-d_Feb.git


FROM nginx:1.19.2 
LABEL "Author"="Marcin K"
RUN apt-get update && apt-get install curl vim -y && apt-get clean && rm -rf /var/lib/apt/lists/*
COPY --from=helper /src/lx-d_Feb/web-content/* /usr/share/nginx/html/
