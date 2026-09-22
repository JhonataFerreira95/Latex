# Introdução ao **LaTex**

## Índice

1. [O que é o `LateX`?](#introdução-ao-latex)
2. [Estrutura básica de documentos](#entendendo-a-estrutura-de-documentos)
3. [Formatação de texto e equações](#formatando-texto-e-escrevendo-equações)
4. [Tabelas, figuras e referências](#criando-e-formatando-tabelas-inserindo-e-manipulando-figuras-e-criando-referências-cruzadas-e-bibliográficas)

---

## Introdução ao `LaTex`

> Neste módulo, vamos aprender o básico. Primeiramente, você terá contato com a história e o contexto do LaTeX. Em seguida, você aprenderá como preparar o seu ambiente de trabalho para começar a utilizar a ferramenta.

---

- Quando se fala em `LATEX`, muitas pessoas pensam no material látex utilizado na produção de
borrachas, luvas e outros produtos. No entanto, o `LATEX` se trata de um sistema de preparação de documentos de alta qualidade, que inclui recursos projetados para a produção de documentação
técnica e científica. O `LATEX` é a versão de alto nível do `TEX`, um sistema de tipografia criado por `Donald Knuth`, que permite aos usuários focar o conteúdo dos seus documentos, em vez de se preocupar com os detalhes de formatação.

---

- `Word` e `LaTex`: Prós e contra;

    - `Word`:

        - Prós:

            - Familiaridade:

                - Sendo o editor mais conhecido no mundo, o `Word` é provavelmente a ferramenta mais utilizada. Consequentemente, seu orientador certamente domina o aplicativo—o que é importante, sem dúvida.

            - Facilidade:

                - `Word` é WYSIWYG (‘What you see is what you get’), o que significa que tudo que você faz (conteúdo) é diretamente mapeado para a página (forma). Você não precisa aprender a lidar com scripts ou com uma sintaxe especial. Fazer tabelas, inserir figuras, contar palavras… tudo é muito “simples” e intuitivo. Ou seja: se você quer escrever algo rápido e simples, `Word` oferece a vantagem da praticidade.

            - Aceitação de periódicos/eventos:

                - Infelizmente, muitos eventos/periódicos ainda não aceitam `LaTeX` em nossa área—principalmente no **Brasil**. Portanto, de nada adianta ter um artigo em `tex` se apenas `doc` é aceito. Isso é frustrante, porque conversões geralmente não são uma boa ideia.

            ---

        - Contra: 

            - Espaçamentos:

                - O `Word` simplesmente não lida bem com espaçamentos entre caracteres.

            - Velocidade:

                - Para documentos mais longos, o `Word` simplesmente atrasa a sua vida. Uma tese cheia de figuras e gráficos, por exemplo, causa lags frequentes.

            - Referências:

                -  É preciso ter um aplicativo separado para lidar com bibliografias. A interação com o `Word` não é tão ruim, mas programas como EndNote estão realmente longe do ideal (embora haja opções gratuitas).

            - Qualidade de layout:

                - Sem dúvida docs são esteticamente inferiores a texs. Documentos em `Word` simplesmente não têm o aspecto profissional que você encontra em publicações standard. Talvez o layout seja uma das grandes vantagens do `LaTeX`.

            - Ferramentas científicas:

                - Se você precisa de fórmulas, equações, diagramas, estruturas não lineares… o `Word` se torna inutilizável. Mesmo utilizando assistente de fórmula, o resultado fica bem longe do que você encontra em livros-texto.

            ---

    - `Latex`:

        - Prós:

            - Velocidade e automatização:

                - Um arquivo tex é rápido, já que trata de texto apenas. O output, em pdf, é obviamente mais rápido do que o doc, por razões óbvias. Links entre seções (também possíveis em `Word`) são facilmente implementados. O mesmo pode ser dito sobre figuras e gráficos, por exemplo.

            - Layout e ferramentas científicas:

                - Se você é perfeccionista e procura o layout mais profissional possível, use `LaTeX`. A interação entre diferentes tipos de objeto e texto flui de forma excelente, algo raro em `Word`.

            - Compatibilidade: 

                - Diferentes versões de `Word` podem causar mudanças bruscas de formatação em um doc. `TeX`, por outro lado, não sofre com esse tipo de problema. OK, pacotes são atualizados, e alguns detalhes podem mudar, mas o nível de compatibilidade é suficientemente baixo para que você possa simplesmente presumir que seja zero—principalmente quando comparamos com docs. Um tex pode ser aberto em virtualmente qualquer lugar. Você pode editá-lo mesmo sem ter LaTeX instalado, porque não é preciso compilar um tex para editá-lo: o resultado final (pdf) é um arquivo independente do arquivo com o conteúdo (tex).

            - Pacotes:

                - `LaTeX` é gratuito (open source). Há milhares de pacotes disponíveis para as mais variadas tarefas. Se você quer criar X, é bem provável que há um pacote para isso. Diferentes desenvolvedores pode adicionar funcionalidades a partir de pacotes—essa é a grande vantagem de sistemas open source (há outras, é claro). O número de desenvolvedores/programadores trabalhando no `Word` é limitado, o que significa que bugs demoram mais a serem corrigidos. Em sistemas abertos, como a Wikipedia, há um número absurdo de pessoas trabalhando constantemente para que a coisa toda funcione. Não há como competir: basta ver quantas pessoas ainda consultam a Britannica…

            - Aprendizado:

                - Usar `LaTeX` é aprender, constantemente, coisas diferentes. Se você nunca programou, utilizar `LaTeX` será uma introdução básica: você possivelmente irá partir para outras linguagens depois. Isso porque o feedback é bastante instantâneo: você aprende algo, compila, e percebe que conseguiu criar uma estrutura bastante complexa. Isso é estimulante, como qualquer atividade em que você aprende constantemente. Além disso, para pessoas que não são da computação/programação, como eu, usar `LaTeX` é uma ótima oportunidade de “pensar” em códigos. Você passar a entender uma nova sintaxe, e aplicar seus conhecimentos intuitivamente para criar aquilo que o `Word` não consegue. Isso é excelente não apenas para artigos/teses/dissertações, mas para handouts e apresentações de slides: muito do que usamos em Linguística exige uma certa complexidade gráfica, e transmitir isso nem sempre é intuitivo—principalmente em editores de texto como o `Word`.

            ---

        - Contras:

            - Basicamente, a desvantagem de `LaTeX` é a interface. Se você não se dá bem com computadores e sabe apenas o básico, dificilmente irá gostar de usar `LaTeX`. É preciso paciência e dedicação no início; coisas que antes eram simples são, de repente, complicadas; você vê erros e não sabe como corrigí-los, etc. Isso é comum a qualquer linguagem de programação, e simplesmente faz parte da coisa toda.

            - Por outro lado, se você gosta de desenvolver diferentes habilidades e se considera um usuário avançado, `LaTeX` será uma ótima opção. Se você está cogitando utilizá-lo é provável que você faça Mestrado ou Doutorado. Nesse caso, você certamente tem capacidade para aprender uma linguagem como TeX. Ou seja: as pessoas que normalmente procurarão `LaTeX` têm o nível de instrução necessário para aprender—afinal, pessoas que mal sabem usar um computador não devem estar pensando em publicar artigos científicos.

            ---

        - Conclusão:    

            - Para documentos pequenos e simples, `Word` sempre será uma boa opção. Para documentos complexos (acadêmicos), contudo, `LaTeX` será infinitamente superior. Se você  aplica rigor à forma do que produz (academicamente), utilizar `Word` realmente não é o caminho. A learning curve do `LaTeX` é um certo obstáculo, mas isso não deveria ser novidade se você está no mundo acadêmico—veja isso como uma oportunidade de desenvolver um skill técnico extremamente útil na sua educação/profissão.

---

## Entendendo a estrutura de documentos

> O `LateX` funciona como o código para escrita do texto atráves da compilação. Normalmente o código em `LateX` inicia com o `\`, usamos para escrever um comando em `LateX` e dentro desses comandos podemos adicionar argumentos, como obseva-se abaixo:

    ```tex

        \title{Meu primeiro documento}

    ```

    - Aqui escrevi um comando em `LateX` para demonstra o título.

---

- `Preâmbulo`:

    - O `Preâmbulo` é o inicio do documento entre o `documentclass` até o inicio do documento em `\begin{document}`.

---

- Comandos que denotam ambiente no `LateX`, onde se inicia um bloco de código e finaliza, estilo o `ruby`.

    ```tex

        \begin{document}

        \maketitle

        \section{Introduction}



        \end{document}

    ```

    - Observa-se que ele puxa muito da programação em `ruby`, podendo ter coisas aninhadas como um condicional em um escopo

---

- O comando em `LateX` começa com `\` e após isso a palavra reservada e caso necessário a opção e após o argumento:

    ```tex

        \documentclass[lipt]{article}

    ```

    - Observa-se acima um exeplo prático do que comentei.

    ---

    ```tex

        \maketitle

    ```

    - Exbie no centro como título os dados acima dele, serve para definir o escopo do título.

    ---

    - Quando deixo uma em linha em  branco entre texto e outro em `LateX`, tenho um paragráfo. Se eu colocar `\\` no final da frase, tenho uma quebra de linha, mas sem paragráfo.

---

## Criando um documento simples

> Nessa parte irei abordar as seções, que são responsáveis por dividir os artigos.

---

- Dicas para numeração:

    ```tex

        \section*{alpha}

        \section{beta}

    ```

    - Observa-se que aqui utilizei dois comandos com uma pequena diferença. O `alpha` com o `*`, sem o `*` fica com a numeração.

---

- `Subseções`:

    ```tex

        \section{alpha}

        \subsection{gama}

        \section{beta}

    ```

    - Aqui criamos uma subseção de `alpha` e essa subseção só acaba quando começa a seção `beta`

---

- `Subsubseções`:

    ```tex

        \section{alpha}

        \subsection{gama}

        \subsubsection{epsilion}

        \section{beta}
    
    ```

    - A `subsubseções` funcionam da mesma forma das `subseções`, acabam quando outras começãm.

---

- Comando para separar a página:

    ```tex

        \newpage

    ```

    - Serve para quebrar a página automáticamente.

---

- Exibindo comentários no `LateX`:

    ```tex

        \& comentário

    ```

    - Para exibir algum comentário no `LateX` usamos o `\&`

---

- Sumário:

    ```tex

        \tableofcontents

    ```

    - Esse comando gera uma sumário automático, sem necessidade de organizar o mesmo, basta por o comando onde quer que o sumário apareça, e pronto.

---

- Comando para mudar a lingaugem do documento:

    ```tex

        \usepackage[brazil]{babel}

    ```

    - O comando acima converte todo o documento para português brasileiro, pode utilizar esse comando para várias outras linguagens.

---

- Importando pacotes para o `Latex`:

    ```tex

        \usepackge

    ```

    - Observa-se que usamos o comando `\usepackge` para importa qualquer pacote em nosso documento `LateX`.

---

- Comando para deixar a data de hoje:

    ```tex

        \date{\today}

        \date{data_desejada}

    ```

---

## Formatando texto e Escrevendo equações

> Aqui irei aborda a como formatar um text em `LateX` quanto a criar equações no mesmo, de forma simples e rápida.

---

- Escrevendo uma `abstract` em `LateX`:

    ```tex

        \begin{abstract}


        \end{abstract}

    ```

    - Dentro desses comandos acima fica nosso `abstract` em `LateX`.

---

- Tamanhos de textos em `LateX`:

    ```tex

        {\tiny texto em tamanho tiny.}\\
        {\scriptsize texto tamanho scriptsize.}\\
        {\footnotesize texto em tamanho footnotesize.}\\
        {\small texto em tamanho small.}\\
        {\nromalsize texto em tamanho normalsize.}\\
        {\large texto em tamanho large.}\\
        {\Large texto em tamanho Large.}\\
        {\LARGE texto em tamanho LARGE.}\\
        {\huge texto em tamanho huge.}\\
        {\Huge texto em tamanho Huge.}\\

    ```

    - Aqui tem diversos tamanhos de textos em vários exemplos.

---

- Formatação de texto em `LateX`:

    ```tex

        \textbf{texto em negrito.}\\
        \textit{texto em itálico.}\\
        \underline{texto sublinhado.}\\
        \texttt{texto fonte monoespaçada}\\
        \textsc{texto em caixa alta.}\\
        \textsf{texto em fonto sem seriga.}\\
        \textsl{texto em fonte inclinada}\\

    ```

    - Observa-se que temos vários tipos de formatar um texto em `LateX`, desda fonte com `negrito` até fonte sem `serifa`, só ressaltando que podemos aidiconar tipos de formação com tamanhos como `{hug\textbf{\textit{veja como fica.}}}`

---

> Agora irei aborda a parte de como escrever equações matemáticas no `LateX`!

---

- Pare ter nossos símbolos das equações tudo ok, importe esses comandos abaixo:

    ```tex

        \usepackage{amsmath}
        \usepackage{amsfonts}
        \usepackage{amssymb}

    ```

    - São pacote criados pela associação americana de matemática.

---

- Escrevando equação em linha no `LateX`:

    ```tex

        \section{equação em linha}

        A minha equação predileta é $$x + y = z$

    ```

    - Observa-se que todo texto baixo se torna uma equação, ou quase todo. O padrão de todas as equações é o ítalico. Observe que usei dois símbolos de `$`, um no início e outro no final, isso detona o inicio de final do ambiente matemático.

---

- Segunda forma de escrever equações:

    ```tex

        \section{Destacada}

            A minha equação predileta é $$x + y = z$$

    ```

    - Observe que aqui é a mesma equação que passei anteriormente, mas a diferença que usei `$` dois símbolos para ficar centralizador e denotar o ínicio e fim da equação. 

---

- Enumerando equações: 

    ```tex

        \section{enumerada}
        \begin{equation}
        x + y = z
        \end{equation}

    ```

    - Aqui utilizando o `enumerada` para deixa a nossa equação númerada.

---

- Símbolos matemáticos:

    ```tex

        \section{símbolos}

        Letras grega podem ser escritas como $\alpha$, $\beta$, $\gamma$,$\delta$, $\epsilon$, $\zeta$, $\theta$, $\kappa$, $\lambda$, $\mu$, $\pi$ e $\omega$.\\
        Pode ser escritos em letras maisculas como $\Gamma$, $\Delta$, $\Theta$, $\Lambda$, $\Xi$, $\Pi$ e $\Omega$\\

    ```

    - Aqui escrevi várias letras gregas utilizadas para equações, tanto de forma normal quanto de maisculas.

---
        
- Subscript e superscript(escrevendo em baixo e em cima):

    ```tex

        \begin{align}
        x^2 + y_2 \\
        x^{2} + y_2 \\
        x^{2} + y_{2 + z1} \\
        x_{2} + y^{2+4} \\
        a^2 + b^2 = c^2
        \end{align}

    ```

    - Qual é funcionalidade? Serve para criar equações como uma subtração por exemplos, coisas simples. Como subir um numero e descer um outro, essa é a funcionalidade.

---

- Exibindo expressões metemática que o `LateX` consegue representar bem:

    ```tex

        /section{Operações}
        
        O Teorema fundamental do Cálculo é dado por:
        \begin{equation}
        \int_a^b f(x)\ \mathrm{d}x = F(b) - F(a)
        \end{equation}
        A definição de derivada é dada por:
        \begin{equation}
        \frac{\mathrm{d}f}{\mathrm{d}x} = \lim_{h \to 0} \frac{f(x + h) - f(x)}{h}
        \end{equation}
        O somatório de $l$ até $n$ é dado por:
        \begin{equation}
        \sum_{i = l}^n i = \frac{n \cdot (n + 1)}{2}
        \end{equation}

    ```

    - Aqui temos exemplos de onde o `LateX` se destaca, com foco no comando `\frac` para criar uma fração. Os demais comando irei explicar nos módulos mais a frente.

    ---

    - **\cdot**:

        - Utilizando esse comando em `LateX` para representar a multiplicação

    ---

    - **\frac{numerador}{denominador}**:

        - Como mencionei anteriormente, usamos esse comando para definir uma fração.

    ---

    - **\sum**:

        - Auto-explicativo, mas utilizamos para somar o resultado de nossas equações.
    
    ---

    - **\text**

        - Para utilizamos texto dentro do ambiente matemático usamos o `$\text{texto_sugerido} + {texto_sugerido}$`

---

## Criando e formatando tabelas, Inserindo e manipulando figuras e Criando referências cruzadas e bibliográficas.

> Aqui irei aborda como criar tabelas com diferentes números de colunas e linhas e como formatar o texto dentro das células de maneira simples e intuitiva. E também irei aborda  como inserir figuras em diferentes formatos e a manipular o seu tamanho e a sua posição.

---

- Agora irei aborda a parte de formatação tabelas e como criar as mesmas:

    ```tex

        \section{Tabelas}
        \begin{tabular}{lcr}
        esquerda & centro & direita\\
        1 & 2 & 3\\
        4 & 5 & 6\\
        7 & 8 & 9\\
        \end{tabular}

    ```

    - Para criar o ambiente das tabelas utilziamos o comando entre chaves `tabular`, e para determina o fim de um linha em uma tabela utilizamos o `\\`. O `lcr` significa para determina os lados da talela, sabendo `l` para `left`, o `r` para `right` e o `c` para o `centro`.  

---

- Tabelas com barras entres as colunas:

    ```tex

        \section{Tabelas}
        \begin{tabular}{|c|c|c|}
        esquerda & centro & direita\\
        1 & 2 & 3\\
        4 & 5 & 6\\
        7 & 8 & 9\\
        \end{tabular}

        \section{Tabelas}
        \begin{tabular}{|c|c|c|}
        \hline
        esquerda & centro & direita\\
        \hline
        1 & 2 & 3\\
        4 & 5 & 6\\
        7 & 8 & 9\\
        \hline
        \end{tabular}

    ```

    - Aqui em nosso argumento passamos o `|c|c|c|`, faz a criação de barras em volta da nossas colunas. A utilizaçõa do `\hline`, serve para criar barras na parte supererior e inferior da nossa tabela.

---

- Centralizando tabela:

    ```tex

        \begin{table}[h]
            \centering
            \begin{tabular}{|c|c|c|}
            \hline
            esquerda & centro & direita\\
            \hline
            1 & 2 & 3\\
            4 & 5 & 6\\
            7 & 8 & 9\\
            \hline
            \end{tabular}
            \caption{essa é minha tabela}
        \end{table}

    ```

    - Aqui utilizamos o comando `\centering` para centralizar a tabela de forma automática. Sobre o argumento passado em colchetes `[h]`, significa `here`, para sinalziar que a tabela está "aqui". Abaixo utilizei um `\caption{}` para detorna que é a minha tabela.

---

> Aqui aborda a parte de inserindo imagens e figuras.

---

- Importando o pacote `graphicx` para importa a imagem dentro do `LateX`:

    ```tex

        \usepackage{graphicx}

    ```

    - Aqui importei o pacote para usarmos livremente imagem no `LateX`.

---

- Inserindo figuras:

    ```tex

        \section{Figuras}
        \begin{figure}[h]
            \centering
            \includegraphics[width=.8\textwidth]{Assets/imagem_exemplo.png}
            \caption{Imagem de exemolo}
        \end{figure}

    ```

    - O código utiliza o ambiente `\begin{figure}` para inserir imagens. O comando principal é o `\includegraphics`, que recebe o parâmetro opcional `[width=.8\textwidth]` para definir a largura da imagem como 80% da largura do texto da página. Em seguida, entre chaves, informamos o caminho do arquivo `Assets/imagem_exemplo.png`, onde `Assets` é a pasta e `imagem_exemplo.png` é a imagem."

---

> Aqui irei aborda como fazer referência no `LateX`:

    ```tex

        \section{Figuras}
        \begin{figure}[h]
            \centering
            \includegraphics[width=.8\textwidth]{Assets/imagem_exemplo.png}
            \caption{Imagem de exemolo}
            \label{img:exemplo}
        \end{figure}


        veja a imagem \ref{img:exemplo}

    ```

    - Veja que aqui usei o comando `\label{img:nome_da_imagem_desejada}`, para fazer uma referência à uma imagem em meu texto.

---

- Referência equações em `LateX`:

    ```tex

        \section{Operações}
        
        O Teorema fundamental do Cálculo é dado por:
        \begin{equation}
        \int_a^b f(x)\ \mathrm{d}x = F(b) - F(a)
        \end{equation}
        A definição de derivada é dada por:
        \begin{equation}
        \frac{\mathrm{d}f}{\mathrm{d}x} = \lim_{h \to 0} \frac{f(x + h) - f(x)}{h}
        \end{equation}
        A definição de derivada é dada pela equação \ref{eq:derivada}
        \begin{equation}
        \frac{\mathrm{d}f}{\mathrm{d}x} = \lim_{h \to 0} \frac{f(x + h) - f(x)}{h}
        \label{eq:derivada}
        \end{equation}
        O somatório de $1$ até $n$ é dado por:
        \begin{equation}
        \sum_{i = 1}^n i = \frac{n \cdot (n + 1)}{2}
        \end{equation}


    ```

    - Aqui usei o mesmo conceito que usei para referência nossa imagem, mas com uma pequena mudança. Uso do comando pré `\label{ref:derivada}` e após a definição usei o comando `\label{eq:equação_desejada}` para referência nossa equação. 

---

- Agora irei aborda como usar `hyperlinks`, primeiramente vamos importa o mesmo:

    ```tex


    ```


