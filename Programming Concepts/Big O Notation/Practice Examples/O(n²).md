# **EXEMPLOS DE O(n²) - QUADRÁTICO COM C SHARP**

```c sharp

public static void Main(string[] args)
{
	int[] vet = new int[] { 1, 2, 3, 4, 5 };
	
	BigQuadractic(vet);
	// 25
	
}

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



### **SOMAR NÚMEROS DE UMA MATRIZ**

```c sharp
public static void Main(string[] args)
{

	int[,] matriz = new int[,]
	{
		{1, 2},
		{3, 4}
	}
	
	Matriz(matriz);
	// 10
	
}

public static void SomarMatriz(int[,] matriz)
{
	int count = 0;
	
	for (int i = 0; i < matriz.GetLength(dimension:0); i++)
	{
		for (int j = 0; j < matriz.GetLength(dimension:1); j++)
		{
			count += matriz[j, i];
		}
	}
	
	Console.WriteLine(count);
}
```

- No exemplo acima, estamos somando todos os números da matriz.

- Pela matriz possuir **2 dimensões** (linhas e colunas), temos que fazer um for pra cada uma

- No primeiro for, pegamos todas as linhas

- No segundo, pegamos todas as colunas

- Depois, somamos todas as linhas e colunas com `count += matriz[j, i]`