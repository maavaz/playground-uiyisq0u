# Processamento com Repetição

---
### Repetição com sinalizador de parada
---
Um comando, ou grupo de comandos pode ser repetido enquanto uma determinada condição definida no cabeçalho for verdadeira. Uma vez que essa condição é falsa, as repetições param. 
A estrutura que representa esse tipo de repetição é a **while**, que possui a seguinte forma geral:
```
while condição de continuidade:
 comando 1
 ...
 Comando n
próximo comando depois do bloco do while
```
A condição de continuidade definida no cabeçalho obrigatoriamente deve ser modificada a cada volta no laço (loop). Se ela for verdadeira todo o bloco de comandos pertencente a estrutura (recuado) será executado. Esse processo se repete até que a condição de continuidade se torne falsa. Assim o próximo comando que não está recuado é executado e a execução do restante do programa continua.
A condição de continuidade é testada toda vez que encontra o **while**, isto significa que se for falsa desde a primeira vez o bloco de comandos nunca será executado. 
O exemplo a seguir é o mesmo apresentado no caso da estrutura for, isto é, um programa que imprime os números de 0 até 9.
``` python runnble
i = 0
while i < 10:
 print(i)
 i += 1
``` 

---
<b>Atenção:</b> Uma das coisas que chama a atenção em Python é o **else**. O seu uso “natural”, para definir um caminho alternativo para um **if**, não tem nada demais. O que é um pouco estranho é o fato de Python aceitar else em expressões de loop como **for e while**. O else não será explicado até o momento que for necessário em algum problema. Mas, é importante informar a você que é possível ter else em estrutura de repetição.
