# **EXEMPLOS DE O(n) - LINEAR COM C SHARP**

```c sharp
public static int SomarArr(int[] arr) 
{
	int sum = 0
	
	for (int i = 0; i < array.length; i++) 
	{
		sum += array[i]
	}
	
	return sum
}
```

- No caso, o exemplo de cima é O(n) pois o tempo de complexidade aumenta conforme o valor do parâmetro *arr* aumenta.

- Mesmo se fosse uma função de buscar o primeiro elemento, porém recebesse um parâmetro que é mutável, a notação ainda seria de O(n) - pois sempre analisamos o **pior dos casos**. O **melhor dos casos** seria O(1)

- O(n) é sempre quando temos que iterar sobre todos os itens de um vetor.