Compreensão da lista é uma maneira eficiente de criar uma lista com base em outra, permitindo [iterar](../DS%20&%20Iterators/Itarables%20and%20Iterators.md) sobre seus elementos e aplicando uma expressão a cada um deles.

![](Pasted%20image%2020231220231314.png)

Como visto acima, a sintaxe não é muito difícil também:
```python
listCompreension = [expressao for elemento in iteravel if condicao]
```

- **expressão** é a qual vai ser avaliada em cada elemento da lista, como se fosse um "critério".
 ^ad8926
- **elemento** significa literalmente a variável que vai representar o elemento na lista.

- **iterável** é qualquer objeto iterável, seja tupla, lista, sets, dicts e por aí vai.

- **condição** é uma condição que vai definir se o elemento do **iterável** irá ser incluído ou não.

# Exemplos:

Pegando apenas os números pares da **lista**:
```python
lista = [1, 2, 3, 4, 5]

listCompreension = [x for x in lista if x % 2 == 0]

print(listCompreension) # [2, 4]
```

Elevando todos os números ao quadrado:
```python
lst = [5, 10, 25, 40]

compreension = [x ** 2 for x in lst]

print(compreension) # [25, 100, 625, 1600]
```

Dobrando todos os elementos:
```python
lst = [5, 10, 15, 25, 30]

newLst = [y * 2 for y in lst] # ou [y + y for y in lst]

print(newLst) # [10, 20, 30, 50, 60]
```

Criando uma lista que não tenha a palavra 'Cristian':
```python
y = ['xpto', 'Cristian', '2023']

newLst = [x for x in y if x != 'Cristian']

print(newLst) # ['xpto', '2023']
```

# Links

https://www.w3schools.com/python/python_lists_comprehension.asp

https://realpython.com/list-comprehension-python/