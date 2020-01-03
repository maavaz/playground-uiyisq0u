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
``` python runnable
item = 0
while item < 10:
 print(item)
 item += 1
``` 
Notem que, na estrutura **for**, a inicialização e o incremento da variável **item** são efetuadas automaticamente pela estrutura. Na estrutura **while** isso tem que ser feito pelo programador. Por isso, nesse tipo de problema (processamento com um número pré-determinado de repetições é melhor implementado com a estrutura **for**).
O comando **item += 1** significa **item = item + 1** (instrução de incremento de 1 unidade).

---
Outro tipo de Exemplo:
---
Faça um programa para calcula o valor da tarifa do pacote de serviços das contas dos clientes de um Banco. O programa deverá ler o número da conta e o saldo do cliente. Para contas com saldo de pelo menos 10.000,00 reais o valor do pacote de serviços é igual a 0,1%, do contrário é igual 0,3%. Para cada conta, calcule e exiba o valor da taxa de serviços e o novo saldo. O programa termina quando o número da conta é igual a -1
<p></p>

<b>Comentários para a solução:</b>
+ O modo de pensar a solução segue o padrão já ensinado: Entrada + Processamento + Saída.
   + Entrada: ler numero da conta e saldo
   + Processamento: verificar o saldo do cliente para selecionar o percentual; calcular o valor do serviço baseado no percentual selecionado
   + saida: Exibir o valor da taxa e o novo saldo (descontado do valor da taxa).
+ Diferentemente do problema anterior, nesse caso não sabemos quantas vezes a estrutura while irá executar, pois o processamento só irá parar quando for lido o valor -1 para o número da conta.
+ Logo, quem controla a quantidade de laços(repetições) é o usuário. Além disso, como dito anteriormente, a estrutura testa a condição de continuidade (nesse caso, número da conta) toda vez que o processamento encontra o **while**.
+ Portanto, em todos os casos de processamento semelhante a esse, obrigatoriamento, o programador deverá colocar um comando de leitura (somente aquele com a variável da condição de contitnuidade) antes do while e repeti-lo no final da estrutura, como mostrado no modelo a seguir:
```
  variável = input(´mensagem qualquer´)  # comando de Leitura da variável da condição de continuidade
  while variável != valor de parada:   #representar a variável com o operador != seguido do valor de parada
     comando1
     ...
     comando n
     variável = input(´mensagem qualquer´)  # repetir o comando de Leitura da variável da condição de continuidade
```
+ Tente resolver o problema.
::: Solução
conta = int(input("Digite o número da conta:")) #esse comando deverá ser repetido no fim do while.
while (conta != -1):
   saldo = float(input("Digite o saldo da conta: "))
   if (saldo >= 10000):
     vtaxa = saldo * 0.001;
   else:
     vtaxa = saldo * 0.002;
    
   nsaldo = saldo - vtaxa
   print("saldo atual = {0:.2f}".format (nsaldo))
   print("valor Servicos = {0:.2f}".format(vtaxa)) 
   conta = int(input("Digite o número da conta:"))
:::   
 
<b>Atenção:</b> Uma das coisas que chama a atenção em Python é o **else**. O seu uso “natural”, para definir um caminho alternativo para um **if**, não tem nada demais. O que é um pouco estranho é o fato de Python aceitar else em expressões de loop como **for e while**. O else não será explicado até o momento que for necessário em algum problema. Mas, é importante informar a você que é possível ter else em estrutura de repetição.
