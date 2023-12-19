A recursão é o nome de um processo que ocorre quando uma função chama a si mesma para fazer determinada ação. É uma técnica que permite tornar o código mais legível e mais fácil de atualiza-lo.

Ela possui varias desvantagens tambem, uma delas sendo o overflow na memoria. Cada chamada dela cria um novo espaço na memoria; com tantas chamadas, pode ocorrer um estouro na memoria kabuuuuuum pow pow

Em geral, a recursividade vai depender muito de quem esta a usando. Se implementar uma 

```python
def fatorial(x: int) -> int:
	if x == 1:
		return 1
		
	return x * fatorial(x - 1) 

print(fatorial(5))
# output: 120
```

Nesse código, estamos usando a recursividade para fatorar todos os números antes do 5, isso é visto no return:

```python
return x * fatorial(x - 1)
```

o **return** pega o x (numero escolhido para a fatoração, no caso o 5) e multiplica usando recursividade.

seria a mesma coisa se utilizássemos o **for**:

```python
def fatorial(n: int) -> int:
	if n == 1:
		return 0

	result = 1
	for i in range(1, n + 1):
	    result *= i
		
	return result

print(fatorial(5))
# output: 120
```

A implementacao com o for possui mais linhas, porem possui menos chance de dar um overflow na memoria caso a funcao recursiva seja instanciada em varios lugares