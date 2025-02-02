# Formas Normais: Motivação

Recentemente deparei com uma postagem no [Stack Overflow](https://stackoverflow.com/questions/6574929/why-is-it-important-to-express-code-in-disjunctive-normal-form) que relatava um padrão de organização de programas dentro de uma empresa. Mais ou menos assim:

> At the company I work for, there has recently been a mandate that all 'highly visibile' boolean logic must be expressed like this:

```
if (defined(A) || (defined(C) && defined(D)) || defined(B))
```

> What is the motivation for mandating that code has to be expressed in this manner? What are the advantages?

Percebam o formato da condição do if; há nele apenas disjunções, e dentro de cada disjunção, apenas conjunções. Uma das respostas que está no site dá uma ideia para a motivação disso:

*Always remember that in many languages both operands of a boolean expression may not be executed if the value of the expression can be determined after evaluating just one of the operands. Such as:*

*1: (trueMethod() || falseMethod())*

*2: (falseMethod() || trueMethod())*

In case one only trueMethod() is executed. But in Case 2 both methods are executed. Order can make a big difference.

Sim, a **ordem faz uma diferença** no processamento da condição, deixando a execução mais rápida quando não é necessário processar o restante da fórmula. Lembre-se, a condição do *if* é uma fórmula na lógica proposicional (sem incluir a implicação, normalmente).

O fato de uma empresa exigir que suas programadoras formatem a condição desse jeito não é uma descoberta recente. Na verdade, o estudo da lógica há tempos trabalha com a ideia de **construir sentenças de um determinada maneira** que facilite sobre elas algum processamento. Vamos imaginar que você precisa verificar alguma propriedade de uma fórmula como *a → b*. Você pode transformar essa fórmula para algo como *¬a∨b*, que tem uma sintaxe diferente, usando outros conectivos, mas é semanticamente **equivalente**, certo? Vamos supor agora que seu algoritmo de verificação consegue processar mais rapidamente negações e disjunções, se comparado a implicações (não se preocupe com uma justificativa para isso, por enquanto). Nesse caso, você concorda que sempre vai compensar transformar a fórmula para esse formato antes de verificar?

Pois é isso que se faz na lógica. Transformar uma fórmula qualquer para usar uma estrutura sintática mais *amigável* para verificação é muito comum, e a gente chama esses formatos *amigáveis* de **formas normais** da lógica. Existem várias formas normais bem conhecidas; o formato que aparece na postagem do início desse texto é chamada de Forma Normal Disjuntiva -- em inglês, DNF. Por causa do tempo que temos disponível, estudaremos o conceito de formas normais usando a chamada **Forma Normal Conjuntiva (CNF)**, que é útil para uma algoritmo de verificação de **validade** muito eficiente.












