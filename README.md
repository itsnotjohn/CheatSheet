# Cheat Sheet: HTML, CSS, JavaScript e Conceitos Gerais

O repositório atual, denominado Cheat Sheet, foi solicitado pelo professor Iskailer com o objetivo de fornecer um recurso educativo prático para os alunos. O conceito de Cheat Sheet refere-se a uma "folha de cola", um guia resumido com informações chave, fórmulas ou processos essenciais, apresentados de forma concisa e de fácil acesso.

Neste caso, o repositório serve como uma ferramenta de apoio, permitindo que os estudantes consultem rapidamente os tópicos mais relevantes para o aprendizado. Embora seja uma excelente referência para revisar e reforçar o conhecimento.

# HTML

## Estrutura Básica

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Título da Página</title>
</head>
<body>
    <h1>Bem-vindo à minha página!</h1>
    <p>Este é um exemplo básico de HTML.</p>
</body>
</html>
```

## Tags mais Usadas

- `<div>`: Usado para agrupar elementos.
- `<p>`: Define um parágrafo de texto.
- `<h1>` a `<h6>`: Definem títulos, de maior a menor importância.
- `<a>`: Cria links.
- `<img>`: Insere imagens.
- `<form>`: Define um formulário.
- `<input>`: Cria campos de entrada em formulários.

### Exemplo de Formulário

```html
<form action="/submit" method="POST">
    <label for="name">Nome:</label>
    <input type="text" id="name" name="name">
    <input type="submit" value="Enviar">
</form>
```

### Boas Práticas

- Use tags semânticas para melhorar a acessibilidade e SEO (ex: `<header>`, `<footer>`, `<article>`, `<section>`).
- Feche sempre as tags corretamente.
- Indente seu código para manter a legibilidade.

## CSS

### Seletores

- Seletores de Elemento: `div`, `p`, `h1`
- Seletores de Classe: `.classe`
- Seletores de ID: `#id`

### Propriedades Essenciais

```css
/* Cor do texto */
color: #333;

/* Tamanho da fonte */
font-size: 16px;

/* Espaçamento interno */
padding: 10px;

/* Espaçamento externo */
margin: 20px;

/* Layout de blocos */
display: block;

/* Layout Flexbox */
display: flex;
justify-content: center;
align-items: center;

/* Layout Grid */
display: grid;
grid-template-columns: 1fr 1fr;
```

### Boas Práticas
- Evite o uso excessivo de `!important`.
- Use unidades relativas como `em`, `rem` e `%` para garantir responsividade.
- Organize seu CSS de forma modular, criando classes reutilizáveis.

## JavaScript
### Variáveis

```javascript
let nome = "João"; // Variável que pode ser reatribuída
const idade = 30;  // Variável constante
console.log(nome, idade); //João 30

nome = "Pedro"; // Variável reatribuída
console.log(nome); // Pedro
```

### Funções
```javascript
function saudacao(nome) {
    return `Olá, ${nome}!`;
}

console.log(saudacao("Maria")); // Maria
```

### Evento
```javascript
document.getElementById("btn").addEventListener("click", function() {
    alert("Botão clicado!");
});
```

### Manipulação do DOM
```javascript
document.getElementById("btn").addEventListener("click", function() {
    alert("Botão clicado!");
});
```

### Exemplo Prático
```javascript
<button id="btn">Clique-me</button>
<p id="titulo">Texto inicial</p>

<script>
    document.getElementById("btn").addEventListener("click", function() {
        document.getElementById("titulo").innerHTML = "Texto alterado após clique!";
    });
</script>
```
