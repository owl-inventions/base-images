FROM python:alpine

# install git
RUN apk update \
    && apk upgrade \
    && apk add --no-cache git \
    && rm -rf /var/lib/apt/lists/* \
      /var/cache/apk/* \
      /usr/share/man \
      /tmp/*

RUN pip install awscli