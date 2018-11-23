FROM grafana/grafana:5.3.2

WORKDIR /etc/grafana
COPY datasources ./datasources

WORKDIR /app
COPY entrypoint.sh ./
USER root
RUN chmod a+x entrypoint.sh

USER grafana
ENTRYPOINT ["/app/entrypoint.sh"]
