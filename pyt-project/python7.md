# Comandos de Entrada e Saída em Python

Os **comandos de entrada e saída** de um programa disponíveis nas linguagens de programação possuem a função de comunicação com o mundo exterior, isto é,
o **comando de entrada** permite que o usuário envie dados do mundo exterior (p.ex. teclado) para uma variável do programa (variável associada ao comando) e o **comando de saída** permite exibir (p. ex. na tela do computador) mensagens, expressões e/ou  valores armazenados em variáveis do programa.

## Comando de Entrada em Python

Esse comando permite receber o valor digitado no teclado pelo usuário e atribuir esse valor a variável associadas ao comando.
            Comando (função) de entrada do python: **input** 

Este comando interrompe a execução do programa para esperar que o usuário digite o valor solicitado no teclado e, ao final da digitação, pressione a tecla "Enter". Após isso, o valor digitado será movido para  variável associada ao **input**.

Sintaxe:       
                **variável = input('Mensagem para o usuário')**
                
Exemplo:
            <p>**nome = input('Digite o seu Nome')**</p>
                                               
 Por padrão, o comando **input** move valores do tipo String para as variáveis associadas ao comando. Mas, caso o usuário queira que um valor númerico seja movido para a variável, deverá ser explicitado no comando, conforme exemplos, a seguir:
+ Para solicitar um número inteiro:
                  <p>**nome da variável = int(input('Texto a ser mostrado '))**</p>
Note a composição da **função input** com a **função int**. Isso garante que o resultado final armazenado na variável seja um número inteiro descartando qualquer casa decimal que porventura seja digitada.

+ Para solicitar um número real:
                 <p>**nome da variável = float(input('Texto a ser mostrado '))**</p>
Note a composição da **função input** com a **função float**. Isso garante que o resultado final que será armazenado na variável seja um número real, acrescentando zeros nas casas decimais caso o usuário não tenha digitado nenhuma casa decimal.                 
