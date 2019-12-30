# Erros de Sintaxe
Caso o interpretador do Python não compreenda um determinado comando escrito pelo usuário é gerado um **erro de sintaxe**.
A forma geral de uma mensagem de erro é:
              Traceback (most recent call last):
              File "nome do arquivo", número da linha, in nome do módulo
              Nome do erro: detalhes do erro.
A última linha da mensagem fornece o nome e os detalhes do erro. A seguir são apresentados dois exemplos de erros: 
No primeiro digita-se o comando print de forma errada (pront), como ele não existe gera-se um NameError e aparece a mensagem “NameError: name 'pront' is not defined”.

```
>>> pront("exemplo de erro de sintaxe") # comando escrito de forma incorreta 

Traceback (most recent call last)
<ipython-input-17-eec38deceaeb> in <module>()
----> 1 pront("exemplo de erro de sintaxe")
NameError: name 'pront' is not defined
```
No segundo tenta-se fazer a divisão do número 1 por zero, que gera um ZeroDivisionError, isto é, um erro de divisão por zero.
```
>>> 1/0

Traceback (most recent call last):
<ipython-input-18-9e1622b385b6> in <module>()
----> 1 1/0
ZeroDivisionError: division by zero
```

As mensagens de erro são fontes importantes para ajudar a descobrir problemas nos programas durante a fase de desenvolvimento.

***Obs:*** Digitação de linhas longas O símbolo “\” (barra invertida) tem a função de indicar ao terminal que um comando digitado não cabe na linha, e que a linha seguinte é uma continuação da linha que termina com a barra.
