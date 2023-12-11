A fila é uma estrutura de dados onde o primeiro item inserido, vai ser o primeiro a sair

Por exemplo, imagine uma fila num banco - o primeiro que está na fila vai ser o primeiro a ser atendido, consequentemente o primeiro a sair do banco.

Ao trazer essa definição para o python, em primeira opção pensa-se em usar uma lista como fila também, né? Porem usar ela como fila se torna inviável, pois fazer **insert()** e **pop()** no inicio da lista se torna lento, afinal todos os outros elementos tem que ser deslocados

Pensando nisso, o python possui uma classe chamada **collections.deque**, onde foi projetada para permitir **appends()** e **pops** tanto no final da lista, quanto no inicio.

```python
from collections import deque
queue = deque(["Eric", "John", "Michael"]) # criando uma litsa
queue.append("Terry")           # Terry arrives
queue.append("Graham")          # Graham arrives
queue.popleft()                 # The first to arrive now leaves
'Eric'
queue.popleft()                 # The second to arrive now leaves
'John'
queue                           # Remaining queue in order of arrival
deque(['Michael', 'Terry', 'Graham'])
```


# Links

https://docs.python.org/pt-br/3.7/tutorial/datastructures.html#using-lists-as-queues