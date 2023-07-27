# Conceitos Básicos

As inferências e deduções que realizamos na nossa rotina são baseadas, em grande parte, no raciocínio lógico. Uma médica deve raciocinar, a partir dos sintomas demonstrados, o diagnóstico; o mesmo faz um mecânico de automóveis (afinal, são muito parecidos, ambos dizem no final que o problema está na rebimboca da parafuseta, e a gente acredita e gasta a  grana que não tem pra consertar). Detetives da televisão ou da vida real devem processar as pistas coletadas de forma lógica para tentar chegar a teorias de como os crimes aconteceram. Donos de empresa tomam decisões de negócio baseadas na análise lógica dos sinais do momento e das possibilidades futuras. Uma jurada num tribunal deve pesar as evidências e seguir a lógica de quem acusa e de quem defende: **se** o réu estava no cinema na hora do crime, **então** ele não poderia ter cometido o crime. No fim das contas, qualquer atividade de *resolução de problemas*, ou o que os educadores chamam de *pensamento crítico*, envolve um casamento de padrões e a chegada a conclusões através de um caminho lógico.

Pensamento dedutivo é crítico na ciência, com as regras de inferência sendo a base da formulação (esse virus inativado, se injetado, protege o ser humano contra o novo Coronavirus) e testagem (aplicar e observar o resultado em 3000 voluntários) de hipóteses científicas.  Independente de ser realizado por uma pessoa ou um computador, o procedimento de passos lógicos, seguidamente, um após o outro, asseguram que as conclusões são consequências corretas dos dados iniciais. Sem isso, a ciência seria pura bruxaria (não que às vezes ela não seja 🧙🏻). A certeza que a lógica nos fornece para avançar o conhecimento é de importância imensurável.

> A Lógica é o alicerce de todo conhecimento que adquirimos.

*Leonhard Euler*

Mesmo que pratiquemos o procedimento lógico desde a primeira infância, ainda caímos em armadilhas lógicas inúmeras vezes. Eu estudo a lógica em detalhes há muitos anos e mesmo assim cometo erros lógicos frequentemente. Na verdade estudos científicos, com testes em pessoas adultas educadas, mostram que muitos cometem erros em deduções simples. E o mundo está cheio dessas cascas de banana esperando a gente escorregar.

Quando a gente preenche formulários pra tirar um documento, ou pra fazer uma declaração de imposto de renda, somos obrigados a compreender logicamente o que está sendo pedido, e muitas vezes problemas de inferência lógica no próprio formulário podem gerar dores de cabeça. Por exemplo, suponha que, no formulário, você depare com a regra "Todos que residem em Campina Grande devem ignorar os campos 13 e 14". Suponha então que você more em Lagoa Seca. Você deve então preencher os campos 13 e 14? Muitas pessoas inteligentes diriam que sim, você deveria preencher. Na verdade a resposta certa é "não sabemos, talvez sim, talvez não, já que não há informação suficiente". Se a regra fosse "Apenas aqueles que residem em Campina Grande devem ignorar os campos 13 e 14", saberíamos que você, distinto residente de Lagoa Seca, deveria preencher esses campos.

Sendo justo com os criadores dos formulários, há um problema aí mais sério do que a inferência lógica: a interpretação da linguagem falada ou escrita pode ser inconsistente, de pessoa para pessoa. Considere que, em uma estrada, tem uma placa dizendo "Tráfego intenso até a saída para Recife"; a maioria das pessoas interpretaria que o trânsito estará tranquilo depois da saída para Recife. Mas eu poderia considerar que a premissa aqui é não afirmar nada sobre o que acontecerá depois da saída, apenas que antes vai ter tráfego.

Mais um exemplo de como a dedução lógica pode ser sutil. Vamos considerar o seguinte problema:

**Estou pensando em uma das duas cores (cinza ou branco) e em uma das duas formas (losango ou círculo). Se um símbolo tem a cor que eu estou pensando, ou a forma que estou pensando, ou ambos, então eu o aceito, senão eu o rejeito. Eu aceito o losango cinza. Eu devo rejeitar quais dos símbolos abaixo?**

![intro/Untitled.png](intro/Untitled.png)

Uma inferência incorreta frequente é concluir que o círculo branco deve ser rejeitado. Estranho, né? Mas veja: o losango cinza pode ser aceito se o experimentador estiver pensando em *círculo* e *cinza*...nesse caso, o círculo branco não pode ser rejeitado! O que erramos é assumir que, na aceitação de losango cinza, o experimentador traz alguma informação adicional que definiria o problema, mas na verdade não sabemos de nada que nos faria saber a escolha final dele! Ou seja, não dá pra fazer a inferência que pensamos poder fazer. E essa é uma situação mais comum do que se imagina. Os métodos dedutivos que veremos nesta disciplina vão revelar várias anomalias semelhantes a esta no nosso raciocínio.

## Conceitos que vamos precisar

Quero aqui definir um terreno comum por onde vamos caminhar até o final da disciplina. Começo já dizendo que há grande chance de você ler versões diferentes dos conceitos que vamos usar aqui, já que escolhas tiveram que ser feitas ao definir os conceitos mais consistentes com o restante dos assuntos que vamos ver. Essa variedade de conceitos adotados por diferentes autores vem do fato da lógica ser uma ciência com aplicações em campos diversos do conhecimento: matemática, filosofia, linguística, computação, retórica, etc. Assim, cada um acaba adotando as definições que melhor lhe convém.

