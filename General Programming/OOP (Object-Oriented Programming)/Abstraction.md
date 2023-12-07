Abstração é o principio de criar uma classe que pode servir de base para outras classes parecidas.

Por exemplo, se eu tenho uma classe Pessoa, eu posso colocar os métodos **falar**, **andar**, **comer** e **beber** nela, porem a implementação das ações desses métodos será responsabilidade das sub classes

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

Desse jeito, criamos uma classe abstrata contendo apenas a assinatura dos métodos

Para criarmos uma sub classe dessa super classe, podemos herdar essa classe e implementar as acoes dos metodos abstratos

```python
class Euuu(Pessoa):
	def __init__(self, nome, idade):
		super().__init__(nome, idade):
		
	def beleza(self):
		beleza = 1000
		return beleza
		
	def falar(self):
		return speak():
		
	def andar():
		return walk():
		
	def comer():
		return eat():
		
	def beber():
		return drink():
```

Assim, foi implementado as ações dos métodos contidos na classe Pessoa

A super classe eh responsável por ter os atributos comuns a todas as outras sub classe (nesse caso foi **nome** e **idade**)

Assim, a abstração permite que a classe Pessoa seja definida de forma mais genérica, sem se preocupar com as particularidades de cada pessoa, deixando esses detalhes para as suas classes filhas (sub classes)

# Links
https://www.usandopy.com/pt/artigo/desvendando-o-conceito-de-abstracao-na-programacao-orientada-a-objetos/

https://dev.to/armandodelcolcoder/4-pilares-da-orientacao-a-objetos-em-python-2g1o