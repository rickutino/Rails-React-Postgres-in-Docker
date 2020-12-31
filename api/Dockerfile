FROM ruby:2.7.1

RUN apt-get update -qq && apt-get install -y build-essential libpq-dev nodejs
RUN mkdir /ToDo

WORKDIR /ToDo

COPY Gemfile /ToDo/Gemfile
COPY Gemfile.lock /ToDo/Gemfile.lock

RUN bundle install
COPY . /ToDo
