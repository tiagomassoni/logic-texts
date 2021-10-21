# Provando argumentos com árvores

Eita, galera, árvores podem ter muitas utilidades, dentro da mesma ideia de aumentar a eficiência da verificação das fórmulas. Deixa eu começar aqui com mais um uso interessante, verificar se duas ou mais fórmulas são satisfazíveis se consideradas ao mesmo tempo. Como diria Nietzsche, se são satisfazíveis juntas, imagina juntas!

Basta, para isso, usar, como raiz da árvore, duas fórmulas em vez de apenas. As regras são aplicadas da mesma forma, e vamos procurar literais complementares pra verificar. Se chegaremos a um nó-folha (ou caminho) aberto, quer dizer que considerar as duas fórmulas como verdadeiras em conjunto é satisfazível. Veja o exemplo abaixo, onde achamos um caminho aberto para satisfazer, ao mesmo tempo, B e A → B. Isso quer dizer que as duas fórmulas podem ser verdadeiras ao mesmo tempo, com a interpretação A=F e B=T (situação dada pelo próprio caminho).

![provas/t1.png](provas/t1.png)

Em termos gerais, a árvore sempre nos responde um tipo de pergunta: se todas as proposições no topo da árvore podem ser verdadeiras em uma mesma interpretação -- se o conjunto destas proposições é satisfazível. Uma árvore sempre nos responde isso, mas nunca pode nos responder, diretamente, se essas proposições são tautologias; ela é incapaz de responder "esta proposição pode ser falsa?". 

Quero trazer agora o conceito de **argumento** pra todo esse contexto de árvores. Lembra, né, argumento, aquele conjunto de fórmulas com uma conclusão e zero ou mais premissas? Pois é, é um conjunto de fórmulas, não apenas uma. Conseguimos provar se um argumento é válido com a nossa amiga tabela-verdade, através do conceito de vinculação semântica (todas as premissas sendo verdadeiras em uma interpretação obriga a conclusão a ser verdadeira, sem isso o argumento é inválido). Será que a árvore pode nos ser útil na hora de provar argumentos, nos salvando da ineficiência da tabela-verdade?

Gente, pior que sim. 