É uma coleção de dados nao ordenados que é iterável, mutável e não possui elementos duplicados. Ehh representado por **{}** - chaves

![](../../../Images/Python/Sets/Pasted%20image%2020231212212417.png)

### Criando Sets

Para criar um set, basta declarar uma variável e as chaves com os elementos dentro:

```python
firstSet = {'a', 'b', 'c'}
print(firstSet)
# {'c', 'a', 'b'}
```

Justamente pelos **sets** NÃO serem ordenados que não conseguimos saber em que ordem os elementos são armazenados na memoria.


Para adicionar um elemento, basta passar o método **.add(elemento)**:

```python
outroSet = {'Barbie', 'Ken', 'Batman'}
print(outroSet) # {'Ken', 'Barbie', 'Batman'}


outroSet.add('Caneta Azul')


print(outroSet) # {'Ken', 'Caneta Azul', 'Batman', 'Barbie'}

```


Eles também podem armazenar muitos tipos de dados de uma só vez:

```python
abcSet = {"Cristian", "Santos", 12, 12, True}

print(abcSet)
# {True, 'Santos', 12, 'Cristian'}
```


# Sets congelados

Os sets congelados (**frozen sets**) são imutáveis, sendo essa a principal diferença dos sets normais. Uma vez criados, eles nao podem ser alterados depois. Eles tambem não são ordenados.

Para cria-los, é só usar a função **frozenset()**

```python
frozenSets = frozenset(['a', 'b', 'c'])

print(frozenSets) # frozenset({'b', 'a', 'c'})
```


# Links

https://www.geeksforgeeks.org/sets-in-python/