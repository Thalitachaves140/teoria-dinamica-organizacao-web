## A Semântica por Trás da Apresentação:Desvendando a Estrutura Textual em HTML

**Atividade 1:**
*Análise da Estrutura Textual de Páginas Web (Individual)*

**página 1:** https://www.legiaodosherois.com.br/

Utilizando a ferramenta de ``inspecionar elemento``, temos:

A classe para ativar um tema escuro(dark mode,que altere o esquema das cores das telas dos programas) em uma página web,geralmente usando um CSS.

```javascript
<body class="bg--enabled theme--dark">:
```
Classe que pode ser utilizada para agrupar elementos para fins de estilos(usando class -),ou porque eles compartilham valores de atributos,como lang.
Ela deve ser utilizada somente quando não tiver outro elemento de semântico(tal como < article > - composição independente em um documento ou < nav > - seção de uma página que aponta para outras páginas ou para outras áreas da página):

```javascript
<div class="mobile-fixed-banner">:
```
Estrutura da barra de cabeçalho(header) de um site.Ele contém um elemento <  section  >  que encapsula o conteúdo da barra de cabeçalho,com a classe CSS site-header.
Dentro dessa seção,há um < div > com a classe container que define um contêiner para o conteúdo da barra,e um < div > com a classe row que utiliza um sistema de grade ( grid ) para organizar os elementos.

```javascript
<section class="site-header>
  <div class="container">
     <div class="row site-header_content">
        <a href="https://www.legiaodeherois.com.br" class="site-header_content_link">
           <img src="//www.legiaodeherois.com.br/wp-content/themes/legiao3.0.0/images/1h-logo/full.svg" width="120" heigth="22" alt="Logo da Legião">
        </a>
```
