Imagine um tocador de dvd. Você coloca o dvd e aperta o botão de play

Tadannnn!!! Magicamente o dvd é tocado

Encapsulamento consiste nisso. Toda a engenharia/complexidade por trás foi escondida e só é exposto a interface para o usuário usufruir do sistema.

Levando isso para programação, também podemos aplicar em Classes e Objetos, escondendo os métodos e atributos do exterior, deixando apenas a linda interface (odeio design eca)


```python
class Funcionario():
	def __init__(self, nome, cargo, valorHora):
		self.nome = nome
		self.cargo = cargo
		self.valorHora = valorHora
		self.salario = 0
		
	def registra_hora_trabalhada(self): 
		self.horas_trabalhadas += 1 
		
	def calcula_salario(self): 
		self.salario = self.horas_trabalhadas * self.valor_hora_trabalhada
```

Se o codigo ficar assim, qualquer entidade fora da classe ira conseguir acessar a propriedade **self.salario** e alterar ela

Em algumas linguagens, o encapsulamento se dá pela palavra **private**, privando um objeto e tornando-o inacessivel para outras classes, deixando apenas a interface livre pro cliente usar.
Em python o **private** vira underline


```python
class Funcionario():
	def __init__(self, nome, cargo, valorHora):
		self.nome = nome
		self.cargo = cargo
		self.valorHora = valorHora
		self.__horasTrabalhadas = 0
		self.__salario = 0
		
	def registra_hora_trabalhada(self): 
		self.__horas_trabalhadas += 1 
		
	def calcula_salario(self): 
		self.__salario = self.__horas_trabalhadas * self.valorHora
```