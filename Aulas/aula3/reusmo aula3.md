## Aula 03 - Projetos com Frameworks Front-end

**Objetivo da Aula:** 
Apresentar o ecossistema moderno de desenvolvimento front-end, diferenciando os conceitos de frameworks e bibliotecas, explorando seus paradigmas (componentização, reatividade) e analisando as principais ferramentas do mercado para auxiliar na escolha da melhor arquitetura para cada projeto.

---

**Resumo dos Tópicos:**
* **A Diferença entre Framework e Biblioteca:** Uma distinção crucial na arquitetura de software é a inversão de controle. Enquanto uma biblioteca (como o React tradicional) oferece ferramentas que você decide quando e onde chamar, um framework dita a estrutura do projeto e o fluxo de execução, exigindo que o desenvolvedor siga suas regras arquiteturais.

* **Princípios do Front-end Moderno:** Independentemente da ferramenta escolhida, o desenvolvimento moderno foca em organizar o código através de componentização (criação de blocos visuais isolados e reutilizáveis). Também utiliza programação reativa (a interface atualiza automaticamente quando os dados mudam) e arquitetura de Single Page Applications (SPA), onde o sistema de rotas troca o conteúdo da tela sem a necessidade de recarregar a página inteira no navegador.
* **React:** Ferramenta criada pelo Facebook, destaca-se pelo uso do Virtual DOM para atualizações rápidas na tela, pela sintaxe JSX (que permite escrever HTML dentro do JavaScript) e pela utilização de Hooks, como o `useState` (para gerenciar estado) e `useEffect` (para efeitos colaterais).

* **Angular:** Mantido pelo Google, é um framework robusto, completo e opinativo. Ele já traz soluções nativas para roteamento e requisições HTTP, utiliza obrigatoriamente a linguagem TypeScript (que adiciona tipagem ao JavaScript) e força uma arquitetura bem estruturada baseada no padrão MVC (Model-View-Controller).

* **Vue.js:** Destaca-se por ser um framework "progressivo", o que significa que pode ser adotado aos poucos em um projeto existente. É famoso por sua curva de aprendizado mais amigável e pelo uso de Single-File Components (arquivos com a extensão `.vue`), que unem HTML, CSS e JS em um único lugar de forma intuitiva.

* **Next.js:** Uma evolução dentro do ecossistema React. É um framework que resolve limitações tradicionais das SPAs, oferecendo renderização no servidor (SSR), o que melhora drasticamente o SEO e o desempenho inicial da página. Também traz o moderno App Router e funcionalidades nativas de otimização de imagens e Server Components.

---

**Conclusão da Aula:** 
A escolha entre React, Angular, Vue ou ecossistemas mais complexos como Next.js deve basear-se nas necessidades específicas do projeto e na curva de aprendizado da equipe. Mais importante do que decorar a sintaxe de uma única ferramenta é absorver os fundamentos universais do front-end moderno: componentização inteligente, gerenciamento de estado e ciclo de vida da interface.