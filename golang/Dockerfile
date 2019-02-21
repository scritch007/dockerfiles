FROM debian:stable-slim

RUN apt-get update
RUN apt-get install -y --no-install-recommends \
    gcc libc-dev 
RUN apt-get install -y --no-install-recommends \
    wget
RUN cd /tmp && wget --no-check-certificate --continue https://dl.google.com/go/go1.11.5.linux-amd64.tar.gz
RUN tar -C /usr/local -xzf /tmp/go1.11.5.linux-amd64.tar.gz
ENV PATH=${PATH}:/usr/local/go/bin
ENV GOPATH=/go