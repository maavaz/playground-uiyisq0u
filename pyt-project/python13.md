# Saída Formatada
Até agora vimos apenas o comando **print** na sua forma mais simples, mas existem situações que desejamos que os dados sejam apresentados de maneira mais próxima da que estamos acostumados no nosso dia a dia. Por exemplo, os dados do tipo Float sempre são impressos com uma precisão de 14 casas decimais, mas quando estamos exibindo valores monetários, seria interessante que tivessem apenas 2 casas, como formatar essa impressão (print) para que isso ocorra?
Existe uma construção que permite formatar a saída com certa facilidade: é o método format. A forma mais simples de usar essa construção é de marcar a posição onde o conteúdo da variável (ou resultado da expressão) aparecerá, com chaves que envolvem o número que representa a variável que será colocada, por exemplo: 
 ![programa](/imagens/format.png)
 
 No exemplo acima, o método **format** possui três argumentos: **a (cujo índice é zero)**, **b (cujo índice é um)** e **x (cujo índice é dois)**. Dentro da string a marcação **{0}** é substituída pelo valor de **a**, a marcação **{1}** é substituída pelo valor de **b** e a marcação **{2}** é substituída pelo valor de **x**.
 
 Além da formatação posicional das variáveis, é possível, também, incluir a especificação da largura que se deseja reservar para um número, assim como o número de casas decimais que serão exibidos. Para efetuar a formatação, são utilizados códigos dentro da marcação dos parêntesis e seguidos de : (dois pontos).
 
 
 Para os números inteiros usa-se o código:
 
                     :nd, onde n é o número mínimo de espaços reservados para o número.
    
O número ficará alinhado com a margem direita do espaço reservado ao número. veja o exemplo abaixo:

 ![programa](/imagens/format2.png)


Para os números reais (float), pode-se fixar o número de casas decimais que será exibido usando o código:

                    :.nf , onde n é o número de casas decimais para o arredondamento.  
                    
 ![programa](/imagens/format1.png)
