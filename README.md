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
FROM ruby:2.3.1

RUN apt-get update -qq && apt-get -y install sudo

RUN sudo apt-get install -qq -y build-essential nodejs npm libpq-dev git fp-compiler nodejs-legacy libfontconfig1-dev cron

RUN sudo npm install -g phantomjs

ENV APP /farma_alg_reborn

CMD ["/sbin/my_init"]

WORKDIR /tmp
ADD Gemfile /tmp/
ADD Gemfile.lock /tmp
RUN sudo bundle install

RUN mkdir -p $APP

WORKDIR $APP

ENV BUNDLE_PATH /box

COPY . $APP

```

### Alteração com o Professor:

```rails
<div class="form-group">
                <%= f.label :Categoria, "Professor" %>
                <%= f.radio_button :teacher, true %>
                <%= f.label :Categoria, "Aluno" %>
                <%= f.radio_button :teacher, false, :checked => true %>
              </div>
```
