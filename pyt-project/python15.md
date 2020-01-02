# Processamento Condicional

### Estrutura Condicional Composta

+ Existem situações onde é necessário agrupar um conjunto de comandos quando a Condição for avaliada **Verdadeira** e outro conjunto de comandos quando a Condição for avaliada **Falsa**
+ Na linguagem python o código equivalente para essa estrutura de decisão é:
```
 if condição:
    comando 1 para condição Verdadeira 
    ....
    comando n para condição Verdadeira
 else:
    comando A para condição Falsa
    ....
    comando Z para a condição Falsa
 comando fora da estrutura if
 ```
 + O **else:** simboliza a negação da condição associada ao ```if```, logo está ligado ao conjunto de comandos que será executado quando a condição for **Falsa**.
 + A Estrutura Condicional Composta representa uma bifurcação,i.e., ou executo os comandos associados a condição Verdadeira **OU** executo os comandos associados a condição Falsa, mas nunca os dois.
![bifurcacao](/imagens/bifurcação.png)
---

+ Exemplo de Programa com estrutura condicional composta: 
    + selecione o botão **Run** para execução do programa;
    + Modifique os valores das variáveis a e b para criar situações diferentes da apresentada;

``` python runnable
a = 25
b = 35;
if a > b:
   print("O valor da soma de a e b é", a+b)
else:
   print ("Valor da diferença é", b - a);

```
#### Condições Compostas
Quando uma estrutura condicional possui mais de uma condição, elas podem ser combinadas pelos operadores lógicas **and (e)**, **or (ou não exclusivo)** e **not (inversão)** para formar uma condição composta. A tabela abaixo lista a forma com que cada operador lógico combina as expressões:
![tabela](/imagens/tabela.png)

Execute o exemplo a seguir que mostra como duas comparações são combinadas
``` python runnable
x = 3.5
y = 1.2
if y < x and x > 3:
    print("As duas condições são verdadeiras")
else:
    print("Pelo menos uma condição ou as duas condições são falsas")
```


