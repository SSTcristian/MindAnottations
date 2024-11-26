# **EXEMPLOS DE O(n²) - QUADRÁTICO COM C SHARP**

```c sharp

public static void Main(string[] args)
{
	int[] vet = new int[] { 1, 2, 3, 4, 5 };
	
	BigQuadractic(vet);
	// 25
	
}q

public static void BigQuadractic(int[] arr)
{
	int count = 0;
	for (int i = 0; i < arr.Length; i++)
	{
		for (int j = 0; j < arr.Length; j++)
		{
			count++;
		}
	}
	Console.WriteLine(count);
}
```

- O código acima retorna 25 pois a notação O(n²) sempre aumenta conforme o número de for cresce. Explico melhor no [O(n²)](Programming%20Concepts/Big%20O%20Notation/Asymptotic%20Notation/O(n²).md), já que aqui é só exemplos práticos