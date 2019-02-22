FROM prom/alertmanager:latest

COPY conf /etc/alertmanager/

CMD        [ "--config.file=/etc/alertmanager/alertmanager.yml", \
             "--storage.path=/alertmanager" ]
