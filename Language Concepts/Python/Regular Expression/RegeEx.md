As expressões regulares (RegeEx) servem para buscar determinado padrão em alguma string. Por exemplo, posso usar elas para verificar se tal string corresponde a um gmail valido ou a um numero de celular correto.

![](../../../Images/Python/Regular%20Expression/Pasted%20image%2020231220233033.png)

Em python, se faz uso do modulo **re** junto com o método **re.search()**:

```
re.search(<padrao_da_string>, <string>)
```

```python
import re  
  
string = 'abc:defghi!!!'

match = re.search(r'\w', string) # \w verifica se a string contem alguma letra ou um digito

print(f'encontrado a letra "{match.group()}" ' if match else False)
# output:
# encontrado a letra "a" 
```

Com esse método, podemos verificar qualquer string dentro de um determinado padrão:

```python
import re

stringMatch = re.match(r'cris', 'cristian')

print(bool(stringMatch)) 
# retorna True, pois foi encontrado "cris" entre a string "cristian"

g = re.search(r'.', 'Cassio do Corinthians')
print(bool(g))
# True, pois "." significa qualquer tipo de caractere


barraD = re.search(r'\d\d\d', 'p123g')
print(barraD.group())
# retorna '123', pois \d é qualquer DIGITO  

barraW = re.search(r'\w\w\w', '@@abcd!!')
print(bool(barraW))
# True, \w (como ja falei) é qualquer letra (o arroba e a exclamações 
# são caracteres especiais, entao se dermos barraW.group() irá retornar apenas 'abcd')
```


# CheatSheets:

https://www.datacamp.com/cheat-sheet/regular-expresso (imagem do DataCamp lá em cima)

https://developers.google.com/edu/python/regular-expressions?hl=pt-br#basic-patterns

https://pythex.org/

https://www.geeksforgeeks.org/python-regex-cheat-sheet/

https://www.datacamp.com/cheat-sheet/regular-expresso