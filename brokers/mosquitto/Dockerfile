FROM eclipse-mosquitto
COPY docker-entrypoint.sh /
COPY config /mqtt/config

VOLUME ["/mqtt/config", "/mqtt/data", "/mqtt/log"]
ENTRYPOINT ["/docker-entrypoint.sh"]

EXPOSE 1883 9001

CMD ["/usr/sbin/mosquitto", "-c", "/mosquitto/config/mosquitto.conf"]