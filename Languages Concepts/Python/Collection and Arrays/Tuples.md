As tuplas são coleções de objetos (separados por virgulas). Ao contrario das listas, as tuplas são imutáveis. Elas permitem vários tipos de dados (ou seja, uma unica tupla pode conter strings, ints, booleanos e por ai vai).

Embora seja possível fazer uma tupla conter apenas UM elemento, não é tão pratico pois teríamos que colocar uma virgula no final (exemplo [aqui](#^e642aa))

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


## Acessando os elementos de uma tupla
Acessar os elementos de uma tupla eh bem parecido com os métodos na lista, basta passar o valor entre colchetes ([salvo em caso que aja indexacao, declarando uma tupla na variavel](#^d26c9a))

```python
tuplaaaa = ('Cristian', 'Santos')

print(tupla)
# ('Cristian', 'Santos')

print(tupla[0])
# ('Cristian')
```

Tuplas com indexacoes e descompactadas:

```python
pq_eu_to_fazendo_isso = tuple('abcde')

print(pq_eu_to_fazendo_isso[0])
# output: a
# nesse caso, o 0 esta pegando a primeira letra da tupla


```
