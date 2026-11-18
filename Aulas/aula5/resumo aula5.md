# Aula 05 - Criando APIs para o Front-end

## Objetivo da Aula

Esta aula apresentou os conceitos básicos de APIs e o processo de criação de uma API REST utilizando Express.js. O objetivo foi compreender a comunicação entre o Front-end e o Back-end e desenvolver operações CRUD para uma aplicação de notas.

---

## API e Comunicação HTTP

Uma API (Application Programming Interface) permite que sistemas troquem dados e funcionalidades. O protocolo HTTP organiza essa comunicação por meio de métodos, URLs e respostas padronizadas.

Os principais métodos HTTP apresentados foram:

- **GET**: recupera dados do servidor;
- **POST**: cria novos recursos;
- **PUT**: substitui ou atualiza um recurso existente;
- **PATCH**: atualiza parcialmente um recurso;
- **DELETE**: remove um recurso.

## Endpoints e JSON

Um endpoint é uma URL que representa um recurso ou uma operação da API. Os dados normalmente são enviados e recebidos no formato JSON (JavaScript Object Notation), que utiliza objetos e arrays para representar informações.

## Servidor Backend e Web Services

O servidor Back-end recebe requisições, processa regras de negócio, acessa dados e envia respostas aos clientes. Um Web Service permite que sistemas diferentes se comuniquem pela internet utilizando padrões como HTTP e JSON.

## Express.js

O Express.js é um framework para Node.js que facilita a criação de servidores web e APIs REST. Ele simplifica:

- a definição de rotas;
- o uso de middlewares;
- o tratamento de requisições e respostas;
- a integração com arquivos, bancos de dados e aplicações Front-end;
- a configuração de CORS para permitir acesso entre domínios.

## CRUD de Notas

A atividade prática utilizou um arquivo `data.json` para armazenar notas. A API foi criada com as seguintes operações:

- `GET /api/notes`: lista todas as notas;
- `POST /api/notes`: cria uma nova nota;
- `PUT /api/notes/:id`: atualiza uma nota existente;
- `DELETE /api/notes/:id`: remove uma nota.

Cada nova nota pode receber um identificador gerado pelo JavaScript e os campos `titulo` e `texto`.

## Deploy e Integração

A API pode ser publicada na plataforma Render, enquanto o Front-end pode ser desenvolvido em React e publicado na Vercel. Após o deploy, a aplicação Front-end substitui a URL local pelo endereço público da API.

## Documentação com Postman

O Postman permite organizar, testar e documentar requisições HTTP. Uma coleção pode conter as quatro operações CRUD, seus parâmetros, exemplos de respostas e códigos de status.

## Atividades

- Criar uma API REST com Express.js;
- Implementar operações CRUD utilizando um arquivo JSON;
- Publicar o Back-end no Render;
- Conectar uma aplicação React à API;
- Publicar o Front-end na Vercel;
- Criar uma coleção documentada no Postman.

## Conclusão

A Aula 05 mostrou como o Front-end se comunica com um servidor por meio de APIs REST. O Express permite criar endpoints de forma simples, enquanto JSON e HTTP estruturam a troca de dados. A prática integrou desenvolvimento Back-end, Front-end e publicação na nuvem.
