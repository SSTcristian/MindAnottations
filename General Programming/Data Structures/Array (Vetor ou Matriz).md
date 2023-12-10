Array é uma estrutura de dados simples, usado para armazenar valores num espaço continuo da memoria. 

Em python, os arrays são chamados de listas. Nela, pode-se armazenar vários tipos de dados (int, string, booleano e etc.), porem isso não eh recomendado justamente pela linearidade de memoria

- A linearidade de memoria permite que o array seja armazenado de forma consecutivos na memoria, possibilitando que 

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
As matrizes são arrays que contem linhas e colunas
