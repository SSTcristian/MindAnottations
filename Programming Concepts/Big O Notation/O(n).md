
```c#
public int calculaVetor(int[] vetor) {
	int qtd = 0; // => N
	
	for (var i = 0; i < vetor.Length; i++)
	{
		qtd += i;
	}
	
	return qtd;
}

// N = constante
// var i tbm é N
// temos dois N
// se o vetor fosse 10, entao seria 2 . 10 + 3 = 23 passos pro algoritmo
// complexidade aumenta conforme a entrada, ou seja, n linear
```