FROM redis:latest

RUN mkdir -p /usr/local/etc/redis
COPY sentinel.conf /usr/local/etc/redis/sentinel.conf

EXPOSE 26379

ENTRYPOINT ["redis-server", "/usr/local/etc/redis/sentinel.conf", "--sentinel"]
