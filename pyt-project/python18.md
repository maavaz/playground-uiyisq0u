# Processamento com Repetição
Em algumas situações, é comum que um comando (ou conjunto deles) precise ser executado várias vezes seguidas.
+ O processamento com repetição permite que um conjunto de comandos possa ser repetidos **n vezes**.
+ Há dois tipos de processamento com repetição: 
    + Processamento com um número pré-determinado de repetições - Representado pela estrutura **for** e, nesse caso, comandos pertencentes a estrutura serão repetidos um número fixo de vezes.
    + Processamento com sinalizador de parada - - Representado pela estrutura **while* e, nesse caso, comandos pertencente a estrutura serão repetidos enquanto uma condição associada for Verdadeira (True). 
+ Estas estruturas de repetição são também conhecidas como laços (do inglês loops).

---
### Processamento com um número pré-determinado de repetições.
---
Esse tipo de processamento é representado pela estrutura do ```for``` que tem o objetivo de repetir um conjunto de comandos um número fixo de vezes. 
Nessa estrutura define-se uma variável de controle da repetição que vai assumindo um valor dentro de um conjunto de valores pré-definidos. Cabe ao programador definir o nome e a lista de valores possíveis para essa variável. A forma geral do comando for é a que segue:
```
for variável in sequência:
 comando 1
 comando 2
 etc.
 comando n
próximo comando
```
A sequência colocada na instrução **for** pode ser uma função (range) e a variável será incrementado ou decrementada a cada ciclo.

O exemplo a seguir exibe o laço **for** onde a variável **item** recebera um número, iniciando em zero, finalizando em 9 e, a cada ciclo (volta), a variável item é incrementada de 1 unidade. Execute o código selecionando a tecla Run.
``` python runnable
for item in range(10):
    print(item)
```

