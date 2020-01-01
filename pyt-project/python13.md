# Saída Formatada
Até agora vimos apenas o comando **print** na sua forma mais simples, mas existem situações que desejamos que os dados sejam apresentados de maneira mais próxima da que estamos acostumados no nosso dia a dia. Por exemplo, os dados do tipo Float sempre são impressos com uma precisão de 14 casas decimais, mas quando estamos exibindo valores monetários, seria interessante que tivessem apenas 2 casas, como formatar essa impressão (print) para que isso ocorra?
Existe uma construção que permite formatar a saída com certa facilidade: é o método format. A forma mais simples de usar essa construção é de marcar a posição onde o conteúdo da variável (ou resultado da expressão) aparecerá, com chaves que envolvem o número que representa a variável que será colocada, por exemplo: 
 ![programa](/imagens/format.png)
 
 No exemplo acima, o método **format** possui três argumentos: **a (cujo índice é zero)**, **b (cujo índice é um)** e **x (cujo índice é dois)**. Dentro da string a marcação **{0}** é substituída pelo valor de **a**, a marcação **{1}** é substituída pelo valor de **b** e a marcação **{2}** é substituída pelo valor de **x**.
 
 Além de mesclar o conteúdo de uma variável, é possível, também, incluir a
especificação da largura que se deseja reservar para um número, assim como o número de
casas decimais que se deseja mostrar. Para especificar a formatação com mais detalhes usamse códigos dentro da marcação dos parêntesis, esses códigos são colocados depois do sinal
de : (dois pontos).
Para números inteiros usa-se o código:
:nd
onde n é o número mínimo de espaços reservados para o número. O número ficará alinhado
com a margem direita do espaço reservado ao número.
Para números reais, pode-se fixar o número de casas decimais a ser mostrado
usando o código
:.nf
onde n é o número de casas decimais para o arredondamento. Para fixar a largura mínima e o
número de casas decimais tem-se:
:m.nf
onde m é o número mínimo de caracteres que o número usará, e n é o número de casas
decimais
