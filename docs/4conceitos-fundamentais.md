# 🧩 Conceitos Fundamentais do Flexbox

> Aqui vou registrar meus **aprendizados e experimentos**, com exemplos e exercícios que estou fazendo na prática.  

O objetivo é **entender os eixos, direções e hierarquia** do Flexbox de um jeito que faça sentido pra quem está estudando sozinho, como eu.  

---

## ⚡ Eixos Principal e Transversal

No Flexbox temos dois eixos:

- **Eixo Principal:** definido pelo `flex-direction` (linha ou coluna)  
- **Eixo Transversal:** perpendicular ao eixo principal  

💡 Quando mudamos `flex-direction`, os eixos se invertem.  
Exemplo visual (ASCII):
```
flex-direction: row
Eixo Principal → --->
Eixo Transversal ↓

flex-direction: column
Eixo Principal ↓
Eixo Transversal →
```


---

## 🔹 Flex Container vs. Flex Itens

- **Container:** controla o **comportamento de todos os itens** (ex.: `justify-content`, `align-items`)  
- **Itens:** têm propriedades próprias que podem sobrescrever o container (ex.: `flex-grow`, `align-self`)  

---

## 🌀 Ordem dos Itens

- A propriedade `order` permite **mudar a ordem visual dos itens**, sem alterar o HTML.  
- Exemplo rápido:

```html
<div class="container">
  <div class="item" style="order:2">Item 1</div>
  <div class="item" style="order:1">Item 2</div>
</div>
```

🏋️ Exercício Prático

Crie um container flex no VSCode.

Adicione 3 itens dentro.

Altere flex-direction (row, column) e veja como os eixos mudam.

Brinque com justify-content e align-items para alinhar e distribuir o espaço.

Tente mudar o order de alguns itens e observe o efeito sem mexer no HTML.

⚠️ Dica de estudo: escrever o código, ver o resultado e anotar o que mudou ajuda a fixar melhor do que só ler a apostila.

<div class="container">
  <div class="item">Item 1</div>
  <div class="item">Item 2</div>
  <div class="item">Item 3</div>
</div>

```html
<div class="container">
  <div class="item">Item 1</div>
  <div class="item">Item 2</div>
  <div class="item">Item 3</div>
</div>

<style>
.container {
  display: flex;
  border: 2px solid #333;
  height: 150px;
  gap: 10px;
  padding: 10px;
  background: #f0f0f0;
}

.item {
  background: #4caf50;
  color: white;
  padding: 20px;
  text-align: center;
}
</style>

