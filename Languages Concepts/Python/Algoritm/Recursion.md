A recursão é o nome de um processo que ocorre quando uma função chama a si mesma para fazer determinada ação. É uma técnica que permite tornar o código mais legível e mais fácil de atualiza-lo

```python
def fatorial(x: int) -> int:
	if x == 1:
		return 1
		
	return x * fatorial(x - 1) 

print(fatorial(5)) # 120
```

Nesse codigo, estamos usando a recursividade para fatorar todos os numeros antes do 5, isso é visto no return:

```python
return x * fatorial(x - 1)
```

nessa linha, estamos multiplicando o x (numero escolhido para a fatoraçção, no caso o 5)