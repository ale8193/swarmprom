FROM prom/alertmanager:latest

COPY ./conf /etc/alertmanager/conf

CMD        [ "--config.file=/etc/alertmanager/conf/alertmanager.yml", \
             "--storage.path=/alertmanager" ]
