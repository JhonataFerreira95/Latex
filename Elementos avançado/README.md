# Elementos avançados

## Índice

1. [Listas, enumerações e descrições](#listas-e-enumerações)
2. [Personalização do `layout` da página](#geometria-da-página)
3. [Recursos de matemática e ciência](#aprendendo-mais-sobre-matemática-no-latex)

---

## Elementos avançados

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

- Antes de seguir para o ambiente matemático, devo ressaltar a importância do pacote `amsmath` e `amssymb` para os símbolos, para usarmos todo o potência e formas disponível:

```tex

    \usepackage{amsmath}
    \usepackage{amssymb}

```

---

- Irei aborda alguns comandos essênciais para criar cálculos em `LateX`. Começarei falando de `Matrizes`

```tex

    \section{Matrizes}

    \begin{equation}
    A =
        \begin{pmatrix}
            1 & 2 & 3\\
            0 & 4 & 5
        \end{pmatrix}

    \end{equation}

```

- Acima utilziei a matriz, dentro do ambiente `equation`, para detonar a ragião da matriz usamos o comando `\begin{matrix}`, para deixar formatado com parênteses usamos o `pmtrix`.

---

- Sistema e casos:

```tex

\section{sistemas e casos}

\begin{equation}
    Y =
    \begin{cases}
        1, Y>X \\
        0, Z\le Y
    \end{cases}
\end{equation}

```

- Acima usamamos o ambiente `case`, para detornar uma parte de um sistema matemático.

---

- Diferentes estilos:

```tex

\section{diferentes estilos}

\begin{itemize}
    \item $\mathbf{x}$: negrito;
    \item $\mathcal{x}$: caligrafia;
    \item $\mathfrak{x}$: gótico;
    \item $\mathbb{x}$: balckboard;
    \item $\mathit{x}$: itálico;
    \item $\mathrm{x}$: romano;
\end{itemize}

```

- Acima apresento diferentes estilos para escrever nossas equações/matrizes or casos.

---

- Marcações gráficas:

```tex

\section{marcas gráficas}

\begin{itemize}
    \item $\hat{x}$: chapeu;
    \item $\bar{x}$: barra;
    \item $\vec{x}$: vetor;
    \item $\dot{x}$: ponto;
    \item $\tilde{x}$: til;
    \item $\ddot{x}$: dois pontos;
    \item $\dddot{x}$: três pontos;
\end{itemize}

```

- Observa-se acima que abordei algumas marcas gráficas para serem colocadas em nossas expressões.

---

## Melhorando a aparência de suas equações e expressões científicas

> Formatar equações e expressões científicas. Também será apresentado a diferentes pacotes para facilitar o uso de símbolos matemáticos e relacionados à Física e Química.

---

- Agora irei aborda o ambiente `align`:

```tex

\section{alinhamento}

\begin{align*}
    x + y &= z \\
    k &= j - o 
\end{align}

```

- Observa-se que acima usei o ambiente `align`, que por si só já é um ambiente matemático, após o mesmo usei o `*`, serve para remover as numerações das equações. Para alinhar de forma uniforme, usamos o `&` para alinharmos onde for necessário. 

---

- Alinhamento de equações de forma diferentes:

```tex

\begin{align*}
    x - 5 &= 2 & 2y + 2 &= 1 \\
    x &= 7 & 2y &= -1 \\
    & & y &= - \dfrac{1}{2}
\end{align*}

```

- Aqui estou alinhando as equações de forma diferente, dispor elas. 

---

- Espaçamento:

```tex

\section{Espaçamento}

\begin{itemize}
    \item $x = y$: sem espaçamento;
    \item $x \, = \, y$: espaçamento pequeno;
    \item $x \: = \: y$: espaçamento médio;
    \item $x \; = \; y$: espaçamento grande;
    \item $x \! = \! y$: espaçamento negativo;
    \item $x \quad = \quad y$: espaçamento de tamanho de um caractere;
    \item $x \qquad = \qquad y$: espaçamento de tamanho de dois caracteres.
\end{itemize}

```

- Acima abordei os tipo de espaçamento no `LateX`.

---

- Pacotes `mhchem` para química e o `physics` para física. Para isso importe os pacotes abaixos:

```tex

\usepackage{mhchem}
\usepackage{physics}

```

- Importei ambos os pacotes.

---

- Usando parâmetros em química:

```tex

\section{química}

    \ce{H2O + C -> H2 + CO}

```

- Acima usei comandos para criar uma fórmula química.

---

- Irei aborda a parte dos parâmetros de física:

```tex

\section{Física (e matemática)}

\begin{align*}
    \dv[x] \sin(x) &= \cos(x)\\
    \dv{\sin(x)}{x} &= \cos(x)\\
    \dv[2]{x} \sin(x) &= -\sin(x)\\
    \pdv{x} f(x, y) &= y\\
\end{align*}

```

- Acima abordei a parte de física com os parãmetros em `LateX`.

---

