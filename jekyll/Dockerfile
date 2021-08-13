FROM ruby:3.0-slim

RUN apt update \
    && apt -y install build-essential gcc bash cmake git
RUN gem update --system \
    && gem install bundler rake jekyll

EXPOSE 4000

WORKDIR /srv/jekyll
