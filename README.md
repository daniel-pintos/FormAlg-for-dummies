# Form-Alg for Dummies:

> O algoritmo é constituído em 3 partes dais quais são:
  1. a similaridade entre as respostas do grupo de estudantes
  2. a respostas que para cada grupo corresponde melhor.
  3. a resposta da segunda pergunta, para encontrar uma nova similaridade

### Derivação de similaridade:

- [ ] pedir ajuda para o Alex sobre a parte de similaridade.

Vamos assumir que a similaridade das respostas é {A} onde cada


### Dockerfile:

```
FROM ruby:2.4-slim
FROM node:latest

RUN apt-get update -qq && apt-get -y install sudo
RUN node -v
RUN sudo apt-get install -qq -y build-essential nodejs npm libpq-dev git fp-compiler nodejs-legacy libfontconfig1-dev cron
RUN sudo npm install -g phantomjs@2.1.1 --unsafe-perm

ENV APP /farma_alg_reborn

RUN mkdir -p $APP

WORKDIR $APP

ENV BUNDLE_PATH /box

COPY . $APP
```
