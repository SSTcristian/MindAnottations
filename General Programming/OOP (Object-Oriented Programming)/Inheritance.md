# Definição
A **herança** consiste em aproveitar os métodos e atributos de uma classe para usar em outras classes.

# Exemplo
Supunhetamos que eu tenha a classe **cachorro**, porem também tenho uma classe chamada **animais** que possui o método **andar**, **nadar** e etc. Para eu não reinventar a roda, eu posso herdar o método **andar** da classe animal e colocar esse método na classe cachorro.

```python
# definindo uma super-classe
class Animais:
	def __init__(self) -> None:
		pass
	
    def funcaoDeAndar(self):
	    print('anda ae animal')
	    
	def funcaoDeNadar(self):
		print('nada aí')
		
# herança
class Cachorro(Animais): # -> no parenteses to herdando da classe "Animais"
    def andar(self):
	    self.funcaoDeAndar() # -> to pegando o metodo da classe "Animais"

dog = Cachorro()
dog.andar() # -> irá retornar o print 'anda ae animal'
```