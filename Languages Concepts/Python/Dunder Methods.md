os métodos dunder (ou métodos mágicos) se refere a métodos que começam e terminam com dois sublinhados (**__init__, __str___** e por ai vai)

Eles são usados para fornecer funções especiais as classes em python e são chamados por debaixo dos panos pelo interpretador

Para vê-los, podemos passar a função **dir()**, sendo o parâmetro uma classe para mostrar quais métodos dunder ela herda

```python
print(dir(int)) # mostra quais metodos dunder a classe "int" herda

# output:
# ['__abs__', '__add__', '__and__', '__bool__', '__ceil__', '__class__', '__delattr__', '__dir__', '__divmod__', '__doc__', '__eq__', '__float__', '__floor__', '__floordiv__', '__format__', '__ge__', '__getattribute__', '__getnewargs__', '__getstate__', '__gt__', '__hash__', '__index__', '__init__', '__init_subclass__', '__int__', '__invert__', '__le__', '__lshift__', '__lt__', '__mod__', '__mul__', '__ne__', '__neg__', '__new__', '__or__', '__pos__', '__pow__', '__radd__', '__rand__', '__rdivmod__', '__reduce__', '__reduce_ex__', '__repr__', '__rfloordiv__', '__rlshift__', '__rmod__', '__rmul__', '__ror__', '__round__', '__rpow__', '__rrshift__', '__rshift__', '__rsub__', '__rtruediv__', '__rxor__', '__setattr__', '__sizeof__', '__str__', '__sub__', '__subclasshook__', '__truediv__', '__trunc__', '__xor__', 'as_integer_ratio', 'bit_count', 'bit_length', 'conjugate', 'denominator', 'from_bytes', 'imag', 'numerator', 'real', 'to_bytes']
```


Também é possível fazer isso abrindo o cmd do python e digitando **dir(int)**

![](Pasted%20image%2020231215190531.png)


# Exemplos
### **__repr__** e **__str__**
Em resumo, o método **__repr__** eh uma representação de sua classe, feito para mostrar os detalhes dela. **__repr__** é uma abreviação de **representation**.

Quanto ao **__str__**, ele tambem é uma representação da classe, porem ele é chamado automaticamente quando você da um print numa instancia.

A principal diferenca 

```python
class classeXpto:
	def __init__(self, nome):
		self.nome = nome
		
	def __repr__(self):
		return f'classeXpto({self.nome})'
		
	def __str__(self):
		return f'Instancia da classe classeXpto - {self.nome}'

print(classeXpto('Cristian')) # Instancia da classe classeXpto - Cristian
print(repr(classeXpto('Cristian'))) # classeXpto(Cristian)
```

Quando a classe nao tiver o metodo **__str__**, o interpretador irá pegar o método **__repr__**


# Links

https://www.geeksforgeeks.org/dunder-magic-methods-python/