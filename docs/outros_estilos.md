# Outros Métodos de Prova em Lógica

Para o caso da lógica proposicional, vimos dois métodos de prova de propriedades de fórmulas (validade e satisfazibilidade) e argumentos (validade): tabela-verdade e árvores. Para a lógica de predicados, perdemos o poder de usar tabelas-verdade, por estarmos lidando com infinitos modelos em potencial, mas ainda mantemos a possibilidade de utilizar árvores, com novas regras de desenvolvimento.

Na verdade, vários outros métodos de prova foram desenvolvidos ao longo de história, que funcionam para ambas as lógicas. Neste módulo, faremos um breve passeio por alguns deles, entendendo seus pontos fortes e suas limitações.

Antes de começar, deixa eu revisitar o que devemos entender como **prova formal**. 
Na lógica, primeiro precisa existir um conjunto específico de símbolos a partir dos quais construímos uma prova — os símbolos de uma linguagem lógica, como as duas que vimos na disciplina, junto com alguns símbolos adicionais para organizar a prova.
Qualquer sequência desses símbolos pode ser então uma candidata a receber o título de *prova*; pode ainda não ser, dependendo de uma verificação. 
Segundo, deve haver um *procedimento de decisão* para determinar, dentro de um tempo finito,  se uma sequência candidata a prova é realmente uma prova — algum tipo de algoritmo que recebe a prova candidata como entrada e retorna *sim* ou *não*.  O procedimento deve então ser preciso, para que não haja dúvida sobre a resposta.
Desta forma, as provas precisam também ser *finitas*, algo que é intuitivamente correto: nenhum algoritmo pode ser finito verificando algo infinito.

Vamos verificar, como exemplo, o método de prova com árvores (Tableaux). A sequência de símbolos é a lógica de predicados, adicionada de símbolos gráficos, como traços e números, que ajudam a *desenhar* a prova. Como estamos sempre lidando com fórmulas com um número finito de predicados, quantificadores e conectivos, o número de nós da árvore nunca será infinito, consequentemente a árvore terá um número finito de caminhos. Assumindo isso, temos um procedimento de decisão preciso que sempre termina, pois verifica se, para cada caminho, o mesmo está aberto ou fechado. Desta forma, podemos classificar a árvore do Tableaux como um método de prova formal para *satisfazibilidade* da lógica de predicados.

Os quatro métodos (também chamados de estilos) de prova formal são tableaux (o método da árvore é só um dos tipos de tableaux), axiomático, dedução natural e cálculo de sequents (muito usado em ferramentas provadoras de teoremas). Vamos dar uma olha nos métodos **axiomático** e **dedução**.


## Sistemas Axiomáticos


## Dedução Natural

