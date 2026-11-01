# Estruturação de documentos 

## Índice

1. [Criando apresentações com `Beamer`](#criando-uma-apresentação-simples-com-beamer)
2. [Personalização de estilos e modelos](#estilizando-e-animando-suas-apresentações)
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

## Alterando o estilo dos capítulos e das seções

> Irei alterar o estilo dos capítulos e das seções de um documento de forma a deixá-lo mais bonito e com uma aparência mais profissional.

---

- Irei aborda um pacote para alterar qualquer tipo de comando de secção, basta importa o pacote abaixo em seu arquivo `LaTeX`.

```tex

    \usepackage{titlesec}

```

---

- Alerando o estilo da secção antes do meu preâmbulo no `LaTeX`.

```tex

    \titleformat{\section}[hang]
    {\nomalfront\bfseries\Large}
    {Seção \thesection}{0.5em}{\hrule\vspace{0.5em}}

```

- As regras acima fazem eu mudar o estilo das minhas `\section` e `\subsection`.

---

## Criando caixas de texto e exibições de código-fonte

> Como criar caixas de texto simples, com títulos e cores diferentes bem como a exibir códigos-fonte nos seus documentos.

---

- Para criar textos caixas, vamos usar o pacote abaixo:

```tex

    \usepackage{tcolorbox}

```

---

- Usando o `tcolorbox`:

```tex

    \section{caixas de texto}

    \begin{tcolorbox}
        \lipsum[1]
    \end{tcolorbox}

```

---

- Costumizando o `tcolor box`:

```tex

    \subsection{personalizando}

    \begin{tcolorbox}[colback=red!5!white,colfram=red!75!black,title=meu titulo]
        Essa caixa de texto
    \end{tcolorbox}

```

- Acima usei parâmetros dentro do `{tcolorbox}` para peprsonalizar nossa caixa de texto de forma simples.

---

- Dividino a caixa de texto:

```tex

    \subsection{personalizando}

    \begin{tcolorbox}[colback=red!5!white,colfram=red!75!black,title=meu titulo]
        caixa superior.
        \lipsum[1]
        \tcblower
        caixa de texto inferior.
        \lipsum[1]
    \end{tcolorbox}

```

- Esse comando `\tcblower`, divide a nossa caixa de texto em 2, com uma linha tracejada.

---

- Irei aborda como exibir código ou linguagem de programção via `LaTeX`, para isso basta importa esse pacote abaixo em seu documento `LaTeX`:

```tex

    \usepackage{minted}

```

---

- Usando o ambiente `mint`:

```tex

    \section{códigos em LaTeX}

    \begin{minted}[frame=lines, framesep=2mm, baselinesretch=1.2, bgcolor=gray!20!white, &fontsize=\footnotesize, linenos, numbersep=2mm]{ruby}
        def fatorial(n)
            if n == 0
                return 1
            else
                return n * fatorial(n-1)
            end
        end
    \end{minted}

```

- Aqui usei o comando `{minted}{ruby}` para apresentar um código `ruby` no `LaTeX`.

---

## Escrevendo artigos e relatórios científicos

> Como utilizar o LaTeX para publicações científicas, como artigos, utilizando modelos de periódicos e de conferências. Além disso, o tópico ensina a gerenciar documentos grandes e a resolver os problemas mais comuns.

---

## Gerenciando documentos grandes e resolvendo problemas comuns

- Irei aborda como utilizar o template de artigo do `NeurIPS`, que é adequado para publicações científicas. Também será abordado o uso do `ABNTeX2`, um pacote que permite utilizar o `LaTeX` para escrever documentos de acordo com as normas da `ABNT`.

    - Como é muito comum importa ou exporta coisas na progração, no `LaTeX` é algo bem comum inclusive, imagine ter que criar várias seções, mas o arquivo `.tex` é extesno, você pode apenas criar um novo arquivo e importe, assim se tornando uma tarefa mais simples, orgazinada de com boas práticas.

    ```tex

        \input{arquivo}

    ```

    - O comando acima serve para importe arquivos em `LaTeX`.

---










