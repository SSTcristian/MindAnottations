As tuplas são coleções de objetos (separados por virgulas). Ao contrario das listas, as tuplas são imutáveis. Elas permitem vários tipos de dados (ou seja, uma unica tupla pode conter strings, ints, booleanos e por ai vai).

Embora seja possível fazer uma tupla conter apenas UM elemento, é meio complicado pois teríamos que colocar uma virgula no final (exemplo [aqui](#Criando%20Tuplas))

## Criando Tuplas

```python
tupla = ('Cristian', 15, True) 
# tupla que possui 3 tipos de dados diferentes

print(tupla) 
# ('Cristian', 15, True)
```

Tambem é possível criar tuplas repetidas ou alinhadas

```python
repetitionTuple = ('Cristian', ) *3
# indicando ao compilador para repetir esse elemento na tupla 3 vezes

print(repetitionTuple)
# ('Cristian', 'Cristian', 'Cristian')



firstNested = (0, 1, 2, 3)
secondNested = ('nao aguento mais escrever socorro')

finalNested = (firstNested, secondNested) 
# juntando as duas tuplas

print(finalNested) 
# ((0, 1, 2, 3), 'nao aguento mais escrever socorro')
```

