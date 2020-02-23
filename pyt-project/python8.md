## Comando de Saída em Python

Esse comando (função) permite exibir na tela do usuário mensagens, expressões e/ou valores armazenados em variáveis do programa. 

Forma Geral:
![excecao](/imagens/print.png)

Execute os exemplos, a seguir:
``` python runnable

# por padrão as strings serão exibidas  com um espaço em branco entre elas
print("isso", "é", "teste") 

# Pular \n linha na mensagem  
print("Essa mensagem aparece na primeira linha\nEnquanto essa aparece na segunda") 

#print com separador _ entre os calores a serem exibidos
print("O quadrado do número", x, "é igual a", x**2, sep='_')

#Usando o end para não pular a linha após o print
print("vou imprimir isso em uma linha ", end=' ')
print("continuarei na linha de cima")
``` 
