É uma coleção de dados representados por nodes (nós) de forma hierárquica. 

A partir da Arvore Binaria, é possível utilizar o algoritmo BST (Binary Search Trees - Arvore de Busca Binaria), podendo estruturar os nodes com maior valor na esquerda da raiz e o nodes com menor valor na direita da raiz.

A raiz da arvore é representada no node 0 e está no topo da hierarquia. A raiz nao pode ter pais, porem o restante pode ter pais, filhos e irmaos. A arvore pode possuir no máximo 2 nodes a partir da raiz. 

![](https://algoritmosempython.com.br/images/algoritmos-python/estruturas-dados/ArvoreBinaria.png)

Os nodes de uma Arvore Binaria possuem um valor chave e dois apontadores, um para o filho da esquerda e o outro para o filho da direita. Esses apontadores representam as ligações (arestas) de uma arvore.

```python
class NodoArvore: 
	def __init__(self, chave = None, esquerda = None, direita = None):
	self.chave = chave
	self.esquerda = esquerda
	self.direita = direita
	
	def __repr__(self):
		return '%s <- %s -> %s' % (self.esquerda and self.esquerda.chave,
								   self.chave,
								   self.direita and self.direita.chave)

raiz = NodoArvore(3)
raiz.esquerda = NodoArvore(5)
raiz.direita = NodoArvore(1)
print('Arvore: ', raiz)
```


![](https://algoritmosempython.com.br/images/algoritmos-python/estruturas-dados/ArvoreBinariaRepresentacao.png)
(Imagem que representa a arvore binaria implementada no código)

O nodo raiz 3 possui dois filhos, na esquerda (com o valor 5) e o outro na direita (com o valor 1)

# Binary Search Tress (BST)
Arvores de Busca Binaria são arvores cujos os nodes são organizados de acordo com alguma preferencia

Seja **x** um node em uma árvore binária de pesquisa. Se **y** é um nodo na sub-árvore esquerda de **x**, então **y.chave** ≤ **x.chave**.  Se **y** é um nodo na sub-árvore direita de **x**, então **y.chave** ≥ **x.chave**.

Em outras palavras, em um nodo qualquer, todos os nodes na esquerda dele são menores OU iguais a ele. Todos os nodes na direita são maiores ou iguais a ele.



# Links
https://algoritmosempython.com.br/cursos/algoritmos-python/estruturas-dados/arvores/
