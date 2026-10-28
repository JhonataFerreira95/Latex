# Estruturação de documentos 

## Índice

1. [Criando apresentações com `Beamer`](#criando-uma-apresentação-simples-com-beamer)
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

- Usando blocos de texto com slides:

```tex

\section{Beamer 1}
\begin{frame}{Título}
    \framesubtitle{Subtítulo}
    \lipsum[1]
    \begin{block}{Título do block}
        ksksksksksk
    \end{block}
\end{frame}

```

- Aqui usamos o `block` para criar caixas de destaque com um título personalizado em apresentações de slides.

---

- Definindo sua instituição em slide no `LaTeX`:

```tex

\institute{IFRN}

```

- O comando aicma serve para definir sua instituição em um slide em `LaTeX`.

---

## Estilizando e animando suas apresentações

> Agora irei abordar como estilizar e animar as suas apresentações. Você verá como alterar o tema da apresentação, adicionar animações, criar blocos de texto, adicionar notas e criar apresentações em `.pdf`.

---

- Irei aborda o símbolos de navegação e os número do rodapé do slide:

```tex

\setbeamertemplate{navigation symbols}{}
\setbeamertemplate{footline}[frame number]

```

- O primeiro parâmetro abordado é para remover os símbolos de navegação do slide. O segundo é para marcar a pagina atual e as faltantes para finalizar o slide.

---

- Temas em nossos slide no `LaTeX`:

```tex

\usetheme{Warsaw}

```

- Acima adiconei o tema, mas pode pesquisa vários outros disponível para o `LaTeX`.

---


