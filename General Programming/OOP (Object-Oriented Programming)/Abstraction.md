Abstração é o principio de criar uma classe que pode servir de base para outras classes parecidas.

Por exemplo, se eu tenho uma classe Pessoa, eu posso colocar os métodos **falar**, **andar**, **comer** e **beber** nela, porem a implementação das ações desses métodos sera responsabilidade das sub classes

A super classe abstrata apenas faz assinatura dos métodos abstrata dos, mas a implementação deles se da pela sub classe

A abstração é bem parecia com a herança, de certo modo

```python
from abc import ABCMeta, abstractmethod #importanto a funcao de fazer uma classe e metodo abstrato (a classe nao precisa ser abstrata para o metodo tambem ser)

class Pessoa(ABCMeta):
	def __init__(self, nome, idade)
		self.nome = nome
		self.idade = idade
		
	@abstractmethod
	def falar(self):
		pass
		
	@abstractmethod	
	def andar(self):
		pass
		
	@abstractmethod	
	def comer(self)
		pass
		
	@abstractmethod	
	def beber(self):
		pass
```

Agora, se criarmos outra 