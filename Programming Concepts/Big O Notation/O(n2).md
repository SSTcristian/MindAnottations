Quando temos uma constante e queremos iterar sobre ela, fazemos um for. - o que caracteriza a complexidade de tempo como O(n)

Caso precisamos iterar 2 vezes essa constante, o laço for se torna com uma complexidade quadrática - O(n ^2):

###### Exemplos em CSharp:

```c sharp
// Complexidade O(n)
	public static void OpCubic(int n) 
		{
			for (int i = 0; i < n; i++) 
			{
				Console.WriteLine($"Operação O(n): {i}");
			  }
		}

// Complexidade O(n^2)

	public static void OpCubic(int n)
	{
		for (int x = 0; x < n; x++)
		{
			for (int y = 0; i < n; i++)
			{
				Console.WriteLine($"Operação O(n ^ 2): {x} - {y}");
			}
		}
	}
```

No exemplo da complexidade quadrática, temos dois laços `for` aninhados, ambos iterando n vezes. Assim, como cada laço interno executa `n` operações para cada iteração do laço externo, o total de operações é:
*n×n=n2n* .