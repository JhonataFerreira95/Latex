# Além do básico

## Índice

1. [Cores, ilustrações, tipografia e fontes avançadas](#além-do-básico)
2. [Criando macros e ambientes personalizados](#customizando-suas-listas)
3. [Utilizando `Latex` com outros `softwares`]()


---

## Além do Básico

> Neste módulo, você aprenderá sobre os elementos avançados do LaTeX para a criação de documentos mais complexos, como listas e enumerações, personalização do layout do documento e recursos avançados de formatação matemática e científica.

---

## Listas e Enumerações

- Aqui irei aborda como criar listas e Enumerações no `LateX`. Também irei aborda a forma prática, diferentes tipos de listas enumerações que podem ser criadas em `LateX`.

---

```tex

    \section{Lista Não-ordendas}

    \begin{itemize}

        \item \textbf{Negrito}
        \item \textbf{Itálico}

    \end{itemize}

```

- Nesse exemplo acima criei uma lista não ordenada para listar os dados que desejo.

---


```tex

    \section{Listas Enumeradas}

    \begin{enumerate}

        \item[+] \textbf{Negrito}
        \item[*] \textbf{Itálico}
        \item[] \textbf{Itálico}

    \end{enumerate}

```

- Nesse exemplo acima criei uma lista enumerada dos dados abordados.

---

## Customizando suas listas

- Aqui irei aborda como ersonalizar o `layout` das suas listas e enumerações. Além disso, aprenderá a alterar o símbolo ou a marca de enumeração, a indentação e o espaçamento entre os itens de uma lista.

---

```tex

    \section{Listas Enumeradas}

    \begin{enumerate}[a.]

        \item \textbf{Negrito}
        \item \textbf{Itálico}
        \item \textbf{Itálico}

    \end{enumerate}

```

- No código acima estou costumizando as linhas lista, ela vai ser alterada, no lugar de numeração de número vão ser utilizados letras

---

```tex

    \section{Listas Enumeradas}

    \begin{enumerate}[i]

        \item \textbf{Negrito}
        \item \textbf{Itálico}
        \item \textbf{Itálico}

    \end{enumerate}

```

- Acima fiz a mesma coisa com as lestras, mas com números romanos.

---

## Geometria da página

> Aqui irei abordar como personalizar o layout geométrico da página: ajuste das margens, espaçamento entre linhas e parágrafos, tamanho da página e quantidade de colunas.

---

- Antes de seguir, irei aborda o pacote `Lipsum`, para usarmos o `dame-text`, que é um texto que não vale nada, sem valor semântico. Para isso importe o comando abaixo em seu código `LateX`:

```tex

    \usepackage{lipsum}

    \lipsum[1-10]

```

- O código acima importa o pacote `lipsum` e o comando após criar vários texto sem valor semântico, de forma automática.

---

- Agora irei aborda o `geometry`, mas antes irei importa o comando para utilziar a geometria em `LateX`:

```tex

    \usepackage[top=2cm, bottom=3cm, left=1.5cm, right=3.5cm]{geometry}

```

- Dentro do `\usepackage{geometry}`, podemos abrir colchetes de colocar parâmetros para deixar a personalização da página ao nosso gosto.

---

- Definindo a margem uniforme:

```tex

    \usepackage[margin=2cm]{geometry}

```

- Definindo o padrão de margem da página em `LateX`

---

- Definindo o tamanho da página:


```tex

    \usepackage[margin=2cm, a4paper]{geometry}

```

- Acima utilizei o parâmetro `a4paper` para definiri o tamanho da página em `LateX`.

---

## Cabeçalhos e rodapés

> Ire aborda como criar cabeçalhos e rodapés personalizados. Você aprenderá a inserir o número da página, o título do documento e o nome do autor no cabeçalho e rodapé, além de inserir linhas e outros elementos gráficos.

--- 

- Antes de seguir, para tudo que irei abordar, utilizarei o pacote abaixo:

```tex

    \usepackage{fancyhdr}

```

---

- Mudando o estilo da página:

```tex

    \pagestyle{headings}

```

- Comando acima usamos para mudar o estilo da página.

---

- Agora irei aborda os cabeçalhos:

```tex

    \lhead{esquerda no topo}
    \chead{cetro no topo}
    \rhead{direito no topo}

```

- Os comandos acima são para gerar cabeçalho na esquerda, centro e direita da página.

---

- Irei aborda os rodapé:

```tex

    \lfoot{esquerda no rodapé}
    \cfoot{centro no rodapé}
    \rfoot{direita no rodapé}

```

- Os comandos acima são para gerar o rodapé na esquerda, centro e na direita da página.

---

## Aprendendo mais sobre Matemática no LaTeX 

> Recursos avançados de formatação matemática. Além disso, aprenderá a lidar com matrizes e vetores, a alinhar e agrupar equações matemáticas, e a utilizar diferentes estilos de símbolos matemáticos.

---
