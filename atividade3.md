## Atividade 3:Detalhando a Arquitetura Cliente-Servidor na web

A comunicação entre um navegador web (cliente) e um servidor na internet é a base do funcionamento da web. 
Esse processo envolve diversas etapas e tecnologias que trabalham juntas para que você veja uma página web no seu navegador. Vamos detalhar esse fluxo passo a passo, explicando 
o papel de cada componente envolvido.

**1. O Papel do Cliente (Navegador Web)**
O cliente é geralmente um navegador web (como Chrome, Firefox, Safari), usado por um usuário para acessar páginas da internet. Ele é responsável por:

- Interpretar e renderizar o HTML, CSS e JavaScript recebidos do servidor.

- Enviar requisições HTTP para o servidor solicitando recursos.

- Exibir ao usuário o conteúdo retornado.

 **2. O Papel do Servidor**
O servidor é um computador (ou conjunto de computadores) conectado à internet, responsável por:

- Armazenar sites e aplicações web.

- Processar requisições recebidas do cliente.

- Enviar as respostas HTTP apropriadas com os arquivos requisitados (HTML, CSS, JS, imagens, etc.).

# Fluxo de Comunicação: Passo a Passo
**1. O usuário digita um endereço (URL) no navegador**
**Exemplo:**


https://www.fluxodecomunicação.com 

**2. Resolução de DNS (Sistema de Nomes de Domínio)**
O navegador precisa saber o endereço IP do servidor que hospeda o site.

O DNS (Domain Name System) converte o nome de domínio (www.nomededominio.com) em um endereço IP, como 192.0.2.1.

**Exemplo simplificado:**


www.resoluçãodeDNS.com → 192.0.2.1
**3. Estabelecimento da Conexão com o Servidor**
Com o IP conhecido, o navegador estabelece uma conexão com o servidor usando o protocolo TCP/IP.

Se o site usa HTTPS, é feita uma negociação segura (TLS) para criptografar os dados.

**4. Envio da Requisição HTTP (do Cliente para o Servidor)**
O navegador envia uma requisição HTTP, que é um pedido formal para acessar um recurso no servidor.

**Exemplo de uma requisição HTTP:**

```javascript
GET /index.html HTTP/1.1
Host: www.exemplo.com
User-Agent: Mozilla/5.0
Accept: text/html
```

*Isso indica: "Por favor, me envie a página index.html do domínio www.http.com".*

**5. O Servidor Processa a Requisição**
O servidor:

- Recebe a requisição HTTP.

- Verifica qual recurso foi solicitado.

- Busca esse recurso (por exemplo, um arquivo HTML ou o resultado de um script).

- Prepara a resposta HTTP.

6. Envio da Resposta HTTP (do Servidor para o Cliente)
O servidor envia a resposta HTTP, que contém:

Um código de status (por exemplo, 200 OK, 404 Not Found, 500 Internal Server Error).

Os dados requisitados (HTML, CSS, imagens etc.).

📝 Exemplo de resposta HTTP:

php-template
Copiar
Editar
HTTP/1.1 200 OK
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head><title>Exemplo</title></head>
  <body><h1>Olá, mundo!</h1></body>
</html>
7. O Navegador Renderiza a Página
O navegador recebe a resposta.

Lê o código HTML e começa a baixar os recursos adicionais mencionados no HTML (CSS, JS, imagens).

Exibe a página ao usuário.
