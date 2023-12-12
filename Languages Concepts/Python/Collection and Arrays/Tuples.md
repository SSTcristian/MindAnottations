As tuplas são coleções de objetos (separados por virgulas). Ao contrario das listas, as tuplas são imutáveis. Elas permitem vários tipos de dados (ou seja, uma unica tupla pode conter strings, ints, booleanos e por ai vai).

Embora seja possível fazer uma tupla conter apenas UM elemento, não é tão pratico pois teríamos que colocar uma virgula no final (exemplo [aqui](#^e642aa))

### Criando Tuplas

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

^e642aa

Se quisermos, podemos iterar dentro de um for e criar uma tupla lá dentro tambem

```python
from datetime import datetime

xptoTupla = (datetime.now().date())

print('Tupla com um loop')
for i in range(0, 3):
	xptoTupla = (xptoTupla, )
	print(xptoTupla)

# output:
# Tupla com um loop
# ((datetime.date(2023, 12, 12),),)
# (((datetime.date(2023, 12, 12),),),)
# ((((datetime.date(2023, 12, 12),),),),)
```


### Acessando os elementos de uma tupla
Acessar os elementos de uma tupla é bem parecido com os métodos na lista, basta passar o valor entre colchetes ([salvo em caso que aja indexação, declarando uma tupla na variável](#^d26c9a))

```python
tuplaaaa = ('Cristian', 'Santos')

print(tupla)
# ('Cristian', 'Santos')

print(tupla[0])
# ('Cristian')
```

Tuplas com indexações e descompactadas:

```python
pq_eu_to_fazendo_isso = tuple('abcde') # tupla com indexacao

print(pq_eu_to_fazendo_isso[0])
# output: a
# nesse caso, o 0 esta pegando a primeira letra da tupla


tupla2 = ('abc', 'def', 'ghi')

a, b, c = tupla2 # tupla descompactada
print(a)
print(b)
print(c)
# abc
# def
# ghi
```

^d26c9a

Complexidades para acessar os elementos numa tupla:

**complexidade de tempo:** O(1) - constante
**complexidade de espaço:** O(1) - constante


### Concatenação de Tuplas
É o processo de unir duas OU mais tuplas, feito com o operador **+**.

Só haverá concatenação com os mesmos tipos de dados. Se tentar juntar uma tupla e uma lista, ocorrera um erro

```python
tupla1 = (0, 1, 2, 3)
tupla2 = ('Cristian', 'Santos')

concat = tupla1 + tupla2

print(concat)
# (0, 1, 2, 3, 'Cristian', 'Santos')
```

### Cortando/Fatiando Tuplas



# Links

https://www.geeksforgeeks.org/python-tuples/