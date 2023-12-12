A fila é uma estrutura de dados onde o primeiro item inserido, vai ser o primeiro a sair

Por exemplo, imagine uma fila num banco - o primeiro que está na fila vai ser o primeiro a ser atendido, consequentemente o primeiro a sair do banco.

![](https://dkrn4sk0rn31v.cloudfront.net/uploads/2020/11/Estrutura-de-dados-Fila-3.png)

![](https://dkrn4sk0rn31v.cloudfront.net/uploads/2020/11/Estrutura-de-dados-Fila-4.png)

Ao trazer essa definição para o python, em primeira opção pensa-se em usar uma lista como fila também, né? Porem usar ela como fila se torna inviável, pois fazer **insert()** e **pop()** no inicio da lista se torna lento, afinal todos os outros elementos tem que ser deslocados

Pensando nisso, o python possui uma classe chamada **collections.deque**, onde foi projetada para permitir **appends()** e **pops** tanto no final da lista, quanto no inicio.

```python
from collections import deque
queue = deque(["Agostinho Carrara", "Neo do Matrix", "Caneta Azul"]

queue.append("Cristian") # inserindo 'Cristian' na lista
queue.append("Santos")

queue.popleft() # Indicando que o primeiro a ser inserido, vai ser o primeiro a sair (ou seja, o Agostinho Carrara)

queue.popleft() # O segundo a ser inserido vai ser removido - infelizmente o Neo do Matrix

print(queue) 
# Imprimindo a lista em ordem de chegada
# output: deque(['Caneta Azul', 'Cristian', 'Santos'])
```


# Links

https://docs.python.org/pt-br/3.7/tutorial/datastructures.html#using-lists-as-queues

https://www.treinaweb.com.br/blog/o-que-e-e-como-funciona-a-estrutura-de-dados-fila