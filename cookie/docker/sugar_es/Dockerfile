#FROM docker.elastic.co/elasticsearch/elasticsearch:5.5.1
FROM itzg/elasticsearch:1.4
MAINTAINER Jason Smith

USER sugar
RUN useradd -ms /bin/bash sugar
WORKDIR /sugar


RUN apt-get update && apt-get install -y \
    python

VOLUME
