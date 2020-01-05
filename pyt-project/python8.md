## Comando de Saída em Python

Esse comando (função) permite exibir na tela do usuário mensagens, expressões e/ou valores armazenados em variáveis do programa. 

Forma Geral:

``` 
                   print(mensagem)

```                          

Uma das variações da sintaxe da função é a que permite que várias strings sejam escritas. De forma mais geral a função **print** é
```
                   print(string 1, string 2, …, string n )
```
Assim cada string aparecerá separada por um espaço em branco, como no exemplo a seguir:
<p><b>
print("isso", "é", "teste")</b> #comando no programa do usuário</p>
<p><b>isso é teste</b>          #saída na tela do usuário</p>

Outro Exemplo:
<p><b>
x = int(input('digite: ')) </b> # O usuário digita o número 123</p>
<p><b>print("você digitou: ", x) </b> # será exibida a mensagem juntamente com o número digitado</p>
<p><b>você digitou: 123</b>          #saída na tela do usuário</p>

###Execute o programa (tecla Run) a seguir:
``` python runnable
print("Essa mensagem aparece na primeira linha\nEnquanto essa aparece na segunda") 
x = 10
print("O quadrado do número", x, "é igual a", x**2)
``` 
