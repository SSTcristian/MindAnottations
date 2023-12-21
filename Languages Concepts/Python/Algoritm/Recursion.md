A recursão é o nome de um processo que ocorre quando uma função chama a si mesma para fazer determinada ação. É uma técnica que permite tornar o código mais legível e mais fácil de atualiza-lo.

Ela possui varias desvantagens tambem, uma delas sendo o overflow na memoria. Cada chamada dela cria um novo espaço na memoria; com tantas chamadas, pode ocorrer um estouro na memoria kabuuuuuum pow pow

Em geral, a recursividade vai depender muito de quem está usando. Se nao implementar alguma otimização (como uma tail call), ela dificilmente vai ser utilizada várias vezes.

Usando o exemplo de fatorial, podemos implementar uma função recursiva:

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

Seria a mesma coisa se utilizássemos o **for**:

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

A implementação com o for possui mais linhas, porém possui menos chance de dar um overflow na memoria caso a função recursiva seja instanciada em vários lugares.

