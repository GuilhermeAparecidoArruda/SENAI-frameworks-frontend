# Atividade 01 — Projetos do GitHub que utilizam APIs

## Objetivo

Pesquisar projetos disponíveis no GitHub que utilizam APIs em suas aplicações, identificar o framework utilizado e as APIs consumidas. Os projetos abaixo foram selecionados a partir de seus repositórios e arquivos README públicos.

## Tabela dos projetos analisados

| Nº | Projeto | Framework / tecnologias | API consumida | Como a API é utilizada |
|---:|---|---|---|---|
| 1 | [React Weather App](https://github.com/arasgungore/react-weather-app) | React, Axios, Styled-components | OpenWeatherMap API | Busca informações climáticas de uma cidade e apresenta temperatura, condições do tempo e previsões na interface. |
| 2 | [GitHub Issues Viewer](https://github.com/dceddia/github-issues-viewer) | React, Redux, Create React App | GitHub API | Consulta issues de repositórios, permitindo visualizar informações, comentários e detalhes das issues. |
| 3 | [PokeAPI React](https://github.com/Onnichan/pokeapi-react) | React, JavaScript, CSS | PokéAPI | Consulta dados dos Pokémon por nome e apresenta os resultados em uma Pokédex com cards e detalhes. |
| 4 | [TMDB Posters API](https://github.com/escummy/tmdb-posters-api) | React, Redux Toolkit, Axios, Bootstrap, Material UI | TMDb API | Busca filmes e informações relacionadas, mantendo também dados de favoritos e lista para assistir. |
| 5 | [React-Spotify](https://github.com/Pau1fitz/react-spotify) | React, Redux | Spotify API | Obtém informações de músicas e artistas e utiliza os dados para construir uma interface semelhante a um cliente de música. |
| 6 | [NASA API Front](https://github.com/papplo/nasa-api-front) | React, Create React App, Jest, Enzyme | NASA APOD e Mars Rover Photos | Busca imagens astronômicas e fotografias de Marte para exibição em diferentes telas da aplicação. |
| 7 | [Dashboard](https://github.com/zce/dashboard) | Vue.js 3, Vite, Vue Router | API própria/fake API | O dashboard consulta um servidor de API para obter os dados que serão apresentados nos componentes da aplicação. |
| 8 | [Pokedex](https://github.com/tranmani/pokedex) | Vue.js, Quasar Framework, Vuex | PokéAPI e pokeapi-sprites | Consulta informações dos Pokémon e utiliza os dados e imagens retornados para montar uma Pokédex. |
| 9 | [TMDB 2.0](https://github.com/AhmedSemih/TMDB-2.0) | Next.js, TypeScript, Tailwind CSS | TMDb API v3 | Consulta filmes e séries, permitindo pesquisar e exibir informações de entretenimento em uma interface responsiva. |
| 10 | [Book Explorer](https://github.com/martian56/book-explorer) | React, Vite, Tailwind CSS, React Router | Open Library API | Pesquisa livros por título, autor ou palavra-chave e consulta detalhes, autores, assuntos e capas. |

## Análise dos projetos

### 1. React Weather App

O projeto utiliza React para construir a interface e Axios para realizar as requisições HTTP. A OpenWeatherMap API fornece os dados meteorológicos. A aplicação possui uma separação entre componentes visuais e um serviço responsável pela comunicação com a API.

**Principal aprendizado:** mostra de forma simples como uma aplicação React pode buscar dados externos e transformar a resposta da API em informações visíveis para o usuário.

### 2. GitHub Issues Viewer

O projeto utiliza React e Redux para consultar a GitHub API. A aplicação consegue trabalhar com diferentes organizações e repositórios e apresentar suas issues. Também utiliza componentes para renderizar informações em Markdown.

**Principal aprendizado:** demonstra como uma API pode ser integrada a uma aplicação para consultar dados que mudam conforme o repositório selecionado.

### 3. PokeAPI React

É uma Pokédex desenvolvida com React. O usuário pode pesquisar um Pokémon e visualizar seus dados. A PokéAPI funciona como fonte externa das informações.

**Principal aprendizado:** é um exemplo interessante de consumo de API REST, principalmente para trabalhar com requisições, estados de carregamento e apresentação de dados em componentes.

### 4. TMDB Posters API

O projeto utiliza a API do The Movie Database para buscar informações sobre filmes. React é utilizado para a interface, enquanto Redux Toolkit ajuda no gerenciamento do estado e Axios realiza as requisições.

**Principal aprendizado:** mostra uma aplicação com maior quantidade de dados externos e a necessidade de organizar o estado da aplicação.

### 5. React-Spotify

Esse projeto cria um cliente de música utilizando React e Redux conectado à Spotify API. A API fornece informações relacionadas a músicas e outros conteúdos do Spotify.

**Principal aprendizado:** demonstra como APIs podem ser utilizadas para criar aplicações que trabalham com grandes conjuntos de informações e diferentes recursos relacionados entre si.

### 6. NASA API Front

A aplicação utiliza APIs públicas da NASA, incluindo a Astronomy Picture of the Day (APOD) e a API de fotos dos veículos exploradores de Marte. O projeto apresenta diferentes formas de visualização desses conteúdos.

**Principal aprendizado:** mostra que uma mesma aplicação pode consumir mais de um endpoint/API para criar diferentes funcionalidades.

### 7. Dashboard

O dashboard é desenvolvido com Vue.js 3 e utiliza uma API própria/fake API para fornecer os dados da aplicação. O repositório também disponibiliza um servidor separado para simular o backend.

**Principal aprendizado:** ajuda a compreender a separação entre frontend e backend, mesmo quando o servidor é utilizado apenas para fins de demonstração.

### 8. Pokedex com Vue e Quasar

O projeto utiliza Vue.js com Quasar Framework e Vuex. A PokéAPI fornece os dados dos Pokémon e o projeto também utiliza fontes de sprites para apresentar as imagens.

**Principal aprendizado:** demonstra que frameworks de interface podem ser combinados com bibliotecas de componentes e APIs externas para criar aplicações mais completas.

### 9. TMDB 2.0

É uma aplicação desenvolvida com Next.js e TypeScript, utilizando Tailwind CSS para a interface. A TMDb API v3 é responsável pelos dados de filmes e séries.

**Principal aprendizado:** mostra o consumo de APIs dentro de um projeto Next.js e como variáveis de ambiente podem ser utilizadas para configurar a chave da API.

### 10. Book Explorer

O projeto utiliza React, Vite, Tailwind CSS e React Router. A Open Library API é utilizada para pesquisar livros e obter informações detalhadas, enquanto a API de capas fornece as imagens dos livros.

**Principal aprendizado:** demonstra o uso de múltiplos endpoints relacionados a uma mesma aplicação e a criação de páginas de detalhes a partir dos dados retornados.

## Conclusão

A análise dos dez projetos mostra que o consumo de APIs é uma prática muito comum no desenvolvimento de aplicações modernas. As APIs permitem que o frontend obtenha informações de serviços externos sem precisar armazenar todos os dados diretamente na aplicação.

Também foi possível observar que diferentes frameworks podem trabalhar com APIs de maneira semelhante. React, Vue e Next.js utilizam requisições HTTP para buscar os dados, mas oferecem diferentes formas de organizar componentes, estados, rotas e a comunicação com os serviços.

Entre os projetos analisados, os que mais se destacam para estudos são o **GitHub Issues Viewer**, por demonstrar integração com uma API real e gerenciamento de estado; o **PokeAPI React**, por possuir uma estrutura mais simples para iniciantes; e o **TMDB 2.0**, por apresentar o consumo de uma API dentro de um projeto Next.js com TypeScript.

## Fontes

- GitHub — React Weather App: https://github.com/arasgungore/react-weather-app
- GitHub — GitHub Issues Viewer: https://github.com/dceddia/github-issues-viewer
- GitHub — PokeAPI React: https://github.com/Onnichan/pokeapi-react
- GitHub — TMDB Posters API: https://github.com/escummy/tmdb-posters-api
- GitHub — React-Spotify: https://github.com/Pau1fitz/react-spotify
- GitHub — NASA API Front: https://github.com/papplo/nasa-api-front
- GitHub — Dashboard: https://github.com/zce/dashboard
- GitHub — Pokedex Vue/Quasar: https://github.com/tranmani/pokedex
- GitHub — TMDB 2.0: https://github.com/AhmedSemih/TMDB-2.0
- GitHub — Book Explorer: https://github.com/martian56/book-explorer
