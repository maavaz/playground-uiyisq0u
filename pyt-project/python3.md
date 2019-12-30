# Strings

São compostos por um conjunto de caracteres alfanuméricos (cadeias de caracteres) escritos usando aspas simples ou duplas
Ex.: 
"abc" ou 'abc' 

## Operações com Strings
+ O operador “+” pode ser usado para concatenar strings
   Ex.: "a"+"b" é o mesmo que "ab"
+ O operador “*” pode ser usado para repetir strings
   Ex.: "a"*10 é o mesmo que "aaaaaaaaaa"
+ Os caracteres não imprimíveis (pex Enter) podem ser expressos usando notação “barra-invertida” (\)

  ++ \n é o mesmo que new line (Enter)
  ++ \r é o mesmo que carriage return (retornar para o início da linha)
  ++ \t é o mesmo que tab 
  ++ \b é o mesmo que backspace
  ++ \\ é o mesmo que \ 
  ++  \x41 é o mesmo que o caractere cujo código hexadecimal é 41 (“A” maiúsculo)
  
  ```
  Obs: O comando print exibe as informações na tela do usuário. Formato print(string)
>>> print "ab\rd" # \r retorna para o início da linha, portanto irá exibir o caracter d seguido do b.
db

>>> print "abc\td" # \t irá realizar a tabulação (6 espaços em branco) depois irá exibir a letra d
abc     d

>>> print "abc\nd" # \n representa o Enter e, por isso, exibirá os carateres a seguir na linha debaixo
abc
d

>>> print "abc\\nd" # \\ irá exibir o caracter barra
abc\nd

>>> print "ab\bc" # \b representa o bacspace, portanto retornará uma casa.
ac

>>> print "\x41\xA1" # \x41 representa o A maiúsculo e \xA1 representa o caracterc í
Aí

  ```
