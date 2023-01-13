FROM ubuntu:18.04
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update && \
    apt-get install -y nano bash curl yum git make libmariadb-dev libmariadbclient-dev libmariadbclient-dev-compat gcc g++ zlib1g-dev libpcre3-dev && \
    apt-get clean
RUN mkdir emulador
WORKDIR /emulador
EXPOSE 5121 6121 6900