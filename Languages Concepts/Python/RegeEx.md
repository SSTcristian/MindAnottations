As expressões regulares servem para buscar determinado padrão em alguma string. Por exemplo, posso usar elas para verificar se tal string corresponde a um gmail valido ou a um numero de celular correto.

Em python, se faz uso do modulo **re** junto com o metodo **re.search()**

```python
import re  
  
string = 'abc:defghi!!!'

match = re.search(r'\w', string) # \w verifica se a string contem algum caractere (salvo )

print(f'encontrado {match.group()} ' if match else False)
```