Nosso tijolo fundamental é a **sentença**, que no estudo da língua portuguesa se apresenta frequentemente como *oração* , algo gramaticalmente bem montado que inclui pelo menos um verbo flexionado.

1. Esse tema é muito interessante
2. Já viveram seres inteligentes em Marte?
3. Feche a porta!

Ah, mas para a lógica, nem todas essas sentenças são de interesse! As que nos interessam de verdade são aquelas que chamamos de **sentenças declarativas**, aquelas que podemos inquirir se são ou não verdadeiras. Na lista anterior, apenas a sentença 1 é declarativas; o restante não é alvo da lógica. Veja que a sentença é declarativa independente do valor que damos à ela. Se ela for passível de classificação como verdadeira ou falsa, ela é sentença declarativa. Vale a pena adicionar que certas sentenças declarativas são vagas o suficiente para serem meio que descartadas do raciocínio lógico:

* Gostaríamos de reduzir o desemprego
* Prometo dizer toda a verdade

No contexto da lógica proposicional (nosso próximo assunto), chamaremos uma sentença declarativa de *proposição*; na verdade o conceito de proposição é um pouco diferente de sentença declarativa, já que um exemplo da primeira pode ser representada por várias sentenças diferentes. Veja: "o peixe morreu", "o peixe está morto"; são duas sentenças diferentes, mas definem uma mesma proposição, algo que pode ser julgado verdadeiro ou falso.

Dadas as proposições, como fazemos para usá-las em raciocínios? Os seres humanos raciocinam, tentando estabelecer novos conhecimentos a partir do que já se conhece. Tentamos persuadir outros sobre alguma coisa fornecendo razões para aquilo. A lógica é o estudo do que conta como boas razões para algo. 

Os raciocínios se dão através do conceito de **argumento** -- o mais importante desta disciplina. Começo com exemplos de argumentos.

1. Se o parâmetro não for uma string vazia, o retorno da função é positivo. O retorno da função não foi positivo. Logo, o parâmetro enviado foi uma string vazia.
2. Precisarei treinar a equipe se o aplicativo foi feito em Python. O aplicativo não foi feito em Python. Por isso, não precisarei treinar a equipe.

A gente vai chamar essas sentenças declarativas que vêm antes das conjunções "Logo" e "Por isso" de **premissas**, sendo elas as *razões* dadas pelo argumento para nos convencer, ou persuadir. Já o que vem depois disso chamamos de **conclusão**, normalmente uma só. Os argumentos acima representam dois diferentes raciocínios, ou talvez processos de raciocínio. Leia com atenção, e tente acompanhar os raciocínios. Você concorda com eles? O argumento 1 parece perfeito, mas o argumento 2 nos faz duvidar dele. Pois é, este é o que consideramos como argumento **inválido**, enquanto que o primeiro é **válido**.  

Vamos a uma definição mais precisa: argumentos são uma coleção de sentenças declarativas, uma das quais se chama *conclusão* e cuja verdade procura-se estabelecer; as outras sentenças chamam-se *premissas*, e estas afirmações pretendem conduzir à conclusão (ou apoiá-la, ou persuadir-nos da sua verdade). À conclusão chamamos às vezes *o objetivo do argumento* ou a questão em discussão. Ter um bom conhecimento de lógica, enfim, envolve determinar se nos devemos deixar persuadir que uma afirmação é verdadeira ou que estamos perante um bom argumento; é o que nos capacita também em saber formular bons argumentos.

A lógica se preocupa primordialmente com a validade dos argumentos. Veja isso aqui:

* Moscou é a capital dos EUA. Por isso, para ir à Moscou você precisa ter visto americano.

Aqui a premissa é completamente falsa. No entanto, podemos desconsiderar o argumento? Se a conclusão segue das premissas, ou seja, se há *inferência*, a lógica conclui que o argumento é válido. Como elemento de persuasão este argumento não é útil, mas não deixa de ser válido, do ponto de vista lógico.

A definição mais direta de argumentos válidos: as premissas justificam a conclusão. Para nós, mais importante é saber que, num argumento válido, *sempre que as premissas forem verdadeiras, a conclusão com certeza também é*. Vamos discutir isso semanticamente mais tarde no curso, e isso vai ficar mais preciso.

Perceba que um argumento válido não necessariamente é um *bom* argumento, como aconteceu no exemplo de Moscou acima. A classificação de um argumento *bom* ou *ruim* muitas vezes independe da lógica; existem argumentos inválidos que podem ser considerados bons, por incrível que pareça, como no exemplo abaixo:

* Os cabelos de Júlia são castanhos. Mas hoje ela apareceu com os cabelos loiros. Por isso, ela tingiu os cabelos

O argumento não é válido, pois há situações em que as premissas são verdadeiras com conclusão falsa -- e se Júlia estiver usando peruca? Mas as premissas são plausíveis, e a conclusão tem possibilidade forte, mesmo que, rigorosamente, não dê para concluir. Podemos dizer, na verdade, que o argumento é **indutivamente válido**, que vem de uma noção importantíssima, já que raciocinamos indutivamente o tempo todo ao tentar entender o mundo. Na lógica para computação, no entanto, estamos mais interessados na validade dos argumentos; indução está bem mais relacionada às ciências humanas.


### Referências

*Logic: a Very Short Introduction*. Graham Priest. Oxford Press. 2016.

*Introdução à lógica*. Cezar A. Mortari. 2a. Edição. 2017.

*Pensamento Crítico: o poder da lógica e da argumentação*. Walter Carnielli e Richard Epstein. Rideel.  2011. 


