FROM ubuntu:14.04

RUN apt-get update
RUN apt-get install -q -y language-pack-en
RUN update-locale LANG=en_US.UTF-8

RUN apt-get install -q -y build-essential curl git pigz zlib1g-dev

RUN mkdir -p /app

RUN git clone https://github.com/mietek/halcyon /app/halcyon
RUN /app/halcyon/halcyon install --ghc-version 7.6.3
