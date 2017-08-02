FROM php:5.6-apache
MAINTAINER Jason Smith



RUN apt-get update && apt-get install -y \
    python

RUN mkdir /sugar
RUN useradd -ms /bin/bash sugar
USER sugar
#RUN mkdir /data
WORKDIR /sugar



EXPOSE 80

VOLUME sugar

#COPY /file /sugar
