As lambdas são pequenas funções anônimas. Elas podem receber inúmeros argumentos, porem só podem realizar uma ação. Sao uteis quando precisamos de funcoes simples, onde nao vamos reutilizar ela m

Embora seja mais fácil de escrever do que uma função inteira, tambem é mais limitado.

No python, a sintaxe se dá pela palavra **lambda**:

```python
plusTEN = lambda x: x + 10
# declarando uma lamda onde sempre vai pegar o numero e somar mais 10

print(plusTEN(10)) # output: 20
```

Outro exemplo, porem com dois argumentos:

```python
multiply = lambda y, x: y * x
# nessa lambda, os dois argumentos sao multiplicados

print(multiply(2, 5)) # output: 10
```

