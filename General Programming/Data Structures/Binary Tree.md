É uma coleção de dados representados por nodes (nós) de forma hierárquica. A raiz da arvore é representada no node 0 e está no topo da hierarquia. Um node pode ter pais, filhos e irmãos. A raiz nao pode ter pais, porem o restante pode ter pais, filhos e irmaos. A arvore pode possuir no máximo 2 nodes a partir da raiz. 

![](https://algoritmosempython.com.br/images/algoritmos-python/estruturas-dados/ArvoreBinaria.png)

Os nodes de uma Arvore Binaria possuem um valor chave e dois apontadores, um para o filho da esquerda e o outro para o filho da direita. Esses apontadores representam as ligacoes (arestas) de uma arvore.

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

Imagem que representa a arvore binaria implementada acima
![](https://algoritmosempython.com.br/images/algoritmos-python/estruturas-dados/ArvoreBinariaRepresentacao.png)


O nodo raiz 3 
A partir da Arvore Binaria, é possível utilizar o algoritmo BST (Binary Search Tree - Arvore de Busca Binaria), podendo estruturar os nodes com maior valor na esquerda da raiz e o nodes com menor valor na direita da raiz.
