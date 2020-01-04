# Exercitando (Repetição)

Observe o trecho do programa abaixo.
``` 
  x = int(input('digite um valor inteiro'))
  while x != -1:
    print(x)
```
---
?[Supondo que o usuário tenha digitado no comando input o valor 10 (dez). Selecione a resposta que descreve o resultado da execução do trecho de código acima:]
-[ ] irá exibir o valor 10 tantas vezes quanto o usuário desejar até digitar -1 (valor de parada).
-[ ] irá exibir a letra 'x' tantas vezes quanto o usuário desejar até digitar -1 (valor de parada).
-[x] irá exibir o valor 10 (valor de parada) fornecida pelo usuário infinitamente porque o programa não irá parar.
-[ ] irá exibir apenas o valor -1 ao final da execução.

Dado os trechos de códigos abaixo:
```
     trecho A                       trecho B
for i in range(5, 10):        |   i = 4
   print(i)                   |   while i < 10:
                                    i +=1 
                                    print(i)                                             
```
?[O que será exibido na execução dos trechos acima:]
-[x] O trecho A exibirá os números de 5 até 9 e o trecho B exibirá os números de 5 até 10.
-[ ] O trecho A exibirá os números de 5 até 10 e o trecho B exibirá os números de 5 até 10.
-[ ] O trecho A exibirá os números de 5 até 9 e o trecho B exibirá os números de 5 até 9.
-[ ] O trecho A exibirá os números de 5 até 9 e o trecho B exibirá os números de 4 até 9.

###### Exercício 1  
----
Escreva um programa que leia a idade de uma pessoa e, se a idade digitada for 21 ou mais anos, imprima a idade juntamente com a mensagem "Você já é maior de 21 anos".
@[Programacao Python]({"stubs": ["./www/terminal2"],"command": " /project/target/www/terminal6.sh" })
 
::: Solução

``` python
idade = int(input("Digite a sua Idade:"))
if idade >= 21:
 print("Voce já e maior de 21 anos")
```
:::
---
###### Exercício 2  
----
As maçãs custam R$ 1,40 cada se forem compradas menos do que uma dúzia e, R$ 1,25 cada, se forem compradas pelo menos uma dúzia. Escreva um programa que leia o número de maçãs compradas, calcule e escreva o valor total da compra.  

@[Programacao Python]({"stubs": ["./www/terminal2"],"command": "sh /project/target/www/terminal7.sh" })

::: Solução

``` python

qtd = int(input("Digite a quantidade de maçãs compradas :"))
if qtd >= 12:
   compra= qtd * 1.25
else:
   compra= qtd * 1.4
print("o valor de sua compra é:", compra)

```
:::

---
###### Exercício 3  
----
A escola “APRENDER” faz o pagamento de seus professores por hora/aula mais 15% do salário referente ao Descanso Semanal Remunerado (DSR). Faça um programa que leia o nível do professor (1 ou 2) e a quantidade de horas de aula dadas no Mês, calcule e exiba o salário de um professor. Sabe-se que o valor da hora/aula segue a tabela abaixo: 
+ Professor Nível 1 R$56,00 por hora/aula 
+ Professor Nível 2 R$66,00 por hora/aula 
Obs: Exiba o salário formatado com 2 casas decimais.
 @[Programacao Python]({"stubs": ["./www/terminal2"],"command": "sh /project/target/www/terminal8.sh" })
 
::: Solução

``` python
horas= int(input("Digite a quantidade de horas trabalhadas :"))
nivel = int(input("Digite o nivel do professor(1 ou 2): "))
if nivel == 1:
   salario= horas * 56.00
else:
   salario= horas * 66.00
dsr = salario *  0.15;
salario = salario + dsr;
print("o salario do professor é:{0:.2f}".format(salario))

```
:::
----
----
Desafio
----
Faça um programa que calcule o desconto de uma compra feita em uma loja. O programa deve ler o valor das compras e calcular o valor do desconto obedecendo os seguintes percentuais: 
+ 10% de desconto se a compra for menor ou igual que R$2.000,00; 
+ 5% de desconto se a compra for maior que R$ 2.000,00 e menor ou igual a R$ 3.000,00;
+ 3% de desconto se for maior que R$ 3.000,00 e menor ou igual a R$ 5.000,00;
+ 2% de desconto para compras acima de R$ 5.000,00.
O programa deverá exibir o valor da compra, o valor do desconto e o total a pagar. Formatar as saídas para 2 casas decimais.
@[Programacao Python]({"stubs": ["./www/terminal2"],"command": "sh /project/target/www/terminal9.sh" })

::: Solução
```python
 
compras= float(input("Digite o valor de suas compras:"))

if compras <= 2000:
     taxa=0.1
elif compras <= 3000: # Nessa condição não é necessário por a condição de maior que 2000, pois nesse if já é maior que 2000*/
     taxa = 0.05     
elif compras <= 5000: # Nessa condição não é necessário por a condição de maior que 3000, pois nesse if já é maior que 3000*/
     taxa = 0.03    
else:
      taxa=0.02      # Nessa condição não é necessário por a condição de maior que 2000, pois nesse if já é maior que 2000*/        
desconto = compras * taxa
totpagar = compras - desconto
print("Compras : R$ {0:.2f}".format(compras))
print("Desconto: R$ {0:.2f}".format(desconto))
print("Total   : R$ {0:.2f}".format(totpagar))

```
:::
