Testar o código garante que ele esteja funcionando corretamente e que as alterações no projeto nao cause erros. Em vez de termos que ficar escrevendo testes, podemos usar o framework **PyTest**


## Instalacao
Para instalar ele, basta utilizar o **pip**. Mas antes, vamos configurar um ambiente virtual ne (já fiz muuuita cagada por não ter feito isso, então já vou deixar o aviso logo aqui

```python
PS> virtualenv venvPyTest

PS> venvPyTest/Scripts/Activate
```

agora, basta instalar o PyTest no ambiente virtual:

```python
(venvPyTest) PS> pip install pytest
```

## Exemplo

Com um código simples, podemos usar o PyTest para verificar se tudo esta funcionando corretamente:

```python
# test.py
def increment(x):
    return x + 1

def test():
    assert increment(3) == 5
```

o **assert** verifica se o retorno do **increment(3)** vai ser igual a 5

Se digitarmos **pytest test.py** no terminal, irá aparecer a seguinte mensagem:

![](Pasted%20image%2020240101183637.png)

Isso significa que o retorno da funcao **increment(3)** nao vai ser igual a 5,