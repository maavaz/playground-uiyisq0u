# Processamento Sequencial
---
 #### Exercício 3 
---

<p>Faça um Programa que peça dois números inteiros e um número real. Calcule e mostre:</p>
<p>a) o produto do dobro do primeiro com metade do segundo.</p>   
<p>b) a soma do triplo do primeiro com o terceiro.</p>                                                                     
<p>c) o terceiro elevado ao cubo. </p>


@[Programacao Python]({"stubs": ["./www/terminal2"],"command": "sh /project/target/www/terminal4.sh" })

::: Solução
``` python
numint1 = int(input("digite um número inteiro:"))
numint2 = int(input("digite outro número inteiro:"))
numfloat = float(input("digite um número real:"))

produto = (2*numint1) * (numint2/2)
soma = (3*numint1) + numfloat
cubo = numfloat ** 3

print("produto=",produto)
print("soma=",soma)
print("cubo=",cubo)
```
:::

---
 #### Exercício 4 
---
Faça um programa que leia o salário bruto de uma pessoa em um determinado mês. Calcule e mostre o seu salário líquido no referido mês, sabendo-se que são descontados 11% para o Imposto de Renda, 8% para o INSS e 5% para o sindicato. A saída do programa deve escrever o seguinte texto:
```
(+) Salário Bruto: R$ valor
(-) IR (11%): R$ valor
(-) INSS (8%): R$ valor
(-) Sindicato ( 5%): R$ valor
(-) Total Desconto : R$ valor
(=) Salário Liquido: R$ valor
```
Obs.: Salário Bruto - Descontos = Salário Líquido. 


@[Programacao Python]({"stubs": ["./www/terminal2"],"command": "sh /project/target/www/terminal5.sh" })

::: Solução
``` python
sbruto = float(input("digite o seu salario bruto:"))
inss = 0.08 * sbruto
ir = 0.11 * sbruto
sindi = 0.05 * sbruto
totdesc = ir + inss + sindi
sliq = sbruto - totdesc
print("(+) Salário Bruto:   R$",sbruto)
print("(-) IR (11%):        R$",ir)
print("(-) INSS (8%):       R$",inss)
print("(-) Sindicato ( 5%): R$",sindi)
print("(-) Total Desconto : R$",totdesc)
print("(=) Salário Liquido: R$",sliq)
```
:::
