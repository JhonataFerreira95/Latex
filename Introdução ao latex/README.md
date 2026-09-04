# Introdução ao **LaTex**

## Índice

1. [O que é o `LateX`?](#introdução-ao-latex)
2. [Estrutura básica de documentos](#entendendo-a-estrutura-de-documentos)
3. [Formatação de texto e equações]()
4. [Tabelas, figuras e referências]()

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