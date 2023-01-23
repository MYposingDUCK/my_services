FROM alpine
LABEL dev="myposingduck"
RUN apk add nginx \
    && mkdir -p /var/www/html/
#ADD ./src/nginx.conf /etc/nginx/
USER nginx
WORKDIR /etc/nginx
ENTRYPOINT ["/usr/sbin/nginx", "-g", "daemon off;"]