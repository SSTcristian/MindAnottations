Array é uma estrutura de dados simples, usado para armazenar valores num espaço continuo da memoria. 

Em python, os arrays são chamados de listas. Nela, pode-se armazenar vários tipos de dados (int, string, booleano e etc.), porem isso não eh recomendado justamente pela **linearidade de memoria**

- A linearidade de memoria permite que o array seja armazenado de forma consecutivos na memoria, permitindo um acesso mais rápido ao elemento, já que o processador ira conseguir identificar facilmente onde esta o próximo elemento pois estão todos armazenados sequencialmente

Os arrays podem ser unidimensionais (vetor) ou bidimensionais (matriz).

As informações podem ser acessadas rapidamente através de um índice, sendo sempre iniciado com zero.

# Vetor (Array Unidimensional)
Para criar um vetor (um array contendo apenas linhas), basta declarar uma variável e depois atribuir um tipo de dado a essa variável (sempre em colchetes)

```python
vetor: int = [1, 2, 3, 4, 5] # declarando o vetor como int

print(vetor) # -> [1, 2, 3, 4, 5]

print(vetor[0]) # acessando o indice 0 do vetor, irá retornar o valor 1
```


# Matriz (Array Bidimensional)
As matrizes são arrays bidimensionais, com elementos organizados em linhas e colunas.  Para criar uma matriz, é só declarar um vetor, porem varias vezes :))))

```python
matriz: int = [
	[1, 2, 3],
	[4, 5, 6],
	[7, 8, 9]
]
	
print(matriz) # -> [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
```

Se eu quiser pegar um determinado valor na matriz, é só especificar a linha e a coluna entre colchetes:

```python
print(matriz[0][1]) # retornará o numero 2
# o primeiro eh a linha e o segundo eh a coluna (matriz[linha][coluna])
```

Dado esse exemplo, se eu quiser acessar o numero 6 na lista de inteiros definido la em cima, é só eu passar as "coordenadas" do elemento:

```python
print(matriz[1][2]) # irá retornar o numero 6
```
	

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
https://kenzie.com.br/blog/o-que-array/#:~:text=programação%2C%20um%20dado.-,Como%20funciona%20um%20array%3F,pelo%20número%2C%20denominado%20como%20índice

https://osprogramadores.com/blog/2020/09/10/vetores-e-matrizes/

https://medium.com/20-21/operações-em-matrizes-numpy-613157ee74c4

https://dev.to/iugstav/python-manipulacao-de-listas-e-matrizes-4bpj
