# Além do básico

## Índice

1. [Cores, ilustrações, tipografia e fontes avançadas](#cores-e-ilustrações)
2. [Criando macros e ambientes personalizados](#macros-e-ambientes-personalizados)
3. [Utilizando `Latex` com outros `softwares`](#latex-com-markdown)


---

## Além do Básico

> Aqui irei abordar algumas funcionalidades mais avançadas do LaTeX, como o uso de cores, ilustrações, criação macros e ambientes personalizados, além de utilizar a ferramenta com outros programas.

---

## Cores e ilustrações

- Como utilizar cores no seu documento, a definir as suas próprias cores e a criar ilustrações simples com `TikZ`.

```tex

    \usepackage{times}

```

- O pacote acima foi para importa uma fonte em `LaTeX`, a fonte em questão foi à `Times New Roman`. Isso vale para importar qualquer tipo de fonte em `LaTeX`.

---

## Tipografia e fontes avançadas

- Como  utilizar formatações de tipografia mais avançadas e a personalizar a sua tipografia. Antes de tudo vamos importa os pacotes;

```tex

    \usepackage{xcolor}
    \usepackage{tikz}

```

- Os pacotes acima são para ilustrações(`tikz`), para cores usamos o `xcolor`.

---

- Usando o `xcolor`:

```tex

    \section{Introduction}

    \textcolor{red}{\lipsum[1]}

```

- Acima usei o comando `\textcolor{red}` para definir a fonte do meu texto como vermelha.

---

- Usando o `colorbox`:

```tex

    \colorbox{gray}{grifando}

```

- Acima usei o comando parar gerar uma caixa na cor cinza em volta do texto. Geralmente utilizado para grifar apenas uma parte do texto.

---

- Alterando a cor da página:

```tex

    \pagecolor{yellow! 10}

```

- Acima usei o comando paga mudar a cor da página para amarelo. Observa-se que após o `yellow!` adicionei um `10`, significa que quero que a página tenha uma tonalidade de 10% de amarelo.

---

- Usando o `tikz`:

```tex

    \section{usando o pikz}

    \begin{tikzpicture}
        \draw (0,0) -- (1,1);
    \end{tikzpicture}

```

- O `tikz` funciona com um sistema de cordenadas. Observa-se que pedi para desenhar uma linha do ponto `0,0` até `1,1`, sempre finalizamos as cordenadas do `tikz` com **`;`**.

---

## Macros e ambientes personalizados

- Como criar macros e ambientes personalizados. Isso é útil para criar comandos e ambientes utilizados com frequência no seu documento.

---

- Criando um comando em `LaTeX`:

```tex

    \pagecolor{yellow! 10}
    \newcommand{\institution}{IFIRN}
    \maketitle

    \section{macros}

    A instituição de ensino é {\institution}

```

- Observa-se que criei o comando antes do `maketitle`, usando o comando `\newcommand` e após passando os parâmetros para o mesmo, usei ele chamando no texto no `LaTeX` usando o `{\institution}`, que foi o nome dado ao mesmo.

---

- Alerando comando já existentes no `LaTeX`:

```tex

    \pagecolor{yellow! 10}
    \newcommand{\institution}{IFIRN}
    \renewcommand{\epsilon}{\varepsilon}
    \maketitle

    \subsection{alterando comandos já existentes}

    Usando o novo comando para o $\epsilon > 0$


```

- Aqui alterei a forma do `epsilon`, sempre alterando antes do `maketitle` e usando o comando `\epsilon` para domonstra a nova forma do `epsilon`.

---

## Ambientes enumerados e contadores

> Irei abordar como enumerar certos ambientes e a criar ambientes com argumentos.

---

- Usando o comando `theorem`:

```tex

    \newtheorem{theorem}{Teorema}[section]

    \section{Introduction}

    \begin{theorem}[teste]
        \lipsum[1]
    \end{theorem}

```

- Acima utilizei o comando `theorem` para criar um novo teorma, adicionei o contato `section`, para a cada nova utilziação do `theorem`, ir contando de forma sucessetivamente.

---

- Alterando o contador da página no `LaTeX`:

```tex

    \pagenumbering{roman}

```

- Acima usei o estilo `roman` para alterar a numeração da página, para isso usei o comando `\pagenumbering`.

---

## LaTeX com Markdown

> Formatação de texto em `LaTeX`. Você aprenderá a formatar o texto em negrito, itálico, sublinhado, etc. Além disso, você verá como formatar o texto em diferentes tamanhos e fontes.

--- 