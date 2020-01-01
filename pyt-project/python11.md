# Processamento Sequencial
---
 #### Exercício 3 
---

<p>Faça um Programa que peça 2 números inteiros e um número real. Calcule e mostre:
a) o produto do dobro do primeiro com metade do segundo .
b) a soma do triplo do primeiro com o terceiro.
c) o terceiro elevado ao cubo.</p> 
---

@[Programacao Python]({"stubs": ["./www/terminal2"],"command": "sh /project/target/www/terminal4.sh" })

::: Solução
``` python
raio = float(input("digite o raio do círculo:"))
area = 3.1415 * raio**2
print("O circulo de raio",raio, " tem area igual a", area)
```
:::

---
 #### Exercício 4 
---
Faça um programa que pergunte quanto alguém ganha no mês de salário bruto. Calcule e mostre o total do seu salário líquido no referido mês, sabendo-se que são descontados 11% para o Imposto de Renda, 8% para o INSS e 5% para o sindicato. A saída do programa deve escrever o seguinte texto:
+ Salário Bruto: R$ valor
- IR (11%): R$ valor
- INSS (8%): R$ valor
- Sindicato ( 5%): R$ valor
= Salário Liquido: R$ valor
Obs.: Salário Bruto - Descontos = Salário Líquido. 


@[Programacao Python]({"stubs": ["./www/terminal2"],"command": "sh /project/target/www/terminal5.sh" })

::: Solução
``` python
farenheit = float(input("Digite uma temperatura em graus farenheit:"))
celsius = 5 * (farenheit - 32)/9
print("A temperatura", farenheit, "ºF corresponde a", celsius,"ºC")
```
:::
