FROM debian:jessie
RUN apt-get update && apt-get install -y openjdk-7-jre

WORKDIR /var/www/html/ezpublish/ezpublish_legacy/extension/ezfind/java

EXPOSE 8983

CMD ["solr.sh"]
