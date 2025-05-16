## Atividade 2: Analisando a Validação de Formulários com JavaScript 
 **Expressões Regulares (RegEx)**
*O que são?*
Expressões Regulares são padrões usados para verificar se um texto segue uma determinada estrutura. No contexto de formulários, elas são muito úteis para validar formatos como:

- E-mails

- Números de telefone

- CEPs

- Códigos postais

- Senhas com regras específicas

**Exemplo: Validação de E-mail com Expressão Regular**
```javascript
const regexEmail = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
```
**Explicação do padrão:**
Padrão	Significado

*^*	Início da string

*[^\s@]+*	Um ou mais caracteres que não sejam espaço (\s) ou @
@	O caractere "@" obrigatório

*[^\s@]+*	Um ou mais caracteres novamente após o "@"
\.	Um ponto literal "."

*[^\s@]+* Um ou mais caracteres após o ponto

$	Fim da string

## Fontes
www.developer.mozilla.org


