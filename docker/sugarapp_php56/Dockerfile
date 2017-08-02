FROM php:5.6-apache
MAINTAINER Jason Smith

USER sugar
RUN mkdir /sugar
RUN useradd -ms /bin/bash sugar
RUN mkdir /data
WORKDIR /sugar



RUN apt-get update && apt-get install -y \
    python

EXPOSE 80

VOLUME /data

ADD ~/myfiles/ /data
