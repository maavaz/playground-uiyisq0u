# Utilizando o Python Interativamente

+ Utilizaremos o Interpretador python para executarmos comandos interativamente.
+ Um comando pode ser representado por uma expressão aritmética, do tipo: **Operando1 operador Operando2**
+ Os operadores artiméticos usados em Python podem ser visualizados na tabela abaixo:
![programa](/imagens/operaritmeticos.png)

+ A ordem de execução dos operadores segue a regra de precedência da matemática e, caso necessite modificá-la, usa-se os parenteses (mais alta precedência). 
+ Entre os operadores, a exponenciação tem a precedência mais alta, assim  <b> 5**2 + 1 </b> é igual a  <b>26 </b> e não  <b>125 </b>. A multiplicação e ambas as divisões têm a mesma precedência, que são mais altas que adição e subtração, que também têm a mesma precedência. Logo,  <b>2 * 3 - 1 </b> é  <b>5 </b> e não  <b>4 </b>, e  <b>5 - 2 * 2 é 1 </b> e não  <b>6  </b>.
+ Operadores com a mesma precedência são executados da esquerda para a direita. Desta forma, na expressão  <b>6 - 3 + 3 </b> a subtração é realizada primeiro e tem como resultado  <b>3 </b>. Depois adicionamos  <b>2 </b> e obtemos o resultado 5. Se os operadores tivessem sido executados da direira para a esquerda o resultado seria  <b>6 - (3 + 2) </b> que é  <b>1 </b>.

@[Interative Python]({"stubs": ["./www/terminal"],"command": "sh /project/target/www/terminal.sh"
})

-------
**Testando os conhecimentos....**
-------
?[qual o valor da expressão:  2 + 3 * 2 - 3 ** 2]
-[ ] 0
-[x] -1
-[ ] 25
-[ ] 1

?[qual o valor da expressão:  16 - 2 * 5 // 3 + 1]
-[ ] 3
-[ ] 12
-[ ] 24
-[x] 14
