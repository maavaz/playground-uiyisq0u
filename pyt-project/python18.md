# Processamento com Repetição
Em algumas situações, é comum que um comando (ou conjunto deles) precise ser executado várias vezes seguidas.
+ O processamento com repetição permite que um conjunto de comandos possa ser repetidos **n vezes**.
+ Há dois tipos de processamento com repetição: 
    + Processamento com um número pré-determinado de repetições - Representado pela estrutura **for** e, nesse caso, comandos pertencentes a estrutura serão repetidos um número fixo de vezes.
    + Processamento com sinalizador de parada - - Representado pela estrutura **while** e, nesse caso, comandos pertencente a estrutura serão repetidos enquanto uma condição associada for Verdadeira (True). 
+ Estas estruturas de repetição são também conhecidas como laços (do inglês loops).

---
### Processamento com um número pré-determinado de repetições.
---
Esse tipo de processamento é representado pela estrutura do ```for``` que tem o objetivo de repetir um conjunto de comandos um número fixo de vezes. 
Nessa estrutura define-se uma variável de controle da repetição que vai assumindo um valor dentro de um conjunto de valores pré-definidos. Cabe ao programador definir o nome e a lista de valores possíveis para essa variável. A forma geral do comando for é a que segue:
```
for variável in sequência:
 comando 1
 comando 2
 etc.
 comando n
próximo comando
```
A sequência colocada na instrução **for** pode ser uma função (range) e a variável será incrementado ou decrementada a cada ciclo.

O exemplo a seguir exibe o laço **for** onde a variável **item** recebera um número, iniciando em zero, finalizando em 9 e, a cada ciclo (volta), a variável item é incrementada de 1 unidade. Execute o código selecionando a tecla Run.
``` python runnable
for item in range(10):
    print(item)
```
---
Outro Exemplo:
---
Faça um programa que leia 2 notas de cada aluno de uma turma de 10 alunos, calcular e exibir a média das notas de cada aluno. Ao final, calcular e exibir a média da turma.
<p></p>

<b>Comentários para a solução:</b> 

+ O modo de pensar a solução segue o padrão já ensinado: Entrada + Processamento + Saída.
   + Entrada: ler nota1 e nota2
   + Processamento: media = (nota1 + nota2)/2
   + saida: Exibir a média
+ O problema diz que a turma tem 10 alunos, se precisamos efetuar o mesmo processamento para cada aluno, a solução acima precisa estar dentro de uma estrutura de repetição **for** que efetuará a repetição dos comandos 10 vezes.
+ O problema irá calcular e exibir a média da turma, logo precisaremos acumular as médias durante a repetição. Para isso, usaremos uma variável para acumular as médias, cujo comando a seguir será inserido após o cálculo da média do aluno, dentro do **for**: totmedia = totmedia + media.
+ Ao final, fora do **for**, calcular e exibir a média final.
+ Tente escrever a sua solução.
::: Solução
totmedia = 0     toda variável acumuladora precisa ser zerada no início do programa
for i in range(10): # Estrutura que repetirá 10 vezes
   nota1 = float(input('Digite a primeira Nota:'))
   nota2 = float(input('Digite a segunda Nota:'))
   media = (nota1 + nota2)/2
   print("A média do aluno é:{0:.2f}".format(media))
   totmedia = totmedia + media
mediager = totmedia/10
print("A média da turma é:{0:.2f}".format(mediager))
:::

**OBS:** Outras variações da Estrutura **for** serão apresentadas no decorrer desse e do tutorial Programação Python.
