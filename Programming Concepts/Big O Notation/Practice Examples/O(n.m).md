# **EXEMPLOS DE O(n * m) - POLINOMIAL COM C SHARP**

```c sharp
int[] nums1 = { 1, 2, 3}; // n
int[] nums2 = {4, 5, 6}; // m

// O(n * m) = 4

int count = 0;
for (int i = 0; i < nums1.Length; i++)
{
	for (int j = 0; j < nums2.Length; j++)
	{
		count++;
		Console.WriteLine(nums1[i] + " " + nums2[j]);
	}
}

Console.WriteLine($"Passos: {count}");
```

- O tempo se dá pela multiplicação entre o `nums1` e o `nums2`
- Pelo `nums1` ter 3 digitos e o `nums2` tbm, fazemos **3 * 3**, o que resulta em **9**
- Esse 9 é a quantidade de passos que ele vai demorar para chegar no resultado