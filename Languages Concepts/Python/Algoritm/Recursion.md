A recursão é o nome de um processo que ocorre quando uma função chama a si mesma para fazer determinada ação. É uma técnica que permite tornar o código mais legível e mais fácil de atualiza-lo

```python
def fatorial(x: int) -> int:
	if x == 1:
		return 1
		
	return x * fatorial(x - 1) 

print(fatorial(5)) # 120
```

Nesse código, estamos usando a recursividade para fatorar todos os números antes do 5, isso é visto no return:

```python
return x * fatorial(x - 1)
```

o **return** pega o x (numero escolhido para a fatoração, no caso o 5) e multiplica usando recursividade.

seria a mesma coisa se utilizassemos o for:

```python
def fatorial(n):
	if n == 1:
		return 0
	
	for i in n:
		return i * n - 1

print(fatorial(5))
```