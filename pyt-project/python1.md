# Utilizando o Python Interativamente

+ Utilizaremos o Interpretador python para executarmos comandos interativamente.
+ Um comando pode ser representado por uma expressão aritmética, do tipo: **Operando1 operador Operando2**
+ Os operadores artiméticos usados em Python podem ser visualizados na tabela abaixo:
![programa](/imagens/operaritmeticos.png)

+ A ordem de execução dos operadores segue a regra de precedência da matemática e, caso necessite modificá-la, usa-se os parenteses (mais alta precedência). 
+ Entre os operadores, a exponeciação tem a precedência mais alta, assim 5**2 + 1 é igual a 26 e não 125. A multiplicação e ambas as divisões têm a mesma precedência, que são mais altas que adição e subtração, que também têm a mesma precedência. Logo, 2 * 3 - 1 é 5 e não 4, e 5 - 2 * 2 é 1 e não 6.
+ Operadores com a mesma precedência são executados da esquerda para a direita. Desta forma, na expressão 6-3+3 a subtração é realizada primeiro e tem como resultado 3. Depois adicionamos 2 e obtemos o resultado 5. Se os operadores tivessem sido executados da direira para a esquerda o resultado seria 6-(3+2) que é 1.

@[Interative Python]({"stubs": ["./www/terminal"],"command": "sh /project/target/www/terminal.sh"
})
