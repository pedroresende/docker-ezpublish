FROM debian:jessie
RUN apt-get update && apt-get install -y nginx vim nano

COPY nginx.conf /etc/nginx/nginx.conf
ADD ez_params.d /etc/nginx/ez_params.d
ADD sites-enabled /etc/nginx/sites-enabled

#RUN ln -s /etc/nginx/sites-available/default.conf /etc/nginx/sites-enabled/default
#RUN rm /etc/nginx/sites-available/default /etc/nginx/sites-enabled/default

#RUN echo "upstream php-upstream { server php:9000; }" > /etc/nginx/conf.d/upstream.conf
WORKDIR /var/www/html/ezpublish

EXPOSE 80
EXPOSE 443

CMD ["nginx"]
