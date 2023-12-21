Uma expressão geradora é uma construção semelhante a [List Comprehension](./List%20Comprehension.md), porem contem uma instrução **yield** e retorna um objeto gerador.

Em grandes quantidades de dados, elas são uteis pois geram valores sob comanda, tornando-as mais eficientes.

![](Pasted%20image%2020231221154600.png)

A sintaxe é bem parecida com [List Comprehension](List%20Comprehension.md), porem em vez de ser colchetes **[]**, se usa parênteses **()**:

```python
generatorExpression = (expressao for elemento in iteravel if condicao)
```

os significados dessa sintaxe ai eh a mema coisa da list comprehension, entao nao vou explicar de novo nao

