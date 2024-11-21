Notação Assintótica, em si, *é uma linguagem que nos permite analisar o tempo de execução de um algoritmo através da identificação de seu comportamento com o crescimento da entrada oferecida, especialmente à medida que o tamanho da entrada (n) cresce para valores muito grandes.*

Ela é usada para analisar a eficiência de algoritmos, o que ajuda a entender o quanto o tempo de execução ou o uso de memória cresce conforme a quantidade de dados aumenta.

Abaixo vou deixar alguns exemplos em C Sharp.

# **NOTAÇÕES**

- ### **Big O ( Notação O )**
	Representa o limite superior do crescimento da função. Ela indica o **pior caso** do tempo de execução de um algoritmo. Por exemplo, O(n) significa que o tempo de execução do algoritmo cresce linearmente com o tamanho da entrada, ou seja, é um tamanho linear. - [Explanation, Example and Links](Explanation,%20Example%20and%20Links.md)
	
	### Exemplo com Busca Linear em um Array O(n):
	No pior caso, o elemento que buscamos está no final ou nem está presente, fazendo com que o tempo de execução cresça linearmente com o tamanho do array sendo `N`.

```c sharp
public bool BuscaLinear(int[] array, int valor) 
{ 
	foreach (int item in array) 
	{ 
		if (item == valor) return true; 
	} 
	return false; 
}
```

Para uma lista de `N` elementos, esse algoritmo percorre cada elemento uma vez, então sua complexidade é **O(n)**, onde o tempo de execução cresce proporcionalmente ao tamanho do array.

- ### **Ômega Ω ( Notação Ômega )**
	Representa o limite inferior do crescimento da função. Ela indica o **melhor caso** do tempo de execução de um algoritmo. Por exemplo, Ω(n) sugere que o algoritmo levará pelo menos tempo linear, mesmo no melhor cenário.

- ### **Theta Θ ( Notação Theta )**
	Representa um limite exato, o que significa que o crescimento da função está **limitado tanto acima quanto abaixo**. Em outras palavras, se um algoritmo é Θ(n), o seu tempo de execução cresce linearmente em todos os casos.