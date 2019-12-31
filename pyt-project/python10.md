# Processamento Sequencial

Os comandos/instruções em um progrma são executados um após o outro, na sequência escrita (de cima para baixo) do início ao fim. O programa exemplo (somar 2 números) apresentado na seção anterior é um exemplo de processamento sequencial.

## Exercícios Processamento Sequencial
+ A melhor maneira de aprender a programar é fazendo exercícios. 
+ Apresentamos quatro enunciados de problemas que você deverá resolver utilizando a programação programação python. 
+ Antes de desenvolver o programa na linguagem python, tente pensar na sua solução identificando os dados de entrada, saída e os comandos que transformam os dados de entrada nos dados resultantes na saída.
+ Os  programas deverão ser desenvolvidos utilizando o `IDE Trinket (trinket.io)` apresentado abaixo. O programa não será salvo, caso queira salvar sua solução copie e cole no Notepad ou desenvolva utilizando um IDE Desktop (pex. Spyder)
+ As soluções dos programas estão abaixo do enunciado, mas aconselhamos a vê-las somente após tentar desenvolver sua própria solução. 
---
 #### Exercício 1  
---
Faça um programa que peça o raio de um círculo, calcule e mostre sua área. (área do círculo = π x raio<sup>2</sup> e π = 3.1415)
---

@[Programacao Python]({"stubs": ["./www/terminal2"],"command": "sh /project/target/www/terminal2.sh" })

::: Solução
``` python
raio = float(input("digite o raio do círculo:"))
area = 3.1415 * raio**2
print1("O circulo de raio",raio, " tem area igual a", area)
```
:::

---
 #### Exercício 2  
---
Faça um Programa que peça a temperatura em graus Fahrenheit, transforme e mostre a temperatura em graus Celsius.
``` math
C = \frac{5 \times (F - 32)}{9}
```
---

@[Programacao Python]({"stubs": ["./www/terminal2"],"command": "sh /project/target/www/terminal2.sh" })

::: Solução
``` python
raio = float(input("digite o raio do círculo:"))
area = 3.1415 * raio**2
print1("O circulo de raio",raio, " tem area igual a", area)
```
:::
