# Estruturação de documentos 

## Índice

1. [Criando apresentações com `Beamer`]()
2. [Personalização de estilos e modelos]()
3. [Escrevendo artigos e relatórios cietíficos]()

---

## Estruturação de documentos

> Neste módulo, você vai aprender a estruturar diversos tipos de documentos em LaTex. Primeiramente, você será introduzido à classe Beamer, uma forma de criar apresentações em `LaTeX`.

---

## Criando uma apresentação simples com Beamer

- Aqui irei abordar a criação de uma apresentação simples utilizando a classe Beamer. Você verá como criar slides, adicionar títulos, subtítulos, listas, imagens, tabelas, equações e referências.

```tex

\documentclass{beamer}

```

- Esse comando acima, transforma o `PDF` para `slide` em `LaTeX`

---

- Utilizando o ambiente `frame`, para melhorar qualidade do nosos slide

```tex

\begin{frame}{Título}
    \framesubtitle{Subtítulo}
    \lipsum[1]
\end{frame}

```

- O comando acima serve para criar um título, um subtítulo e um bloco de texto. Para isso usamos os parãmetros do `freme` no ambiente `begin` e para subtítulo, usamos o `framesubtitle`.

---
