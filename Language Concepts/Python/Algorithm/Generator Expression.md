Uma expressão geradora é uma construção semelhante a [List Comprehension](./List%20Comprehension.md), porem contem uma instrução **yield** e retorna um objeto gerador.

Em grandes quantidades de dados, elas são uteis pois geram valores sob comanda, tornando-as mais eficientes.

![](../../../Images/Python/Generator%20Expression/Pasted%20image%2020231221154600.png)

A sintaxe é bem parecida com [List Comprehension](List%20Comprehension.md), porem em vez de ser colchetes **[]**, se usa parênteses **()**:

```python
generatorExpression = (expressao for elemento in iteravel if condicao)
```

os significados dessa sintaxe ai eh a mema coisa da list comprehension, entao nao vou colocar aqui de novo nao

# Definindo uma funcao geradora

Vamos definir uma funcao que retorna um objeto gerador:
```python
def quadractic(number: int) -> int:
	for i in range(number):
		yield i ** 2
```

Como ela retorna um objeto gerador, podemos iterar sobre o resultado com um for:

```python
for i in quadractic(6): # iterando do 0 ate o 5
	print(i) # retorna 0, 1, 2, 3, 4, 5 elevados ao quadrado
	# 0
	# 1
	# 4
	# 9
	# 16
	# 25
	
```

