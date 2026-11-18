# Aula 07 - Frameworks CSS

## Objetivo da Aula

Esta aula apresentou os fundamentos do CSS, o modelo de caixas, layouts responsivos, Flexbox e o uso de frameworks CSS. O objetivo foi compreender como organizar estilos e construir interfaces adaptáveis de forma consistente.

---

## Cascading Style Sheets

O CSS controla cores, fontes, margens, alinhamentos, dimensões e a disposição dos elementos da página.

Uma regra CSS possui a estrutura:

```css
seletor {
  propriedade: valor;
}
```

Exemplo:

```css
body {
  background-color: #ff0000;
}
```

## Formas de Aplicação do CSS

- **CSS inline:** aplicado diretamente no atributo `style` de um elemento;
- **CSS interno:** definido dentro da tag `<style>` no documento HTML;
- **CSS externo:** escrito em um arquivo `.css` vinculado pela tag `<link>`.

O CSS externo é recomendado para projetos maiores, pois facilita a reutilização e a manutenção.

## Principais Propriedades

- `color`: cor do texto;
- `background-color`: cor de fundo;
- `font-family`: família da fonte;
- `font-size`: tamanho do texto;
- `margin`: margem externa;
- `padding`: espaçamento interno;
- `border`: borda;
- `width` e `height`: largura e altura;
- `display`: tipo de exibição;
- `position`: posicionamento;
- `text-align`: alinhamento do texto.

## Classes e IDs

Classes podem aplicar estilos a vários elementos, enquanto IDs representam elementos únicos e específicos.

```css
.botao-primario {
  background: blue;
  color: white;
  padding: 10px;
}

#cabecalho-principal {
  height: 80px;
  background: #333;
}
```

## Box Model

O Box Model representa os elementos como caixas compostas por:

- **Content:** conteúdo do elemento;
- **Padding:** espaço interno;
- **Border:** borda;
- **Margin:** espaço externo.

Compreender o Box Model ajuda a controlar dimensões, espaçamentos e evitar problemas de alinhamento.

## Flexbox

Flexbox é um modelo de layout unidimensional utilizado para organizar elementos em linhas ou colunas.

Principais propriedades:

- `flex-direction`: define a direção dos itens;
- `justify-content`: distribui os itens no eixo principal;
- `align-items`: alinha os itens no eixo transversal;
- `flex-wrap`: permite que os itens quebrem linha;
- `gap`: define o espaçamento entre itens.

## Layout Responsivo

Um layout responsivo adapta o conteúdo a diferentes tamanhos de tela, como celulares, tablets e computadores. O objetivo é melhorar a usabilidade e evitar a criação de versões completamente separadas para cada dispositivo.

## Frameworks CSS

Um framework CSS fornece recursos, padrões, classes e componentes que ajudam a padronizar e acelerar o desenvolvimento de interfaces.

## Tailwind CSS

O Tailwind CSS é um framework Utility-First. Em vez de criar uma classe CSS para cada componente, combina-se no HTML pequenas classes que representam propriedades específicas.

Exemplo:

```html
<button class="bg-blue-600 text-white px-6 py-3 rounded-lg">
  Enviar
</button>
```

As classes podem controlar cor, tipografia, espaçamento, dimensões, bordas, Flexbox, grid e responsividade.

O Tailwind pode ser utilizado com o Play CDN para testes rápidos ou instalado por meio do Tailwind CLI em projetos maiores.

## Atividades

- Criar um projeto com CSS externo;
- Trabalhar propriedades de content, padding, border e margin;
- Utilizar pelo menos 20 propriedades de Flexbox;
- Construir uma interface responsiva;
- Criar uma atividade utilizando pelo menos 30 classes do Tailwind CSS;
- Documentar as classes utilizadas e o funcionamento da interface.

## Conclusão

CSS permite controlar visualmente a página, enquanto o Box Model e o Flexbox organizam dimensões e layouts. Frameworks como Tailwind padronizam estilos e aceleram o desenvolvimento, tornando as interfaces mais consistentes e responsivas.
