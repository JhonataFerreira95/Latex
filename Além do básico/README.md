# Além do básico

## Índice

1. [Cores, ilustrações, tipografia e fontes avançadas](#cores-e-ilustrações)
2. [Criando macros e ambientes personalizados]()
3. [Utilizando `Latex` com outros `softwares`]()


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