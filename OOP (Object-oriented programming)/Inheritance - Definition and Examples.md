
# Definição
A **herança** consiste em aproveitar os métodos e atributos de uma classe já existente para gerar outras classes.

## Exemplo
Supunhetamos que eu tenha a classe **cachorro**, porem também tenho uma classe chamada **animais** que possui o método **andar**, **nadar** e etc. Para eu não reinventar a roda, eu posso herdar o método **andar** da classe animal e colocar esse método na classe cachorro.

```python
# definindo uma super-classe
class Animais:
	#imagine que tenha o construtor __init__ aq, to com preguica de fazer
	
    def andar(self):
	    self.funcaoDeAndar()
	    
	def nadar(self):
		self.funcaoDeNadar()

# herança
class Cachorro(animais): # <- no parenteses to herdando da classe "Animais"
    def andar(self):
	    self.funcaoDeAndar() # <- to pegando o metodo da classe "Animais"
```