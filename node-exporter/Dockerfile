FROM prom/node-exporter:latest

ENV NODE_ID=none

USER root

COPY ./conf/docker-entrypoint.sh /etc/node-exporter/

# RUN chmod a+x /etc/node-export/docker-entrypoint.sh

ENTRYPOINT  [ "/etc/node-exporter/docker-entrypoint.sh" ]
CMD [ "/bin/node_exporter" ]
