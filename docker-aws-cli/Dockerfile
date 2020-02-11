FROM docker:19.03

RUN apk -v --update add python python-dev py-pip groff build-base \
    && pip install awscli \
    && apk -v --purge del py-pip \
    && rm /var/cache/apk/*
