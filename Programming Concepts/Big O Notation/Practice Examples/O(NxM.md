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

- O tempo se dá pela multiplica