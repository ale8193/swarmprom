FROM prom/prometheus:latest
# https://hub.docker.com/r/prom/prometheus/tags/

COPY conf /etc/prometheus/

ENTRYPOINT ["/etc/prometheus/conf/docker-entrypoint.sh"]
CMD        [ "--config.file=/etc/prometheus/conf/prometheus.yml", \
             "--storage.tsdb.path=/prometheus" ]
