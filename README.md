# 💜 Huddle — Landing Page

> Projeto desenvolvido como parte dos desafios do **[Frontend Mentor](https://www.frontendmentor.io/)**, com o objetivo de praticar HTML e CSS na construção de uma landing page responsiva.

---

## 📸 Preview

![Preview do projeto](./preview.png)

---

## 🎯 Sobre o desafio

Este projeto é baseado no desafio **Huddle landing page with a single introductory section**, disponibilizado pelo Frontend Mentor.

A proposta é reproduzir uma página de apresentação a partir de um design fornecido, buscando manter o máximo de fidelidade possível ao layout original.

O principal objetivo foi praticar a construção de uma interface utilizando **HTML e CSS**, trabalhando principalmente com:

* Estrutura semântica do HTML
* Flexbox
* Responsividade
* Media Queries
* Espaçamento e alinhamento
* Tipografia
* Estados `:hover`
* Organização do CSS
* Adaptação do layout para diferentes tamanhos de tela

---

## 🛠️ Tecnologias utilizadas

<div align="center">

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge\&logo=html5\&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge\&logo=css3\&logoColor=white)
![Bootstrap Icons](https://img.shields.io/badge/Bootstrap%20Icons-7952B3?style=for-the-badge\&logo=bootstrap\&logoColor=white)
![Google Fonts](https://img.shields.io/badge/Google%20Fonts-4285F4?style=for-the-badge\&logo=googlefonts\&logoColor=white)

</div>

### Utilizados no projeto

**HTML5**
Responsável pela estrutura e organização dos elementos da página.

**CSS3**
Utilizado para estilização, posicionamento, responsividade, efeitos e adaptação do layout.

**Flexbox**
Utilizado principalmente para organizar os elementos do conteúdo principal, botão e redes sociais.

**Media Queries**
Utilizadas para adaptar a página entre dispositivos menores e telas maiores.

**Bootstrap Icons**
Utilizado para os ícones das redes sociais no rodapé.

**Google Fonts**
Utilizado para aplicar a fonte `Roboto` ao projeto.

---

## 🧱 Estrutura do projeto

```text
📦 huddle-landing-page
│
├── 📄 index.html
│
├── 📁 src
│   │
│   ├── 📁 css
│   │   ├── reset.css
│   │   ├── global.css
│   │   └── estilos.css
│   │
│   └── 📁 images
│       ├── logo.svg
│       ├── illustration-mockups.svg
│       └── favicon-32x32.png
│
└── 📄 README.md
```

---

## 🎨 Como a página foi construída

### 1. Estrutura HTML

A página foi dividida em três partes principais:

```html
<header>
```

Responsável pelo logo.

```html
<main>
```

Responsável pelo conteúdo principal da landing page.

```html
<footer>
```

Responsável pelos links das redes sociais.

Dentro do `main`, o conteúdo foi dividido entre a ilustração e a área de texto:

```text
MAIN
│
└── SECTION
    │
    ├── Ilustração
    │
    └── Lateral
        ├── Título
        ├── Descrição
        └── Botão
```

---

## 📐 Layout e responsividade

No início, o conteúdo é organizado verticalmente para telas menores:

```css
.conteudo {
    display: flex;
    flex-direction: column;
}
```

Para telas maiores, o layout passa a utilizar duas colunas:

```css
@media (min-width: 768px) {
    .conteudo {
        flex-direction: row;
    }
}
```

Dessa forma, a ilustração fica de um lado e o conteúdo textual do outro.

---

## 🔤 Controle da quebra do título

Um dos ajustes realizados foi controlar a largura máxima do título para reproduzir a quebra de linha presente no design original.

```css
.lateral h1 {
    max-width: 300px;
    font-size: 2rem;
    line-height: 1.2;
}
```

Assim, o navegador consegue distribuir o texto de forma semelhante ao modelo:

```text
Build The Community
Your Fans Will Love
```

---

## 📱 Footer responsivo

O rodapé também foi adaptado para diferentes tamanhos de tela.

Em telas maiores, os ícones das redes sociais ficam alinhados à direita:

```css
footer .redes {
    justify-content: flex-end;
    gap: 30px;
}
```

Além disso, o `body` utiliza Flexbox para manter o footer no final da página sem precisar utilizar `position: fixed`:

```css
body {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
}

main {
    flex: 1;
}
```

---

## ✨ Interações

O botão e os ícones das redes sociais possuem efeitos de `hover`.

### Botão

```css
.btn:hover {
    background-color: hsl(300, 69%, 71%);
    color: #fff;
}
```

### Redes sociais

```css
.redes i:hover {
    color: hsl(300, 69%, 71%);
}
```

Esses pequenos efeitos ajudam a deixar a interface mais dinâmica e próxima da proposta original.

---

## 📚 O que pratiquei neste projeto

* [x] HTML5
* [x] CSS3
* [x] Flexbox
* [x] Media Queries
* [x] Responsividade
* [x] Pseudo-classes
* [x] Tipografia
* [x] Organização de arquivos
* [x] Estrutura semântica
* [x] Posicionamento de elementos
* [x] Controle de espaçamento
* [x] Utilização de bibliotecas de ícones

---

## 🚀 O que pretendo melhorar

Este projeto faz parte do meu processo de aprendizado em desenvolvimento Front-End.

Alguns pontos que podem ser aprimorados futuramente:

* Melhorar a precisão do layout em diferentes resoluções
* Refinar os espaçamentos
* Melhorar a acessibilidade
* Adicionar estados de foco (`:focus`)
* Aperfeiçoar a responsividade para dispositivos menores
* Evoluir a organização e reutilização do CSS

---

## 🧠 Aprendizados

Mais do que simplesmente reproduzir uma imagem, este desafio serviu para entender melhor como transformar um design visual em uma estrutura real utilizando HTML e CSS.

Um dos principais aprendizados foi perceber que **pequenos detalhes fazem uma grande diferença no resultado final**: largura dos elementos, espaçamento, alinhamento, tamanho da fonte e comportamento em diferentes telas.

> "Código bom não é apenas aquele que funciona. É aquele que também faz sentido quando você volta para ele depois."

---

## 🏆 Frontend Mentor

Desafio disponibilizado por:

**Frontend Mentor**

O Frontend Mentor fornece desafios de desenvolvimento Front-End baseados em designs reais, permitindo praticar a construção de interfaces utilizando HTML, CSS e JavaScript.

🔗 [Acessar o Frontend Mentor](https://www.frontendmentor.io/)

---

## 👨‍💻 Desenvolvido por

**Samio Andrade Azeredo**

Projeto desenvolvido para prática e evolução dos conhecimentos em **Desenvolvimento Front-End**.

---

<div align="center">

### 💜 Desenvolvido com HTML + CSS

**Um desafio por vez. Uma linha de código por vez.**

</div>
