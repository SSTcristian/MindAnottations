Abstração é o principio de criar uma classe que pode servir de base para outras classes parecidas.

Por exemplo, se eu tenho uma classe Pessoa, eu posso colocar os métodos **falar**, **andar**, **comer** e **beber** nela. Desse jeito, se eu for criar uma sub classe da Pessoa, eu poderei utilizar esses mesmos métodos sem precisar cria-los de novo

A abstração é bem parecia com a herança, de certo modo

```python
from abc import ABCMeta, abstractmethod #importanto a funcao de fazer uma classe e metodo abstrato (a classe nao precisa ser abstrata para o metodo tambem ser)

class Pessoa:

	def __init__(self, nome, idade)
		self.nome = nome
		self.idade = idade
		
	def falar(self):
		#metodo de falar
		
	def andar(self):
		#metodo de andar
		
	def comer(self)
		#metodo de comer
		
	def beber(self):
		#metodo de beber
```