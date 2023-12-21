Compreensão da lista é uma maneira eficiente de criar uma lista com base em outra, permitindo [iterar](Itarables%20and%20Iterators.md) sobre seus elementos e aplicando uma expressão a cada um deles.

A sintaxe não é muito difícil tambem:
```python
listCompreension = [expressao for elemento in iteravel if condicao]
```

- **expressão** eh a qual vai ser avaliada em cada elemento da lista, como se fosse um "critério".

- **elemento** significa literalmente a variável que vai representar o elemento na lista.

- **iterável** é qualquer objeto iterável, seja tupla, lista, sets, dicts e por ai vai.

- **condição** eh uma condição que ira definir se o elemento do **iterável** ira ser incluído ou não.

# Exemplos:

Pegando apenas os números pares da **lista** e passando para a **listCompreension**
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

Dobrar todos os elementos:
```python
lst = [5, 10, 15, 25, 30]

newLst = [y * 2 for y in lst] ## ou [y + y for y in lst]

print(newLst) # [10, 20, 30, 50, 60]
```

Criando uma lista que naoo tenha a palavra 'Cristian':
```python
y = ['xpto', 'Cristian', '2023']

newLst = [x for x in y if x != 'Cristian']

print(newLst)
```

# Links
https://www.w3schools.com/python/python_lists_comprehension.asp