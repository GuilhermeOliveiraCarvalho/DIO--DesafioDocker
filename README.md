# Desafio de Projeto DIO: Criando um Container de uma Aplicação WEB

## Descrição

Este projeto foi desenvolvido como parte de um desafio da DIO (Digital Innovation One), onde o objetivo principal era criar e configurar um container Docker para uma aplicação web simples utilizando o servidor Apache (httpd).

## Passos Realizados

### 1. Configuração do Ambiente de Trabalho
- Foi criada uma pasta chamada `DesafioDocker` na Área de Trabalho para organizar os arquivos do projeto.
- Dentro desta pasta, foi criada uma subpasta chamada `html` onde foram armazenados os arquivos da aplicação web.

### 2. Criação da Aplicação Web
- Dentro da pasta `html`, foi criado um arquivo `index.html` com um conteúdo simples que descreve o propósito do desafio e os benefícios da containerização de uma aplicação web utilizando Docker.

### 3. Configuração do Docker Compose
- Foi criado um arquivo `docker-compose.yml` na raiz do projeto (`DesafioDocker`) que define a configuração necessária para rodar a aplicação web dentro de um container Docker utilizando o servidor Apache.
- No `docker-compose.yml`, foram configurados:
  - A imagem Docker do Apache (httpd).
  - O mapeamento de portas para permitir o acesso à aplicação via `localhost`.
  - O volume que mapeia a pasta `html` do host para o diretório de conteúdo do Apache dentro do container.

### 4. Execução do Docker Compose
- Utilizou-se o comando `docker-compose up` para criar e iniciar o container que serve a aplicação web.
- A aplicação foi então acessada através de `http://localhost:8080`, onde foi exibida a página web criada.

### 5. Resolução de Problemas
- Ajustaram-se as configurações de segurança no `docker-compose.yml` para resolver um problema relacionado à criação de threads pelo Apache dentro do container, garantindo que o servidor funcionasse corretamente.

### 6. Subida do Projeto para o GitHub
- Foi inicializado um repositório Git na pasta do projeto (`DesafioDocker`).
- Foram cometados os arquivos do projeto e enviados para um repositório remoto no GitHub, garantindo que todo o trabalho realizado estivesse disponível e versionado corretamente.

