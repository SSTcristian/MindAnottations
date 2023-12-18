Um iterador é um objeto que pode ser iterado, ou seja, é possível percorrer todos os valores contidos dentro desse objeto.

[Lists](Lists.md), [Tuples](Tuples.md), [Dictionaries](Dictionaries.md) e [Sets](Sets.md) são objetos iteráveis.

Todos eles possuem um método chamado **iter()** que é usado para obter um iterador:

```python
tupla = ('Cristian', 'Santos', 'abc')

it = iter(tupla)

print(next(it)) # ('Cristian')
print(next(it)) # ('Santos')
print(next(it)) # ('abc')
```



# Links
https://realpython.com/python-iterators-iterables/#:~:text=Iterators%20power%20and%20control%20the,one%20value%20at%20a%20time

