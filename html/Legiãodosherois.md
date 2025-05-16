## A Semântica por Trás da Apresentação: Desvendando a Estrutura Textual em HTML

## Atividade: 

*1-Análise da Estrutura Textual de Páginas Web (Individual)*

*Página 1:* https://developer.mozilla.org/pt-BR/ (Site de tutoriais e documentação web).

Utilizando a ferramenta de ''inspecionar elemento'', temos:

```html
<h1>HTML</h1>
<h2>Elementos Básicos</h2>
<h3>Parágrafos</h3>
```
As tags `<h1>` a `<h6>` são usadas para indicar seções importantes do conteúdo, facilitando a compreensão e navegação.

```html
<p>O elemento <code>&lt;p&gt;</code> nota.</p>
```
A tag `<p>`  é usada para explicar os conteúdos detalhadamente.

```html
<strong>Nota:</strong> 
```
A tag `<strong>` é usada para destacar alertas ou informações importantes.

````html
<p>É <em>nota</em> nota.</p>
````
A tag `<em>`  adiciona ênfase leve a determinadas palavras ou frases, geralmente exibidas em itálico.

```html
<p>Exemplo de uso:<br>&lt;p&gt;nota.&lt;/p&gt;</p>
```
A tag `<br>` é usada para separar linhas no texto.

```html
<hr>
```
A tag `<hr>` é usada para separar visualmente diferentes seções ou tópicos na página.

*2-Explorando a Organização com Listas (Individual)*

As tags `<ul>` e `<li>` são usadas para listar itens sem uma ordem específica, como categorias ou tópicos relacionados.

```html
<ul>
  <li>Fácil de aprender</li>
  <li>Ampla compatibilidade</li>
  <li>Estrutura semântica</li>
</ul>
```
As tags `<ol>` e `<li>` são usadas para listar vantagens, características ou passo a passo em tutoriais.

```html
<ol>
  <li>Abra o editor de código</li>
  <li>Escreva o código HTML</li>
  <li>Salve o arquivo com extensão .html</li>
</ol>
```
As tags `<dl>`, `<dt>`, `<dd>` definem termos e suas descrições, como em glossários.

```html
<dl>
  <dt>HTML</dt>
  <dd>Linguagem de marcação para estruturar conteúdo na web.</dd>
  <dt>CSS</dt>
  <dd>Folhas de estilo para definir a aparência do conteúdo.</dd>
</dl>
```

*3-A Expressão de Citações (Individual)*

A tag `<blockquote>` é usada para destacar normas ou declarações técnicas.

```html
<blockquote>
  "O elemento <code>&lt;section&gt;</code> representa uma seção genérica de conteúdo."
</blockquote>
```
A tag `<q>` é usada para citações curtas dentro de um parágrafo.

```html
<p>nota <q>semântico</q> nota. </p>
```
**O código da estrutura exemplificada com os elementos semânticos analisados, fica assim:**
````html

<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Guia de HTML - MDN Web Docs</title>
</head>
<body>
  <h1>Introdução ao HTML</h1>
  <h2>Elementos Básicos</h2>
  <p>O HTML utiliza <strong>elementos semânticos</strong> para estruturar o conteúdo de uma página web.</p>
  <p>Exemplo de uso:<br>&lt;p&gt;Este é um parágrafo.&lt;/p&gt;</p>
  <hr>
  <h3>Listas em HTML</h3>
  <ul>
    <li>Listas não ordenadas</li>
    <li>Listas ordenadas</li>
    <li>Listas de definição</li>
  </ul>
  <h4>Passos para Criar uma Página</h4>
  <ol>
    <li>Escrever o código HTML</li>
    <li>Salvar com extensão .html</li>
    <li>Abrir no navegador</li>
  </ol>
  <h5>Termos Importantes</h5>
  <dl>
    <dt>&lt;strong&gt;</dt>
    <dd>Define texto com forte importância.</dd>
    <dt>&lt;em&gt;</dt>
    <dd>Define texto com ênfase.</dd>
  </dl>
  <h6>Nota</h6>
  <blockquote cite="https://developer.mozilla.org/pt-BR/docs/Web/HTML">
    "Use elementos semânticos para melhorar a acessibilidade e SEO de suas páginas."
  </blockquote>
  <p>O guia afirma que <q>HTML é a espinha dorsal da web</q>.</p>
</body>
</html>
````
