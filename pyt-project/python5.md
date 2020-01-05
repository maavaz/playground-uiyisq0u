# Variáveis

Para que um programa possa manipular os dados, estes precisam estar armazenados em locais da memória do computador. Esse locais usados para armazenar dados são denominados de variáveis. Portanto,
``` 
Variáveis podem ser definidas como locais de memória que servem para armazenar temporariamente (durante a execução do programa ou seção do terminal) dados(valores) que deverão ser utilizados na execução do programa ou na seção do terminal.
```
Muitas vezes é necessário guardar um dado (p.ex. um número) digitado pelo usuário para ser usado em um cálculo subsequente, gravá-lo em um arquivo ou até enviá-lo pela internet para outro local. Esse
é o objetivo da variável. O nome "Variável" é dado porque a informação guardada pode ser alterada, isto é, pode variar.

Toda variável tem:

+ <b>Um nome</b> - que é como ela será chamada ao guardar e recuperar a informação da memória;
+ <b>Um tipo</b> - esse tipo (inteiro, real etc.) é definido quando variável é criada, baseando-se no conteúdo que foi a ela atribuído; e
+ <b>Uma abrangência (ou escopo)</b> - uma variável só pode ser usada (para armazenar e resgatar dados) no módulo do programa que foi criada.


## Criação da Variável
Uma variável é criada pelo programa python no momento que precisamos armazenar um valor no seu interior. A partir daí, essa variável pode ser usada ao longo do programa.
O nome de uma variável é dado pelo programador e deve seguir as seguintes regras
+ Formado por uma sequência qualquer de caracteres (letras maiusculas/minúsculas ou números);
+ Tem que começar por uma letra ou o caractere sublinhado ( _ );
+ Não pode ter letras acentuadas, nem espaço em branco;
+ Maiúsculas e minúsculas são letras diferentes;
+ Não pode ser uma palavra reservada da linguagem; e
+ Deve ser um nome único, não deve conflitar com nomes de variáveis e funções predefinidas.

## Comando de Atribuição
O comando de atribuição (=) é um comando que possibilita o programados mover valores para dentro das variáveis. Uma variável só pode ser usada depois de criada através de um comando de
atribuição. 
```
    Sintaxe:
              Variavel = valor
              
   Após a execução do comando a variável estará armazenando o valor movido.
```
## EXEMPLOS:
```
In [1]: a = 2       # Guarda o número 2 (número inteiro) na variável chamada a. A partir desse ponto toda vez que se usar a numa expressão, o a será computado como sendo 2. Por exemplo:

In [2]: a + 3      # O número 3 irá ser somado ao número 2 armazenado em a, dando o resultado 5.
Out[2]: 5

In [3]: b = 3.2

In [4]: b - 1.1
Out[4]: 2.1

In [5]: c + 4      # Nesse caso como a variável c não foi criada, não é possível realizar a conta, assim é gerada uma mensagem de erro  avisando que a variável c não está definida. 
---------------------------------------------------------------------------
NameError                Traceback (most recent call last)
<ipython-input-5-8271c808b9af> in <module>()
----> 1 c + 4

NameError: name 'c' is not defined
```
**Obs:** Uma variável criada em uma seção do terminal ou programa será perdida quando a seção ou programa se encerrar. 
Assim caso se inicie uma nova seção ou execute o programa novamente, os valores anteriores não serão reconhecidos.
