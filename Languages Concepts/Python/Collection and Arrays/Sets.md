É uma coleção de dados nao ordenados que é iterável, mutável e não possui elementos duplicados. Ehh representado por **{}** - chaves

```python
firstSet = {'a', 'b', 'c'}
print(firstSet)
# {'c', 'a', 'b'}
```

Justamente pelos **sets** nao serem ordenados que nao conseguimos saber em que ordem os elementos são armazenados na memoria.

Os sets sao imutaveis, o que significa que uma vez declarado, nao podemos mudar o valor.

```
outroSet = {'Barbie', 'Ken', 'Sla'}

outroSet[1] = "Ben 10"
print(outroSet)

```