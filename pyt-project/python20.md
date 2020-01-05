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
                              |     i +=1 
                              |     print(i)                                             
```
?[O que será exibido na execução dos trechos acima:]
-[x] O trecho A exibirá os números de 5 até 9 e o trecho B exibirá os números de 5 até 10.
-[ ] O trecho A exibirá os números de 5 até 10 e o trecho B exibirá os números de 5 até 10.
-[ ] O trecho A exibirá os números de 5 até 9 e o trecho B exibirá os números de 5 até 9.
-[ ] O trecho A exibirá os números de 5 até 9 e o trecho B exibirá os números de 4 até 9.

Considere o código abaixo, digitado em Python.
```
a = 0
b = 1
while b < 10:
  a = b
  b = a + b
```    
?[No final da execução do código, o último valor armazenado nas variáveis a e b serão, respectivamente,]
-[ ] 4 e 16.
-[ ] 8 e 8.
-[ ] 8 e 16.
-[x] 4 e 8.


###### Exercício 1  
----
Faça um programa que imprima os números pares de 100 até 200, incluindo-os.

@[Programacao Python]({"stubs": ["./www/terminal2"],"command": " sh /project/target/www/terminal10.sh" })
 
::: Solução

``` python
num = 100
while num <= 200:
   if num % 2 == 0:  # verifica se o número é par,i.e., resto da divisão (%) do número por dois é igual a zero 
      print(num)
   num = num + 1  # gera o próximo número
```
:::
---
###### Exercício 2  
----
Uma Empresa oferece para os 10 primeiros clientes um determinado desconto de acordo com o valor da compra efetuada. O desconto é de 20% se o valor da compra for maior ou igual a 1.500,00 Reais, e 15% se for menor. Fazer um programa que leia de cada cliente o valor da compra e o nome do cliente, calcule o desconto e exiba o nome do cliente, valor da compra, o desconto e o valor a ser pago. Ao final, exibir total de descontos dado aos 10 clientes. 

@[Programacao Python]({"stubs": ["./www/terminal2"],"command": "sh /project/target/www/terminal11.sh" })

::: Solução

``` python
totdesconto = 0.0
for i in range(10):
    nome = input("Digite seu nome:")
    compra = float(input("Digite o valor da compra:"))
    if compra >= 1500:
        desconto = compra * 0.2
    else:
        desconto = compra * 0.15
    print("Nome    :", nome)
    print("Compra  : R${0:.2f}".format(compra))    
    print("Desconto: R${0:.2f}".format(desconto))
    print("Pagar   : R${0:.2f}".format(compra - desconto))
    totdesconto = totdesconto + desconto #forma reduzida: totdesconto+= desconto
print("total descontos: R${0:.2f}".format(totdesconto))   
```
:::

---
###### Exercício 3  
----
Faça um programa que leia a idade de várias pessoas de uma cidade, calcule e imprima média das idades e a quantidade de pessoas por faixa etária. O programa termina quando a idade digitada for igual -1. As faixas etárias consideradas, são: Menor 12 anos, De 12 até 18 e Acima de 18 anos.
 
 @[Programacao Python]({"stubs": ["./www/terminal2"],"command": "sh /project/target/www/terminal8.sh" })
 
::: Solução

``` python
continf = 0       #contador da faixa de menor que 12 anos
somainf = 0       # acumulador das idades da faixa menor que 12 anos
contadol = 0      #contador da faixa de 12 - 18 anos
somadol = 0       # acumulador das idades da faixa de 12-18 anos
contadul = 0      #contador da faixa acima de 18 anos
somadul = 0       # acumulador das idades da faixa acima de 18 anos
idade = int(input('Digite sua idade:'))
while idade != -1:
    if idade < 12:
        somainf += idade
        continf += 1
    elif idade <= 18:
        somadol += idade
        contadol += 1
    else:
        somadul += idade
        contadul += 1
    idade = int(input('Digite sua idade:')) #Leitura dentro do while
print('Média das idade das crianças (<12 anos):{0:.2f}'.format(somainf/continf))
print('Quantidade de Crianças pesquisadas(<12 anos):',continf)    
print('Média das idade do adolescentes (12-18 anos):{0:.2f}'.format(somadol/contadol))
print('Quantidade de adolescentes pesquisados(12-18 anos):',contadol) 
print('Média das idade dos adultos (>18 anos):{0:.2f}'.format(somadul/contadul))
print('Quantidade de adultos pesquisados(>18 anos):',contadul) 

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
