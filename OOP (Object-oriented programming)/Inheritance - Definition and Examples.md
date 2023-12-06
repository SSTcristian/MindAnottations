
# Definição
A **herança** consiste em aproveitar os métodos e atributos de uma classe já existente para gerar outras classes.

## Exemplo
Supunhetamos que eu tenha a classe **cachorro**, porem também tenho uma classe chamada **animais** que possui o método **andar**, **nadar** e etc. Para eu não reinventar a roda, eu posso herdar o método **andar** da classe animal e colocar esse método na classe cachorro.

```python
# definindo uma super-classe
class animais:
	#imagine que tenha o construtor __init__ aq, to com preguica de fazer
	
    def andar(self):
	    self.andar()
	    
	def nadar(self):
		self.nadar()

# inheritance
class ac(animais):
    # attributes and method of super_class
    # attributes and method of sub_class
```