FROM php:7.1-apache
MAINTAINER Jason Smith

USER sugar
RUN useradd -ms /bin/bash sugar
WORKDIR /sugar


RUN apt-get update && apt-get install -y \
    python

VOLUME
