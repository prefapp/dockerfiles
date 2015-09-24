FROM 4eixos/base

MAINTAINER J.Gomez <jgomez@4eixos.com>

COPY node.json /root/node.json

RUN /bin/warmup

# clean config files that can cause problems in next run
RUN rm -f /etc/nginx/sites-available/* /etc/nginx/sites-enables/*
