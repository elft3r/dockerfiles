FROM docker:19.03

RUN apk -v --update add python python-dev py-pip groff build-base \
    && pip install 'awscli>=1.17.0,<1.18.0' \
    && apk -v --purge del py-pip \
    && rm /var/cache/apk/*
