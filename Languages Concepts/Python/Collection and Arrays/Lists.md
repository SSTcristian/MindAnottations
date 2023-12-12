As listas são arrays de tamanho dinâmico (isso em C é um vetor), um tipo de dados em sequencia que armazena uma coleção de dados.

```python
names = ['Caneta Azul', 'Ben 10']

print(names) # ['Caneta Azul', 'Ben 10']
```

As listas tambem são mutáveis, permitindo que alteramos ela mesmo depois da declaração

# Manipulando as listas (array) em python
## Inserindo Elemento
Para inserir elemento em uma lista já criada, basta utilizar o método **lista.append(elemento)**

```python
lista = [2, 4, 6, 8, 10]
print(lista) # [2, 4, 6, 8, 10]

lista.append(12)

print(lista) # [2, 4, 6, 8, 10, 12]
```


## Removendo Elementos na Lista
Para remover um elemento em uma lista, é só utilizar o método **remove()**

```python
xpto = [10, 2, 2008]
print(xpto) # [10, 2, 2008]

xpto.remove(2008)

print(xpto) # [10, 2]
```


## Cortar (ou dividir) as listas
Há duas formas de dividir as listas no python: usando colchetes ou o método **slice(intervalo)**

```python
naoAguentoMaisEscreverLista = ['socorro', 'aaaaa', 'nao aguento mais']
print(naoAguentoMaisEscreverLista) # ['socorro', 'aaaaa', 'nao aguento mais']

print(naoAguentoMaisEscreverLista[0:2])
# nesse print, ira cortar a lista da posicao 0 ate a 2
# output: ['socorro', 'aaaaa']

print(naoAguentoMaisEscreverLista[0:1])
# cortando do indice 0 ate o 1
# ['socorro']

sliceMethod = slice(0, 2)
print(naoAguentoMaisEscreverLista[sliceMethod])
# mesma coisa dos colchetes, mas esse eh utilizando o metodo slice()
# output: ['socorro', 'aaaaa']

sliceMethod = slice(1, 2)
print(naoAguentoMaisEscreverLista[sliceMethod])
# output: ['aaaaa']

```

## Tamanho da Lista
O método **len()** retornará o tamanho da lista

```python
lst = [1, 2]

print(len(lst)) # -> 1
```

# Links
https://www.geeksforgeeks.org/python-lists/

https://roadmap.sh/python#:~:text=Lists%2C%20Tuples%2C%20Sets%2C%20and%20Dictionaries