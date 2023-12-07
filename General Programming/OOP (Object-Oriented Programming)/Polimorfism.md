# Definição
Polimorfismo consiste em uma subclasse ter o mesmo nome de um método da superclasse, porem executando diferentes funções.

Poli = muitos

morfismo = não sei oq é

Ou seja, um método pode ter varias formas (ações)

# Exemplo
```python
class Super:
	def printHI(self):
		print('fala meu mano')

instance = Super()
instance.printHI() # -> 'fala meu mano'

class Sub(Super):
	def printHI(self):
		print('subclasse aq parceiro')

xptoBlaBlaBla = Sub()
xptoBlaBlaBla.printHI() # -> 'subclasse aq parceiro' 
```

Dado esse exemplo, pode-se ver que o polimorfismo consiste em 'sobrepor' um método já existente, alterando as ações que ele faz.

Porém, se fizermos que a sub herde de outra sub que herda de uma superclasse?????
nao sei otario se vira pra entender

Simples, ele vai herdar a sub da sub

```python
class Super:
	def printHI(self):
		print('fala meu mano')

class Sub(Super): # -> herdando a super classe
	def printHI(self):
		print('subclasse aq parceiro')

class SubSub(Sub) # -> herdando a sub classe
	def printHI(self):
		print('sub da subclasse')

ins = SubSub()
ins.printHI() # -> sub da subclasse
```



