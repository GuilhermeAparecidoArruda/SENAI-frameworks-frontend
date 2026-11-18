# Aula 08 - Projeto React

## Objetivo da Aula

Esta aula revisou conceitos fundamentais de JavaScript e apresentou os principais recursos utilizados para construir componentes e interfaces com React.

---

## Revisão de JavaScript

O JavaScript pode ser incluído diretamente no HTML ou em arquivos externos. Ele permite utilizar variáveis, operadores, estruturas de controle, funções, arrays, objetos e eventos.

Principais conceitos revisados:

- `let` e `const`;
- tipos de dados;
- operadores aritméticos, de comparação e lógicos;
- condicionais `if`, `else` e `else if`;
- estruturas `for`, `while` e `do...while`;
- funções e arrow functions;
- arrays e objetos;
- manipulação do DOM;
- eventos como `click` e `input`.

## DOM

O DOM (Document Object Model) representa a estrutura HTML como uma árvore manipulável por JavaScript.

Podemos selecionar elementos com:

- `getElementById()`;
- `querySelector()`;
- `querySelectorAll()`.

O DOM pode ser alterado por propriedades como `textContent`, `value` e `classList`, além da criação de elementos com `createElement()`.

## JSX

JSX é uma extensão de sintaxe que permite escrever estruturas semelhantes ao HTML dentro do JavaScript.

```jsx
const nome = "João";
const saudacao = <h1>Olá, {nome}!</h1>;
```

No JSX:

- expressões JavaScript são escritas entre chaves;
- utiliza-se `className` em vez de `class`;
- utiliza-se `htmlFor` em vez de `for`;
- elementos sem conteúdo devem ser fechados, como `<img />`.

## Componentes

Componentes são funções que representam partes independentes da interface. Eles podem ser reutilizados em diferentes partes da aplicação.

```jsx
function Cabecalho() {
  return <h1>Catálogo React</h1>;
}

function App() {
  return (
    <main>
      <Cabecalho />
    </main>
  );
}
```

## Props

Props são dados enviados de um componente pai para um componente filho. Permitem reutilizar um mesmo componente com conteúdos diferentes.

```jsx
function Card({ titulo, descricao }) {
  return (
    <article>
      <h2>{titulo}</h2>
      <p>{descricao}</p>
    </article>
  );
}
```

## Virtual DOM

O DOM representa os elementos renderizados pelo navegador. O Virtual DOM é uma representação utilizada pelo React para coordenar as atualizações da interface.

Quando ocorre uma interação:

1. o componente é executado novamente;
2. o React calcula a nova descrição da interface;
3. a reconciliação compara a descrição atual com a anterior;
4. somente as diferenças necessárias são aplicadas ao DOM.

## Reconciliação e Keys

Durante a reconciliação, o React identifica quais elementos foram mantidos, adicionados ou removidos. Em listas, a propriedade `key` ajuda a preservar a identidade de cada item.

## Renderização de Listas

O método `map()` transforma itens de um array em elementos JSX.

```jsx
const alunos = ["Ana", "Bruno", "Caio"];

<ul>
  {alunos.map((aluno) => (
    <li key={aluno}>{aluno}</li>
  ))}
</ul>
```

## Renderização Condicional

É possível utilizar `if`, operador ternário ou operadores lógicos para mostrar partes diferentes da interface conforme os dados ou o estado.

```jsx
function Resultado({ carregando }) {
  return carregando ? <p>Carregando...</p> : <p>Busca finalizada.</p>;
}
```

## Atividade

Desenvolver uma aplicação React utilizando:

- JSX;
- componentes;
- props;
- Virtual DOM;
- listas;
- keys;
- renderização condicional.

O projeto deve ser enviado a um repositório público com um README descrevendo funcionalidades e conceitos utilizados.

## Conclusão

A Aula 08 apresentou a base do desenvolvimento de interfaces com React. JavaScript fornece a lógica, JSX descreve a interface, componentes dividem a aplicação em partes reutilizáveis e props permitem transportar dados entre componentes.
