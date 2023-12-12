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
		#adicionando __ antes do nome, essa propriedade fica "oculta"
		
	def registra_hora_trabalhada(self): 
		self.__horas_trabalhadas += 1 
		
	def calcula_salario(self): 
		self.__salario = self.__horas_trabalhadas * self.valorHora
```

Mesmo assimm, isso so indica que essa variavel nao devera ser acessada, porem se tentarmos ainda vai dar para acessa-la

```python
cristian = Funcionario('Cristian', 'GP rs', 50) # definindo os metodos da classe
pedro.__salario = 100000 #alterando o valor do salario
print(pedro.__salario) # -> 100000
```

Se quisermos impedir esse tipo de alteracao, podemos usar o decorator **@property**

```python
def __init__(self, nome, cargo, valorHora):
		self.nome = nome
		self.cargo = cargo
		self.valorHora = valorHora
		self.__horasTrabalhadas = 0
		self.__salario = 0
		
	@property 
	def salario(self): 
		return self.__salario
		
	@salario.setter 
	def salario(self, novo_salario): 
		raise ValueError("Impossivel alterar salario diretamente. Use a funcao calcula_salario().") 
		
	def registra_hora_trabalhada(self): 
		self.__horas_trabalhadas += 1 
		
	def calcula_salario(self): 
		self.__salario = self.__horas_trabalhadas * self.valor_hora_trabalhada
```


Agora, se tentarmos alterar o salario, ira retornar uma mensagem de erro

```python
cristian = Funcionario('Cristian', 'Garoto de Programa rsrs', 50) 
cristian.salario = 100000

##############################
Traceback (most recent call last):
  File "encapsulamento.py", line 26, in <module>
    f.salario = 1000
  File "encapsulamento.py", line 16, in salario
    raise ValueError("Impossivel alterar salario diretamente. Use a funcao calcula_salario().")
ValueError: Impossivel alterar salario diretamente. Use a funcao calcula_salario().
```



# Links

https://algoritmosempython.com.br/cursos/programacao-python/encapsulamento/

https://cursos.alura.com.br/forum/topico-o-que-o-metaclass-abcmeta-faz-184749