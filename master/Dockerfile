FROM redis

RUN apt-get update \
    && apt-get install -y python python-pip --no-install-recommends \
    && pip install supervisor \
    && rm -fr /var/lib/apt/lists/*

COPY supervisord.conf /tmp/supervisord.conf
ENTRYPOINT ["supervisord"]
CMD ["-c", "/tmp/supervisord.conf"]
