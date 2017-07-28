FROM mysql:5.7
MAINTAINER Jason Smith

USER sugar
RUN useradd -ms /bin/bash sugar
#WORKDIR /sugar

# MySQL
RUN mysql_install_db --user=mysql --ldata=/var/lib/mysql
COPY mysql /var/lib/mysql

VOLUME ["/var/lib/mysql"]

RUN apt-get update && apt-get install -y \
    python
