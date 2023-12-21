Compreensão da lista é uma maneira eficiente de criar uma lista com base em outra, permitindo [iterar](Itarables%20and%20Iterators.md) sobre seus elementos e aplicando uma expressão a cada um deles.

A sintaxe não é muito difícil tambem:
```python
listCompreension = [expressao for elemento in lista_original if condicao]
```

- **expressão** eh a qual vai ser avaliada em cada elemento da lista, como se fosse um "critério".
- **elemento** significa literalmente a variável que vai representar o elemento na lista
- **lista_original** eh a lista original para ser iterada
- **condição** eh uma condição que ira definir se o elemento da **lista_original** ira ser incluído ou não

# Exemplos:

Pegando apenas os números pares da **lista** e passando para a **listCompreension**
```python
lista = [1, 2, 3, 4, 5]

listCompreension = [x for x in lista if x % 2 == 0]

print(listCompreension) # [2, 4]
```

Elevando todos os numeros ao quadrado:
```python
lst = [5, 10, 25, 40]

compreension = [x ** 2 for x in lst]

print(compreension) # 
```