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

print(vetor[0]) # acessando o indice 0 do vetor, ira retornar o valor 1
```

# Matriz (Array Bidimensional)
As matrizes são arrays bidimensionais, com elementos organizados em linhas e colunas.  Para criar uma matriz, eh so declarar um vetor, porem varias vezes :))))

```python
matriz: int = [
	[1, 2, 3],
	[4, 5, 6],
	[7, 8, 9]
]
	
print(matriz) # -> [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
```

Se eu quiser pegar um determinado valor na matriz, eh so especificar a linha e a coluna entre colchetes:

```python
print(matriz[0][1]) 
# o primeiro eh a linha e o segundo eh a coluna (matriz[linha][coluna])
```