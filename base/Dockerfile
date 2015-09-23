FROM ubuntu:14.04

MAINTAINER J.Gomez <jgomez@4eixos.com>

ADD chef /opt/chef/

COPY solo.rb lambom.conf /etc/riyic/

RUN apt-get -y update && apt-get -y dist-upgrade && \
apt-get install -y build-essential curl git vim lsb-release && \ 
apt-get autoclean && apt-get clean && rm -rf /var/lib/apt/lists/* && \ 
ln -sf /opt/chef/bin/lambom /bin/warmup
