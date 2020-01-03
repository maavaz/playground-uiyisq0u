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
