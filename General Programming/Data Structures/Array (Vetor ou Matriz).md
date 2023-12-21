Array é uma estrutura de dados simples, usado para armazenar valores num espaço continuo da memoria. 

Em python, os arrays são chamados de listas. Nela, pode-se armazenar vários tipos de dados (int, string, booleano e etc.), porém isso não é recomendado justamente pela **linearidade de memoria**

- A linearidade de memoria permite que o array seja armazenado de forma consecutivos na memoria, permitindo um acesso mais rápido ao elemento, já que o processador ira conseguir identificar facilmente onde esta o próximo elemento pois estão todos armazenados sequencialmente

Os arrays podem ser unidimensionais (vetor) ou bidimensionais (matriz).

As informações podem ser acessadas rapidamente através de um índice, sendo sempre iniciado com zero.

- No arquivo **[Lists](../../Language%20Concepts/Python/DS%20&%20Iterators/Lists.md)**, é possível ver mais exemplos sobre manipulação de vetores.

# Vetor (Array Unidimensional)
Para criar um vetor (um array contendo apenas linhas), basta declarar uma variável e depois atribuir um tipo de dado a essa variável (sempre em colchetes)

```python
vetor: int = [1, 2, 3, 4, 5] # declarando o vetor como int

print(vetor) # -> [1, 2, 3, 4, 5]

print(vetor[0]) # acessando o indice 0 do vetor, irá retornar o valor 1
```


# Matriz (Array Bidimensional)
As matrizes são arrays bidimensionais, com elementos organizados em linhas e colunas.  Como declaro uma matriz? Se vira ai otario

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
# o primeiro é a linha e o segundo é a coluna (matriz[linha][coluna])
```

Dado esse exemplo, se eu quiser acessar o numero 6 na lista de inteiros definido la em cima, é só eu passar as "coordenadas" do elemento:

```python
print(matriz[1][2]) # irá retornar o numero 6
```



# Links
https://kenzie.com.br/blog/o-que-array/#:~:text=programação%2C%20um%20dado.-,Como%20funciona%20um%20array%3F,pelo%20número%2C%20denominado%20como%20índice

https://osprogramadores.com/blog/2020/09/10/vetores-e-matrizes/

https://medium.com/20-21/operações-em-matrizes-numpy-613157ee74c4

https://dev.to/iugstav/python-manipulacao-de-listas-e-matrizes-4bpj
