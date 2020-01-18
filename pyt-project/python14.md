# Processamento Condicional

O processamento condicional introduz um elemento importante na programação que é a habilidade do computador fazer coisas diferentes dependendo de determinadas condições. Nesse sentido, o processamento Condicional introduz a estrutura de decisão **if** que é uma declaração que instrui o computador a executar um bloco de comandos apenas se uma dada condição associada ao **if** é verdadeira. 
A forma geral do comando **if** é: 
```
                               if condição: 
                                  comando 1 
                                  comando 2
                                  ...
                                  comando n 
                               comando não pertencente ao if                                                                  
```
+ A execução desse conjunto de comandos associados ao **if** dependerá da avaliação (verdadeira ou Falsa) da(s) condição(ões) associada(s).
+ **Atenção:** É importante que os comandos associados a estrutura **if** iniciem sempre na mesma coluna (caso contrário o interpretador irá emitir um erro). 
+ Necessariamente esses comandos devem estar recuados à direita em relação a estrutura para demonstrar pertencimento. 
+ A(s) condição(ões) é(são) representada(s) através de expressões relacionais. 
+ As expressões relacionais permitem a comparação de valores de mesmo tipo, cujo resultado é um valor do tipo Verdadeiro (True) ou Falso (False). 

**Operadores Relacionais:**
São operadores que possibilitam a comparação entre os dois operandos. Os dois operandos, obrigatoriamente, devem ser do mesmo tipo e o resultado da expressão é um valor booleano(True ou False).

 ![programa](/imagens/operadoresrelacionais.png)

**Exemplo de Expressões relacionais**
``` python
In [1]: 2 == 3
Out[1]: False

In [2]: 3 >= 2
Out[2]: True

In [3]: 5 != 6
Out[3]: True
```

-------
**Testando os conhecimentos....**

?[Sabendo que x = 8, y = -3 e z = 4, quais expressões abaixo tem como resultado o valor Verdadeiro(True)?](multiple)
-[x] x > y	
-[x] x / z == z / 2 
-[ ] y >= 0
-[x] z * 2 == x
-[ ] x / y - 1 == 0
-[ ] y == 3
-[ ] x + y >= x - y 

---
+ Exemplo de Programa com estrutura condicional simples: 
    + selecione o botão **Run** para execução do programa;
    + Modifique os valores das variáveis a e a para criar situações diferentes da apresentada;
    
``` python runnable
a = 4;
b = 6;
soma = a + b;

if soma > 0:
 print("valor da soma é",soma)
 
