FROM grafana/grafana:last
# https://hub.docker.com/r/grafana/grafana/tags/

COPY datasources /etc/grafana/provisioning/datasources/
COPY swarmprom_dashboards.yml /etc/grafana/provisioning/dashboards/
COPY dashboards /etc/grafana/dashboards/
COPY docker-entrypoint.sh /etc/grafana/

ENV GF_SECURITY_ADMIN_PASSWORD=admin \
    GF_SECURITY_ADMIN_USER=pass \
    GF_PATHS_PROVISIONING=/etc/grafana/provisioning/

ENTRYPOINT [ "/etc/grafana/docker-entrypoint.sh" ]
