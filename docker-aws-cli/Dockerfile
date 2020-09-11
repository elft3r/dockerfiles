FROM alpine:3.11

RUN apk -v --update add docker-cli

RUN apk -v --update add python python-dev py-pip groff build-base \
	&& pip install 'awscli>=1.18.0,<1.19.0' \
	&& apk -v --purge del py-pip \
	&& rm /var/cache/apk/*
