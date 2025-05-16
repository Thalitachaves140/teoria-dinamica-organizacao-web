## Atividade 1: Descrevendo Efeitos Visuais com JavaScript

JavaScript é uma das principais tecnologias utilizadas para criar efeitos visuais dinâmicos e interativos em páginas web. Ele permite que os desenvolvedores modifiquem o conteúdo, o estilo e o comportamento dos elementos HTML em tempo real, respondendo a eventos do usuário, como cliques, movimentos do mouse ou rolagem da página.
**Como o JavaScript Cria Efeitos Visuais em Páginas Web?**
**1. Manipulação do DOM**
O JavaScript pode acessar e modificar qualquer elemento HTML através do DOM (Document Object Model). Isso permite alterar propriedades visuais diretamente, como posição, cor, opacidade, tamanho etc.

**Exemplo:**

```javascript
document.getElementById("caixa").style.backgroundColor = "blue";
```
Essa linha muda a cor de fundo de um elemento com o ID caixa.

**Interação com o CSS: Modificando Estilos Dinamicamente**
O JavaScript interage com o CSS de três formas principais:

**Modificando Estilos Inline**
 
```javascript
elemento.style.opacity = "0.5";
elemento.style.transform = "scale(1.2)";
```

**Alterando Classes CSS**
Você pode alternar classes inteiras que já têm estilos definidos no CSS:

```javascript
elemento.classList.add("ativo");
elemento.classList.remove("oculto");
elemento.classList.toggle("expandido");
```
## Trabalhando com CSS Custom Properties (Variáveis)
```javascript
document.documentElement.style.setProperty('--cor-tema', '#ff0000');
```
**Animações Simples com JavaScript Puro**
*1. Usando setInterval() ou requestAnimationFrame()*
Essas funções permitem criar animações quadro a quadro, alterando gradualmente valores CSS.

**Exemplo básico de animação:**


```javascript
let box = document.getElementById("box");
let pos = 0;

function mover() {
  if (pos < 300) {
    pos++;
    box.style.left = pos + "px";
    requestAnimationFrame(mover);
  }
}

mover();
```

## Diferença entre setInterval e requestAnimationFrame
setInterval: executa a cada intervalo de tempo fixo (não sincronizado com o navegador).

requestAnimationFrame: sincronizado com a taxa de atualização do navegador (melhor desempenho e suavidade).

# Uso de Bibliotecas JavaScript para Efeitos Visuais
As bibliotecas facilitam muito a criação de efeitos visuais complexos, abstraindo o código de baixo nível. Abaixo estão algumas das mais populares:

*1. jQuery*
Facilitou muito a criação de animações nos primórdios do JavaScript moderno.

**Exemplo:**

```javascript
$("#box").fadeOut(1000);
$("#menu").slideToggle();
```

*2. GSAP (GreenSock Animation Platform)*
Uma das mais poderosas bibliotecas para animações performáticas e complexas.

**Exemplo:**

```javascript
gsap.to("#quadrado", { x: 300, duration: 2, opacity: 0.5, scale: 1.2 });
```
Suporta timelines, easing, repetição, reversão, etc.

Ideal para animações profissionais (ex: jogos, banners, apresentações).

*3. Anime.js*
Famosa por seu equilíbrio entre simplicidade e poder.

**Exemplo:**

```javascript
anime({
  targets: '#circle',
  translateX: 250,
  rotate: '1turn',
  duration: 2000
});
```
## Fontes:
https://www.escoladnc.com.br/blog/aprimorando-a-experiencia-do-usuario-efeitos-visuais-em-desenvolvimento-web
https://www.aprendaprogramar.online/2024/05/criando-animacoes-com-css-e-javascript.html
https://www.webmundi.com/desenvolvimento-de-sistemas/javascript/criando-animacoes-basicas-com-javascript
https://awari.com.br/como-criar-animacoes-incriveis-com-javascript-guia-completo-para-iniciantes
https://mailchimp.com/pt-br/resources/javascript-animation

