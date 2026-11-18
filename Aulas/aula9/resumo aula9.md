# Aula 09 - Projeto React 02

## Objetivo da Aula

Esta aula apresentou recursos mais avançados do React: estado, formulários controlados, efeitos, consumo de APIs e navegação entre páginas com React Router.

---

## State e useState

State representa informações que podem mudar durante a utilização de um componente e que precisam atualizar a interface.

O Hook `useState` retorna o valor atual e uma função para modificá-lo:

```jsx
import { useState } from "react";

function Contador() {
  const [contador, setContador] = useState(0);

  return (
    <button onClick={() => setContador(contador + 1)}>
      Valor: {contador}
    </button>
  );
}
```

Uma variável comum não solicita automaticamente uma nova renderização. Por isso, estados são usados para atualizar a interface de forma previsível.

## Hooks

Hooks são funções especiais que permitem utilizar recursos do React em componentes funcionais. Seus nomes começam com `use`, como `useState` e `useEffect`. Devem ser utilizados no início do componente ou de outro Hook.

## Formulários

Em React, formulários podem ser controlados pelo estado. O valor do campo é definido pela propriedade `value`, e o evento `onChange` atualiza o estado conforme o usuário digita.

```jsx
const [nome, setNome] = useState("");

<input
  value={nome}
  onChange={(evento) => setNome(evento.target.value)}
/>;
```

Para enviar o formulário, usa-se `onSubmit` e `preventDefault()` para impedir o recarregamento automático da página.

## useEffect

`useEffect` permite sincronizar componentes com sistemas externos, como título da página, temporizadores, eventos do navegador e APIs.

```jsx
useEffect(() => {
  document.title = "Aula React";
}, []);
```

O segundo argumento controla quando o efeito será executado:

- `[]`: executa ao montar o componente;
- `[titulo]`: executa novamente quando `titulo` mudar.

## Limpeza de Efeitos

Alguns efeitos precisam ser encerrados para evitar recursos ativos indevidamente. O retorno do `useEffect` pode remover eventos ou temporizadores.

```jsx
useEffect(() => {
  window.addEventListener("resize", atualizar);

  return () => {
    window.removeEventListener("resize", atualizar);
  };
}, []);
```

## Consumo de APIs

Uma API permite que uma aplicação React consulte ou envie dados para um serviço externo.

O método `fetch` realiza requisições HTTP assíncronas:

```jsx
const resposta = await fetch(url);

if (!resposta.ok) {
  throw new Error("Erro na consulta");
}

const dados = await resposta.json();
```

O `useEffect` pode iniciar uma consulta quando o componente é exibido, e o `useState` pode armazenar os dados recebidos.

## Envio de Dados

Para enviar dados, utiliza-se o método `POST` e informa-se o formato do conteúdo:

```jsx
await fetch(url, {
  method: "POST",
  headers: { "Content-Type": "application/json" },
  body: JSON.stringify({ titulo: "Aprendendo React" })
});
```

## Cuidados com APIs

- verificar o status HTTP;
- tratar erros de rede;
- representar estados de carregamento, sucesso e erro;
- evitar dependências incorretas no `useEffect`;
- não armazenar chaves secretas no código do navegador;
- considerar autenticação, CORS e limites de uso;
- cancelar ações ou recursos quando o componente deixar de existir.

## React Router

React Router permite associar caminhos da URL aos componentes da aplicação.

```jsx
import { BrowserRouter, Routes, Route } from "react-router-dom";

<BrowserRouter>
  <Routes>
    <Route path="/" element={<Inicio />} />
    <Route path="/sobre" element={<Sobre />} />
  </Routes>
</BrowserRouter>
```

Principais recursos:

- `Link`: navegação entre páginas sem recarregar o documento;
- `Route`: associa um caminho a um componente;
- `Routes`: agrupa as rotas;
- `useParams`: acessa parâmetros presentes na URL;
- rotas aninhadas: organizam interfaces dentro de uma estrutura pai.

## Atividade

Criar uma aplicação React que utilize:

- `useState`;
- formulários;
- `useEffect`;
- consumo de APIs;
- React Router;
- estados de carregamento e erro.

O projeto deve possuir um repositório público e um README com descrição, funcionalidades e conceitos utilizados.

## Conclusão

A Aula 09 integrou os principais conceitos usados em aplicações React modernas. State controla dados mutáveis, formulários permitem entrada de informações, useEffect sincroniza componentes com sistemas externos, APIs fornecem dados e React Router organiza a navegação da aplicação.
