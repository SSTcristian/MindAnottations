# **EXEMPLOS DE O(n²) - QUADRÁTICO COM C SHARP**

```c sharp
int[] vet = [1, 2, 3, 4, 5]

public static int BigQuadractic(int[] arr) 
{
	int count = 0;
	for (int i = 0; i < arr.length; i++)
	{
		for (int j = 0; j < arr.length; j++)
		{
			count++
		}
	}
}

Console.WriteLine(BigQuadractic(vet))
```