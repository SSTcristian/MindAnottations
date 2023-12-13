Um dicionário é uma coleção ordenada de valores-chaves, onde armazenam valores como se fosse um mapa. Possui Case-Sensitive.

![](Pasted%20image%2020231212202458.png)


# Criação de dicionários
O dicionário (como mostrado na imagem acima) é formado por pares de valores, onde o primeiro é a chave e o segundo é o valor:
```python
dict_var = {chave1: valor1, chave2: valor2,…..}
```


Para criar um dicionário, basta apenas seguir a sintaxe acima, porem mudar de acordo com a sua preferencia

```python
dictionary = {1: '12', 2: '12', 3: '2023'}

print(dictionary) # {1: '12', 2: '12', 3: '2023'}
```


Tambem é possível criar dicionários com diferentes valores:

```python
dicionarioA = {'Abc': 'Def', 1: [1, 2, 3, 4]}

print(dicionarioA) # {'Abc': 'Def', 1: [1, 2, 3, 4]}
```


## Adicionando elementos a um dict

A adição de elementos a um dicionário pode ser feita de diversas maneiras:

```python
emptyDict = {}
print(emptyDict) # {}

emptyDict[0] = 'cara eu nao lembro o abecedario meuDeus'
emptyDict[2] = 'abcde etc'
emptyDict[3] = 1

print(emptyDict)
# {0: 'cara eu nao lembro o abecedario meuDeus', 2: 'abcde etc', 3: 1}


emptyDict['set_Value'] = 2, 3, 4
print(emptyDict) # {'set_Value': (2, 3, 4)}



emptyDict[2] = 'sem ideia pro q escrever'
print(emptyDict)
# {2: 'sem ideia pro q escrever'}



emptyDict[5] = {'Aninhado': {'1': 'x', '2': 'y'}} 
# adicionando uma chave aninhada

print(emptyDict)
# {5: {'Aninhado': {'1': 'x', '2': 'y'}}}


# dict no final:
# {0: 'cara eu nao lembro o abecedario meuDeus', 2: 'sem ideia pro q escrever', 3: 1, 'set_Value': (2, 3, 4), 5: {'Aninhado': {'1': 'x', '2': 'y'}}}

```



# Links

https://www.geeksforgeeks.org/python-dictionary/