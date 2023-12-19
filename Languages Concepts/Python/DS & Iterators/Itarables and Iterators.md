# Itarables
Os iteráveis são objetos que podem ser iterados, ou seja, é possível percorrer todos os valores contidos dentro desse objeto.

o **for** é justamente pra isso, percorrer os elementos de um iterador:

```python
lst = [1, 2, 3, 4, 5]

for x in lst: # percorrendo todos os elementos
	print(x) # printando eles para sair um embaixo do outro

# output:
# 1
# 2
# 3
# 4
# 5
```

Eu também poderia percorrer os elementos e no final passar um __print(x **2)__ para elevar todos os números da lista ao quadrado:

```python
print(x ** 2)

# 1
# 4
# 9
# 16
# 25
```


# Iterators
O iterador é um objeto usado para percorrer todos os objetos iteráveis.

[Lists](Lists.md), [Tuples](Tuples.md), [Dictionaries](Dictionaries.md), [Sets](Sets.md) e Strings são objetos iteráveis.

Todos eles possuem 2 métodos:
- **iter()** que é usado para obter um iterador
- **next()** para percorrer o iterador e ver o próximo elemento. Quando passamos um for, internamente ele usa o **iter()** para obter um iterador e o **next()** para iterar.

```python
tupla = ('Cristian', 'Santos', 'abc')

it = iter(tupla) # iterador

print(next(it)) # ('Cristian')
print(next(it)) # ('Santos')
print(next(it)) # ('abc')
```

Nesse exemplo, toda vez que passamos o método **next()**, estamos dizendo para o python pegar o próximo objeto do iterador.

# Links
https://www.geeksforgeeks.org/iterators-in-python/

https://realpython.com/python-iterators-iterables/#:~:text=Iterators%20power%20and%20control%20the,one%20value%20at%20a%20time

https://www.w3schools.com/python/python_iterators.asp

