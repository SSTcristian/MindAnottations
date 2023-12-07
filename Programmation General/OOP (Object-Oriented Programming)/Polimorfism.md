# Definição
Polimorfismo consiste em uma subclasse ter o mesmo nome de um método da superclasse, porem executando diferentes funções

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

