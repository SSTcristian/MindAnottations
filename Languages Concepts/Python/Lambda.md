As lambdas são pequenas funções anônimas. Elas podem receber inúmeros argumentos, porem só podem realizar uma ação. São uteis quando precisamos de funções simples, onde não vamos reutilizar ela muitas vezes.

Embora seja mais fácil de escrever do que uma função inteira, tambem é mais limitado.

No python, a sintaxe se dá pela palavra **lambda**:

```python
plusTEN = lambda x: x + 10
# declarando uma lamda onde sempre vai pegar o numero e somar mais 10

print(plusTEN(10)) # output: 20
```

O mesmo código funcionaria se a lambda estivesse dentro do print:
```python
print((lambda x: x + 10)(10)) # output: 20
```

Outro exemplo, porem com dois argumentos:

```python
multiply = lambda y, x: y * x
# nessa lambda, os dois argumentos sao multiplicados

print(multiply(2, 5)) # output: 10
```

Embora da pra se utilizar as lambdas assim, é mais comum ela ser utilizada em conjunto com os métodos **map**, **filter** e **reduce**.

### MAP
```python
listNumbers = [1, 3, 2, 4, 6, 8, 10, 11, 12]

quadratic = list(map(lambda x: x** 2, listNumbers))
#filtrando todos os numeros pares na lista

print(quadratic)
# [1, 9, 4, 16, 36, 64, 100, 121, 144]
```
## Lambda com Filter
```python
listNumbers = [1, 3, 2, 4, 6, 8, 10, 11, 12]

filterEvens = list(filter(lambda x: x % 2 == 0, listNumbers))
#filtrando todos os numeros pares na lista

print(filterEvens)
# [2, 4, 6, 8, 10, 12]
```