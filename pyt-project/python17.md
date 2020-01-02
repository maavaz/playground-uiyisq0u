# Exercitando (Condicional)

Observe o trecho do programa abaixo.
``` 
 if x >= y:
  w = 0;
 else  
  w = 1;
```
---
?[Que valores de X e Y devem ter para que a execução do trecho de código acima faz com que a variável W armazene o valor 0 (zero):]
-[ ] x = 2 e y= 3.
-[ ] x = 1 e y= 2.
-[x] x = 1 e y= 1.
-[ ] Em nenhuma das respostas acima a variável w conterá o valor 0.

Dado o trecho de código abaixo:
```
print ("A");
if q1:
 print ("B")
else:
 print ("C")
print ("D");
if q2:
 print("E");
else:
 print ("F")
print ("G")
print ("H")
```

?[Que sequência será impressa pelo programa, caso as condições q1 e q2 sejam verdadeiras:] (single)
-[x] A B D E G H.
-[ ] A C D F G H.
-[ ] A B D F G H.
-[ ] A C D E G H.

###### Exercício 1  
----
Escreva um programa C que peça a idade de uma pessoa e, se a idade digitada for 21 ou mais anos, imprima a idade juntamente com a mensagem "Você já é maior de 21 anos".

 
::: Solução

``` C
#include<stdio.h>
int main(){
int idade;

printf("Digite a sua Idade:");
scanf("%d", &idade);

if (idade >= 21){
 printf("Voce já e maior de 21 anos");
}
}
```
:::
---
###### Exercício 2  
----
As maçãs custam R$ 0,30 cada se forem compradas menos do que uma dúzia e, R$0,25 cada, se forem compradas pelo menos uma dúzia. Escreva um programa que leia o número de maçãs compradas, calcule e escreva o valor total da compra.



::: Solução

``` C
#include<stdio.h>
int main(){
int qtd;
float compra;
printf("Digite a quantidade de maçãs compradas :");
scanf("%d", &qtd);

if (qtd >= 12){
   compra= qtd * 0.25;
}
else {
   compra= qtd * 0.3;
}
printf("o valor de sua compra é: %f", compra);
}

```
:::

---
###### Exercício 3  
----
A escola “APRENDER” faz o pagamento de seus professores por hora/aula mais 15% do salário referente ao Descanso Semanal Remunerado (DSR). Faça um programa C que leia o nível do professor (1 ou 2) e a quantidade de horas dadas no Mês, calcule e exiba o salário de um professor. Sabe-se que o valor da hora/aula segue a tabela abaixo: 
+ Professor Nível 1 R$56,00 por hora/aula 
+ Professor Nível 2 R$66,00 por hora/aula 

 
::: Solução

``` C
#include<stdio.h>
int main(){
int nivel;
int horas;
float salario;
float dsr;
printf("Digite a quantidade de horas trabalhadas :");
scanf("%d", &horas);
printf("Digite o nivel do professor(1 ou 2): ");
scanf("%d", &nivel);
if (nivel == 1){
   salario= horas * 56;
}
else {
   salario= horas * 66;
}
dsr = salario *  0.15;
salario = salario + dsr;
printf("o salario do professor é: %f", salario);
}

```
:::
----
