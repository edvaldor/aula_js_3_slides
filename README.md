# Aula: Introdução ao JavaScript

📅 **Data:** 14/05/2025  
👨‍🏫 **Professor:** Edvaldo Rodrigues  
🏫 **Curso:** Análise e Desenvolvimento de Sistemas – UNIPAR  
🧑‍💻 **Disciplina:** Desenvolvimento para Internet – 1º Período

---

## 🎯 Objetivos da Aula

- Compreender o papel do JavaScript no desenvolvimento web.
- Aprender os conceitos de variáveis, funções, DOM e eventos.
- Desenvolver um exemplo prático interativo.
- Publicar um mini-projeto no GitHub e Vercel.

---

## 🧠 Conteúdo Abordado com Teoria

### 📌 O que é JavaScript?

JavaScript é uma linguagem de programação interpretada, voltada para a criação de comportamentos dinâmicos em páginas web. É executada no navegador do usuário e possibilita interatividade, manipulação de dados e integração com servidores.

---

### 🧱 Formas de inserir JavaScript

- **Inline**: diretamente em atributos HTML (não recomendado para projetos maiores).
```html
<button onclick="alert('Olá!')">Clique</button>
```

- **Interno**: dentro da tag `<script>` no HTML.
```html
<script>
  console.log("Olá!");
</script>
```

- **Externo**: recomendado, separando HTML e JS.
```html
<script src="script.js"></script>
```

---

### 📦 Variáveis: `var`, `let` e `const`

#### `var`
- Possui escopo de função (não respeita blocos).
- Pode ser redeclarada e atualizada.
- Evite em projetos modernos.

#### `let`
- Escopo de bloco (`{}`).
- Pode ser atualizada, mas **não redeclarada** no mesmo escopo.
- Ideal para valores que mudam.

#### `const`
- Escopo de bloco.
- **Não pode ser reatribuída.**
- Ideal para valores constantes ou estruturas que não mudam de referência (como objetos ou arrays).

```js
const nome = "Maria"; // ok
nome = "João"; // erro

const numeros = [1, 2];
numeros.push(3); // permitido
```

---

### 🧩 Funções em JavaScript

Funções são blocos de código que podem ser chamados e reutilizados. Elas recebem parâmetros e podem retornar valores.

```js
// Declarativa
function soma(a, b) {
  return a + b;
}

// Expressão
const saudacao = function(nome) {
  return "Olá " + nome;
};

// Arrow Function
const dobro = x => x * 2;
```

---

### 🖼 DOM – Document Object Model

O DOM representa os elementos HTML como objetos que podem ser manipulados com JavaScript.

#### Seletores comuns:

```js
document.getElementById("titulo");
document.querySelector(".classe");
document.querySelectorAll("p");
```

#### Manipulação:

```js
document.getElementById("titulo").innerText = "Novo título";
```

---

### 🎯 Eventos

Permitem reagir a ações do usuário (como cliques, teclas e movimento).

```js
element.onclick = function() {
  alert("Clique!");
};

// Recomendada:
element.addEventListener("click", () => {
  alert("Clicou!");
});
```

---

## 🧪 Exercício Proposto

Crie uma página HTML com:

- Um parágrafo (`<p id="texto">`) com conteúdo inicial.
- Dois botões:
  - Um para **alterar o texto do parágrafo**.
  - Um para **alterar a cor de fundo da página**.
- Use CSS para organizar o layout.
- JavaScript no final da página ou externo.

---

## 💡 Desafio Extra

- Use função que gera cor aleatória.
- Organize o código com boas práticas.
- Comente o código.

---

## 🚀 Publicação

1. Crie um repositório no GitHub com nome `aula-js-introducao`.
2. Suba seu projeto.
3. Publique no Vercel.
4. Adicione as **tags**:
   - `js-unipar-25`
   - `14052025`

---

## 📚 Referências Bibliográficas

- FLANAGAN, David. *JavaScript: O Guia Definitivo*. Bookman – on-line.
- [MDN Web Docs - JavaScript](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript)
- [W3Schools - JavaScript](https://www.w3schools.com/js/)

---

## ℹ️ Observações Finais

- Este conteúdo é parte integrante da disciplina e será utilizado para avaliação.
- Entregas fora do prazo terão descontos na nota.
- Em caso de dúvidas, contate o professor ou utilize o grupo da turma.
