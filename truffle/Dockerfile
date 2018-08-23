FROM node:8-alpine
LABEL maintainer="pao0111@gmail.com"

RUN apk --no-cache add \
    bash git
RUN npm -g install truffle

RUN mkdir -p /home/alpine && chown 1000:1000 /home/alpine
USER 1000:1000
ENV HOME /home/alpine

WORKDIR "/app"
VOLUME ["/app"]

CMD []
ENTRYPOINT [ "/usr/local/bin/truffle" ]
