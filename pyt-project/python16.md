# Processamento Condicional

### Condicional Múltipla

A estrutura do if simples, bem como a do if com cláusula else testam apenas uma única condição (simples ou composta). Entretanto existem situações em que é necessário testar várias condições onde
apenas uma é verdadeira, e apenas esse bloco será executado. Essa situação pode ser trabalhada com vários comandos if's encadeados onde cada um possui uma condição. 
Há uma variação da estrutura **if** projetada para tratar essas situações, vista a seguir:
```
if condição 1:
   comando 1 se condição 1 for verdadeira
   ...
   Comando n se condição 1 for verdadeira 
elif condição 2:
   comando 1 se condição 2 for verdadeira 
   ...
   comando n se condição 2 for verdadeira 
elif condição 3:
   comando 1 se condição 3 for verdadeira 
   ...
   comando n se condição 3 for verdadeira 
else:
   comando 1 se todas as condições anteriores forem falsas
   ...
   comando n se todas as condições anteriores forem falsas 
primeiro comando depois do if
```
