FROM ubuntu:14.04
MAINTAINER Bryan Cosca <bcosc@curoverse.com>

USER root

RUN apt-get update -q

RUN apt-get install -qy wget build-essential zlib1g-dev

# Installing bwa-0.7.5a

WORKDIR /

RUN wget https://sourceforge.net/projects/bio-bwa/files/bwa-0.7.5a.tar.bz2 && \
    tar -xjvf bwa-0.7.5a.tar.bz2 && cd bwa-0.7.5a && make && \
    cp /bwa-0.7.5a/bwa /usr/local/bin
