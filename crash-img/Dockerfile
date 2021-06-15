FROM alpine:3

LABEL org.opencontainers.image.source https://github.com/phartenfeller/docker-fail-images

RUN mkdir /app

COPY run.sh /app

CMD ["ash", "/app/run.sh"]
