
A complexidade O(n²) é conhecida como **complexidade quadrática**. Esse tipo de complexidade aparece em algoritmos onde precisamos realizar operações para cada combinação de elementos em uma coleção, o que normalmente envolve **dois laços aninhados** que iteram sobre o mesmo conjunto de dados.

## Exemplificando
Quando temos uma constante e queremos iterar sobre ela, fazemos um for. - o que caracteriza a complexidade de tempo como O(n):

```c sharp
public static void OpCubic(int n) 
		{
			for (int i = 0; i < n; i++) 
			{
				Console.WriteLine($"Operação O(n): {i}");
			  }
		}
```
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
*n × n = n²*. A complexidade O(n2)O(n^2)O(n2) é conhecida como **complexidade quadrática**. Esse tipo de complexidade aparece em algoritmos onde precisamos realizar operações para cada combinação de elementos em uma coleção, o que normalmente envolve **dois laços aninhados** que iteram sobre o mesmo conjunto de dados.

*³⁴*