FROM eva/php

# RUN apt-get install -y gcc autoconf bison flex libtool make libboost-all-dev libcurl4-openssl-dev curl libevent-dev memcached uuid-dev libsqlite3-dev libmysqlclient-dev
# COPY gearmand.tgz /home/gearmand.tgz
# RUN cd /home && tar -xvf gearmand.tgz && cd gearmand-1.1.12 && ./configure && make && make install



RUN apt-get update && apt-get install -y gearman-job-server && rm -r /var/lib/apt/lists/*
WORKDIR /opt

# RUN         RUN usermod -u 1000 gearman

CMD "gearmand"
