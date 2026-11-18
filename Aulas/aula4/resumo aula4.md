# Aula 04 - Consumindo APIs no Front-end

## Objetivo da Aula

Esta aula apresentou os fundamentos das APIs, do protocolo HTTP e da comunicação entre Front-end e Back-end. O objetivo foi compreender como aplicações web consomem dados externos e como criar uma API REST básica utilizando Express.js.

---

## API

Uma API (Application Programming Interface) é um conjunto de protocolos e ferramentas que permite que diferentes componentes de software se comuniquem.

Uma API REST segue princípios como:

- comunicação cliente-servidor sem estado;
- uso dos métodos HTTP;
- identificação de recursos por URLs;
- troca de dados em formatos como JSON.

## Protocolo HTTP

O HTTP é o protocolo usado para comunicação na Web. Nesse modelo:

- o navegador ou aplicação atua como cliente;
- o servidor recebe e processa requisições;
- cada requisição é independente;
- a resposta contém dados ou informações sobre o resultado da operação.

Os principais métodos HTTP são:

- **GET:** recupera informações;
- **POST:** cria novos recursos;
- **PUT:** substitui um recurso;
- **PATCH:** atualiza parcialmente um recurso;
- **DELETE:** remove um recurso.

## Endpoint e JSON

Um endpoint é uma URL específica que representa um recurso ou uma funcionalidade da API.

O JSON é um formato leve de troca de dados utilizado por APIs. Ele representa objetos e coleções de valores de maneira legível para pessoas e sistemas.

## Fluxo de uma Requisição

Uma requisição em uma aplicação web pode seguir este fluxo:

1. o usuário realiza uma ação no Front-end;
2. o navegador envia uma requisição HTTP;
3. o servidor Express recebe a requisição;
4. o Back-end consulta uma API externa ou processa uma regra;
5. o servidor retorna os dados em JSON;
6. o Front-end atualiza a interface com a resposta.

## Servidor Backend e Web Service

O servidor Back-end processa requisições, executa regras de negócio e fornece dados ou serviços. Um Web Service permite a comunicação entre sistemas diferentes pela internet utilizando HTTP e HTTPS.

## Express.js

O Express.js é um framework para Node.js que simplifica a criação de servidores e APIs. Ele facilita o uso de rotas e middlewares e reduz a quantidade de código necessário em comparação ao módulo HTTP do Node.js.

Um fluxo básico para criar uma API com Express inclui:

- criar uma pasta do projeto;
- executar `npm install express`;
- instalar o CORS;
- criar o arquivo da API;
- definir rotas;
- iniciar o servidor com `node api.js`.

O CORS é um mecanismo de segurança que controla o acesso entre origens diferentes no navegador.

## Publicação no Render

A plataforma Render permite publicar o Back-end na nuvem. Um Web Service pode ser conectado a um repositório do GitHub, receber os comandos de build e start e gerar uma URL pública para consumo da API.

## Atividades

- Pesquisar dez projetos no GitHub que utilizem APIs;
- Identificar o framework utilizado e a API consumida;
- Criar um arquivo Markdown com uma tabela dos projetos encontrados;
- Criar uma API com Express que retorne data e hora;
- Publicar a API no Render;
- Desenvolver uma aplicação Front-end que consuma a API;
- Publicar o Front-end e documentar o processo.

## Conclusão

A Aula 04 mostrou como o Front-end utiliza HTTP e JSON para comunicar-se com APIs e servidores. APIs externas também podem fornecer dados para aplicações desenvolvidas em React, Vue, Next.js e outros frameworks, desde que a comunicação seja organizada por endpoints e métodos adequados.
