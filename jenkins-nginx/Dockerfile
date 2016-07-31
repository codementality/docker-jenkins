FROM alpine:3.4
MAINTAINER Lisa Ridley

# Upgrade all packages
RUN apk update
RUN apk upgrade

# Install NGINX
RUN apk add --update nginx && rm -rf /var/cache/apk/*

# Add default configuration
COPY conf/jenkins.conf /etc/nginx/conf.d/jenkins.conf
COPY conf/nginx.conf /etc/nginx/nginx.conf

EXPOSE 80

CMD ["nginx"]