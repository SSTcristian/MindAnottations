
```c#
public int calculaVetor(int[] vetor) {
	int qtd = 0;
	
	for (var i = 0; i < vetor.Length; i++)
	{
		qtd += i;
	}
	
	return qtd;
}

// N = constante
// var i = 0 tbm é N
// int qtd = 0 tbm é N
// temos dois N
// se o vetor fosse 10, entao seria 2 . 10 + 3 = 23 passos pro algoritmo
// A complexidade do algoritmo é linear O(n) porque o tempo de execução cresce linearmente conforme o tamanho do vetor.
```