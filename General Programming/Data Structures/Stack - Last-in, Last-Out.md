A pilha é uma forma de armazenar dados, onde o ultimo elemento inserido na pilha, vai ser o primeiro a sair.

Imagine uma louça que tem prato um em cima do outro. O ultimo prato colocado vai ser o primeiro a ser lavado, certo? É nisso que a pilha se baseia.

Uma pilha permite acesso apenas ao ultimo elemento. Se desejar acessar o penúltimo, deve-se retirar o ultimo primeiro.

![](https://miro.medium.com/v2/resize:fit:620/1*iywaX2ID2cwfI6lYMfjm5Q.png)

# Exemplo
Usar a lista em python como pilha se torna muito fácil, pois ela já possui métodos que ajudam nisso

```python
stack: int = [3, 4, 5] # definindo uma lista com o nome 'stack' e atribuindo inteiros
stack.append(6)
stack.append(7) # adicionando dois numeros - 6 e o 7

print(stack) # [3, 4, 5, 6, 7]
stack.pop() # remove o numero 7 da lista

print(stack) # [3, 4, 5, 6]

stack.pop() # remove o numero 6
stack.pop() # remove o numero 5

print(stack) # [3, 4]
```

Nesse exemplo, foi possível ver que apenas os últimos elementos adicionados na fila foram removidos primeiro, enquanto 2 primeiros permaneceram - 3 e o 4
# Links

https://docs.python.org/pt-br/3.7/tutorial/datastructures.html#using-lists-as-stacks

https://www.cos.ufrj.br/~rfarias/cos121/pilhas.html#:~:text=São%20estruturas%20de%20dados%20do,deve-se%20remover%20o%20último

https://algoritmosempython.com.br/cursos/algoritmos-python/estruturas-dados/pilhas/