É uma coleção de dados nao ordenados que é iterável, mutável e não possui elementos duplicados. Ehh representado por **{}** - chaves


### Criando Sets

Para criar um set, basta declarar uma variável e as chaves com os elementos dentro
```python
firstSet = {'a', 'b', 'c'}
print(firstSet)
# {'c', 'a', 'b'}
```

Justamente pelos **sets** NAO serem ordenados que nao conseguimos saber em que ordem os elementos são armazenados na memoria.


##### Mudando o valor de um set
Os sets são imutáveis, o que significa que uma vez declarado, nao podemos mudar o valor. Caso mesmo assim tentarmos muda-lo, ira ocorrer um erro de **TypeError**.

```python
outroSet = {'Barbie', 'Ken', 'Sla'}

outroSet[1] = "Ben 10"
print(outroSet)

# ERROR!
# Traceback (most recent call last):
#   File "<string>", line 3, in <module>
# TypeError: 'set' object does not support item assignment
```


##### Armazenando dados
Os sets podem armazenar muitos tipos de dados de uma só vez:

```python
abcSet = {"Cristian", "Santos", 12, 12, True}

print(abcSet)
# {True, 'Santos', 12, 'Cristian'}
```