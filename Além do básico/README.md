# Além do básico

## Índice

1. [Cores, ilustrações, tipografia e fontes avançadas](#além-do-básico)
2. [Criando macros e ambientes personalizados]()
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

```

---