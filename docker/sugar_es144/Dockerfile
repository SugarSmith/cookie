#FROM docker.elastic.co/elasticsearch/elasticsearch:5.5.1
FROM openjdk:7-jdk-slim
MAINTAINER Jason Smith

RUN useradd -ms /bin/bash elastic
RUN apt-get update && apt-get install -y \
    python \
    wget \
    unzip\
    curl

#USER elastic
WORKDIR /elastic
COPY /files /elastic

RUN dpkg -i elasticsearch-1.4.4.deb
ENV PATH=$PATH:/usr/share/elasticsearch/bin

CMD ["elasticsearch"]

EXPOSE 9200 9300
#RUN unzip elasticsearch-1.4.4.zip
#RUN chmod +x elasticsearch-1.4.4/bin/elasticsearch
#RUN cp ./elasticsearch-1.4.4/bin/elasticsearch /etc/init.d/elasticsearch
#ENTRYPOINT ["/bin/bash", "./elasticsearch-1.4.4/bin/elasticsearch -d"]
