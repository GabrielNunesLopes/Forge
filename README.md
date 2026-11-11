# 🛒 Pixel Forge Games - E-commerce Auditado e Validado pelo W3C

Projeto prático desenvolvido na Unidade Curricular de **Linguagem de Marcação (HTML5 & CSS3)**: loja virtual fictícia de hardware e periféricos gamer.

## 🌐 Links das Páginas Publicadas (GitHub Pages)
- 🏠 [Vitrine Principal (index.html)](https://gabrielnuneslopes.github.io/Forge/index.html)
- 🔍 [Detalhes do Produto (produto.html)](https://gabrielnuneslopes.github.io/Forge/produto.html)
- 🛍️ [Carrinho de Compras (carrinho.html)](https://gabrielnuneslopes.github.io/Forge/carrinho.html)
- 👤 [Cadastro e Checkout (cadastro.html)](https://gabrielnuneslopes.github.io/Forge/cadastro.html)

---

## ✅ Relatório de Conformidade W3C (Clique para Auditar em Tempo Real)

Todas as páginas deste repositório foram inspecionadas e validadas com **Zero Erros** nos validadores oficiais do consórcio W3C:

| Página / Arquivo | Status W3C | Link de Auditoria ao Vivo (W3C URI) |
| :--- | :---: | :--- |
| **`index.html`** | 🟢 100% Válido | [Verificar no W3C Nu Validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Fgabrielnuneslopes.github.io%2FForge%2Findex.html) |
| **`produto.html`** | 🟢 100% Válido | [Verificar no W3C Nu Validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Fgabrielnuneslopes.github.io%2FForge%2Fproduto.html) |
| **`carrinho.html`** | 🟢 100% Válido | [Verificar no W3C Nu Validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Fgabrielnuneslopes.github.io%2FForge%2Fcarrinho.html) |
| **`cadastro.html`** | 🟢 100% Válido | [Verificar no W3C Nu Validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Fgabrielnuneslopes.github.io%2FForge%2Fcadastro.html) |
| **`style.css`** | 🟢 CSS3 Válido | [Verificar no W3C Jigsaw CSS](https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fgabrielnuneslopes.github.io%2FForge%2Findex.html&profile=css3svg) |

---

## 🛠️ Diário de Bordo de Depuração

Erros e avisos encontrados pelo W3C antes da correção:

| Página Auditada | Linha | Mensagem de Erro / Aviso do W3C | Correção aplicada |
| :--- | :---: | :--- | :--- |
| `index.html` | 134 | The `aria-label` attribute must not be specified on any `p` element… | Tirei o `aria-label` do `<p>` da avaliação e coloquei no `<span>` das estrelas com `role="img"`. |
| `index.html` | 122 | The `aria-label` attribute must not be specified on any `p` element… | No cronômetro, troquei o `aria-label` por um texto escondido (`.sr-only`) lido pelo leitor de tela. |
| `index.html` | 361 | Warning: Section lacks heading | Coloquei um `<h2>` ("Receba ofertas exclusivas") na seção da newsletter. |
| `carrinho.html` | 64 | Warning: Section lacks heading | Troquei o `<section>` da lista por `<div>`, já que o título dela é o `<caption>` da tabela. |
| `carrinho.html` | 119 | Warning: This document has heading elements but none of them has a computed heading level of 1 | Adicionei um `<h1>` "Carrinho de compras" no início do `<main>`. |
| `style.css` | 67 | The property clip is deprecated / Invalid separator in shape definition | Troquei `clip: rect(0 0 0 0)` por `clip-path: inset(50%)`. |
| `style.css` | 353 | "mask": Too many values or values are not recognized | Refiz o corte dos tickets com `::before`/`::after` em vez de `mask`. |
| `style.css` | 744 | "-webkit-background-clip" is a vendor extension / The value "text" is deprecated | Refiz as estrelas com duas camadas de ★, sem `background-clip: text`. |

---

## 💻 Tecnologias

HTML5 e CSS3. O `script.js` cuida apenas do carrossel, das contas do carrinho e da confirmação do cadastro. Produtos, preços e promoções são demonstrativos: nenhuma compra é realizada.
