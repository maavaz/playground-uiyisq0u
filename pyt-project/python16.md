# Processamento Condicional

### Condicional Múltipla

A estrutura do **if simples**, bem como a do **if** com **cláusula else** testam apenas uma única condição (simples ou composta). Entretanto existem situações que é necessário testar várias condições onde
apenas uma é verdadeira, e apenas esse bloco será executado. Essa situação pode ser trabalhada com vários comandos **if's encadeados** onde cada um possui uma condição. Essa variação da estrutura **if** foi projetada para tratar essas situações. 
Sua forma geral é vista a seguir:
 ![condicional](/imagens/ifmulti.png)
 
+ Apenas um bloco de comandos será executado:
Caso a condição 1 seja verdadeira, apenas o bloco de comandos da condição 1 será executado. Se a condição 1 for falsa, a condição 2 será testada. Caso a condição 2 seja verdadeira, apenas o bloco de comandos da condição 2 será executado, caso contrário testa-se a próxima condição e assim sucessivamente até encontrar uma condição verdadeira, ou que todas as condições sejam falsas. Se todas as condições forem falsas o bloco de comandos depois da clausula **else** será executado. 
+ Podem existir tantos testes **elif** quanto sejam necessários, e a clausula **else** é opcional. 

+ Exemplo de estrutura condicional com múltiplas condições: 
    + selecione o botão **Run** para execução do programa;
    + retire # das atribuições (uma de cada vez) para testar outras alternativas;
     
``` python runnable
# Este programa verifica a sensação térmica dada uma temperatura
temp = 26.7
# Tente como exemplo as temperaturas abaixo:
# temp = 15.3
# temp = -4.5
if temp >= 30:
    print("Muito calor")
elif temp >= 24:
    print("Calor")
elif temp >= 17:
    print("Temperatura Amena")
elif temp >= 7:
    print("Temperatura Fria")
else:
    print("Muito fria")
```
