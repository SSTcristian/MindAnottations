# Object
O objeto é um conjunto de bytes, formando dados/informações. Em si, um objeto pode ser um array, uma string, um inteiro, um dicionário, uma estrutura de dados ou qualquer coisa que armazena informação

Ta ligado numa variável? É nela que damos um nome a um objeto, de certa forma

```python
xpto = 12345
```

nesse caso, estamos atribuindo o conjunto de inteiros (bytes) na variável xpto, ou seja, alocando esses bytes em um endereço na memoria, a qual podemos acessar a qualquer momento através da variável xpto

Especificamente, a variável não é um objeto em si, mas sim um local de armazenamento para o real objeto

# Class
Uma classe, falando tecnicamente, é um conjunto de métodos e propriedades que define o comportamento de uma entidade (vulgo objeto)

As classes atuam como um modelo para os objetos

Imagine que a classe é a planta de uma casa, é um modelo a ser seguido para a construção e possui certas características. Essa casa ainda não existe, pois só está no papel

O objeto é a CASA. É algo teoricamente físico (pro computador), existe em tempo de execução, já teve um build e existe na memoria.

A casa (classe) só vai passar a existir quando construirmos (build a aplicação) ela, ou seja, quando instanciamos (objeto) a classe

["Então o objeto é uma instância da classe. Na classe você pode dizer que aquele objeto terá uma cor, no objeto você diz qual é a cor, só pode dizer isso porque foi definido na classe que essa informação deve estar no objeto."](https://pt.stackoverflow.com/questions/100812/qual-a-diferen%C3%A7a-entre-uma-classe-e-um-objeto?noredirect=1&lq=1#:~:text=Ent%C3%A3o%20o%20objeto%20%C3%A9%20uma%20inst%C3%A2ncia%20da%20classe.%20Na%20classe%20voc%C3%AA%20pode%20dizer%20que%20aquele%20objeto%20ter%C3%A1%20uma%20cor%2C%20no%20objeto%20voc%C3%AA%20diz%20qual%20%C3%A9%20a%20cor%2C%20s%C3%B3%20pode%20dizer%20isso%20porque%20foi%20definido%20na%20classe%20que%20essa%20informa%C3%A7%C3%A3o%20deve%20estar%20no%20objeto.) <- isso eh um link, nao seja burro futuro eu

```python
# exemplo de classe em python

class Pessoa:
	#construindo os parametros da classe
	def __init__(self, nome, idade):
		self.nome = nome
		self.idade = idade
		
	def dados(self):
		return f'{self.nome}, {self.idade} anos'

#instanciando a classe
pessoa1 = Pessoa('Adrian Lindo', 15) 
# o primeiro parametro é o nome, o segundo é a idade

print(pessoa1.dados()) # -> retornará 'Adrian Lindo, 15 anos'
```


# Instance

É a instancia de uma classe, vulgo objeto que cria a classe

```python
# esse codigo foi usado la em cima, to usando pra ficar mais facil
pessoa1 = Pessoa('Adrian Lindo,' 15)
```

essa variável 'pessoa1' está instanciando a classe Pessoa1, ou seja, esta construindo a classe com as propriedades/parâmetros que ela tem
# Links

https://pt.stackoverflow.com/questions/205482/em-programação-o-que-é-um-objeto

https://pt.stackoverflow.com/questions/100812/qual-a-diferença-entre-uma-classe-e-um-objeto?noredirect=1&lq=1