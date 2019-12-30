# Comandos de Entrada e Saída em Python

Os comandos de entrada e saída de um programa escrito em uma linguagem qualquer possuem a função de comunicação com o mundo exterior, isto é,
o comando de entrada permite que o usuário envie dados para a(s) variável(eis) do programa e o comando de saída permmite exibir o(s) valor(es) armazenados
na(s) variável(eis) do programa.

## Comando de Entrada em Python

Esse comando permite receber o valor digitado no teclado pelo usuário e atribuir esse valor a(s) variável(eis) associadas ao comando.
            Comando (função) de entrada do python: **input** 

Este comando interrompe a execução do programa e espera que o usuário digite alguma coisa e depois pressione a tecla "enter".

Sintaxe:       
                **variável = input('Mensagem para o usuário')**
                
Exemplo:
            <p>**nome = input('Digite o seu Nome')**</p>
            
**Obs:** O input irá esperar a digitação do valor e, após apertar a tecla "enter", o valor será movido para a variavel nome.                                                 
 O comando **input** irá mover um valor do tipo String para variável, independente do que foi digitado, mas caso o usuário queira um valor númerico deverá ser explicitado no comando, conforme exemplos, a seguir:
+ Para solicitar um número inteiro:
                  <p>**nome da variável = int(input('Texto a ser mostrado '))**</p>
Note a composição da função input com a função int. Isso garante que o resultado final armazenado na variável seja um número inteiro descartando qualquer casa decimal que porventura seja digitada.

+ Para solicitar um número real:
                 <p>**nome da variável = float(input('Texto a ser mostrado '))**</p>
Note a composição da função input com a função float. Isso garante que o resultado final que será armazenado na variável seja um número real, acrescentando zeros nas casas decimais caso o usuário não tenha digitado nenhuma casa decimal.                 
