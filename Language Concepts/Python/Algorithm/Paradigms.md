Os paradigmas são métodos para resolver alguns problemas ou realizar tarefas

Um paradigma de programação é uma abordagem para resolver algum problema usando alguma linguagem de programação ou ferramentas e técnicas que nos ajudam na resolução dele. Ele define a maneira de como você organiza e estrutura seu código para resolver um problema.

Os paradigmas mais comuns são os **imperativos**, **orientado a objetos** e os **funcionais**.

- Python suporta vários paradigmas de programação, permitindo usar diferentes estilos dependendo do projeto.

## Imperativos

Este paradigma se concentra em descrever como um programa deve alcançar um determinado resultado usando instruções que alteram o resultado dele. 

Em python, consiste em uma sequencia de instruções que são executadas linha por linha:

```python
x = 10
y = 10 
plus = x + y 
print(plus) # 20
```


## Orientado a Objetos (OO / OOP)

O programa é estruturado em torno de objetos (que podem conter dados e códigos). As interações ocorrem principalmente por meio de mensagens entre objeto. C++, Java, C Sharp e o próprio Python são exemplos de linguagens orientada a objetos.

Pelo Python já ser orientado a objetos, podemos usar [classes](Object,%20Class%20and%20Instance.md), [heranças](Inheritance.md), [polimorfismos](Polymorphism.md), [encapsulações](Encapsulation.md) e [abstrações](Abstraction.md)

```python
class people:
	def __init__(self, nome: str) -> None:
		self.nome = nome
	
	def name(self):
		return self.nome

xpto = people('Cristian')

print(xpto.name()) # 'Cristian'
```


## Funcionais

Trata a computação como as funções em matemática e evita mudanças de estado e dados mutáveis. [Lambda](../Lambda/Lambda.md) e [Recursion](Recursion.md) são abordagens básicas utilizadas nesse paradigma.

```python
# com lambda
numbers = [2, 4, 6, 8, 10]
mapss = map(lambda x: x * 2, numbers)

print(list(mapss)) # [4, 8, 12, 16, 20]
```

Exemplos de recursão podem ser vistos no arquivo [Recursion](Recursion.md).