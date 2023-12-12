É uma coleção de dados nao ordenados que é iterável, mutável e não possui elementos duplicados. Ehh representado por **{}** - chaves


### Criando Sets

Para criar um set, basta declarar uma variável e as chaves com os elementos dentro
```python
firstSet = {'a', 'b', 'c'}
print(firstSet)
# {'c', 'a', 'b'}
```

Justamente pelos **sets** NAO serem ordenados que nao conseguimos saber em que ordem os elementos são armazenados na memoria.



Os sets são mutáveis, basta passar o método **.add(elemento)** para adicionar um valor

```python
outroSet = {'Barbie', 'Ken', 'Batman'}
print(outroSet) # {'Ken', 'Barbie', 'Batman'}


outroSet.add('Caneta Azul')


print(outroSet) # {'Ken', 'Caneta Azul', 'Batman', 'Barbie'}

```



Eles tambem podem armazenar muitos tipos de dados de uma só vez:

```python
abcSet = {"Cristian", "Santos", 12, 12, True}

print(abcSet)
# {True, 'Santos', 12, 'Cristian'}
```


# Sets congelados

Os sets congelados (**frozen sets**) sao imutaveis, sendo essa a principal diferenca dos sets normais. Uma vez criados, 