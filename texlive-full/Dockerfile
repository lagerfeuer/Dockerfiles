FROM ubuntu:latest
LABEL maintainer="Lukas Deutz <publicldz@mailfence.com>"

WORKDIR /data
VOLUME /data

ARG DEBIAN_FRONTEND=noninteractive

RUN apt-get update -q
RUN apt-get install -qy texlive-full
RUN apt-get install -qy \
      make git latexmk rubber scons imagemagick \
    && apt-get clean
RUN rm -rf /var/lib/apt/lists/* 
