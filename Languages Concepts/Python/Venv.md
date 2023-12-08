Uma venv nada mais é do que um ambiente virtual isolado. Ela serve para isolar o projeto de outros, permitindo que baixemos diferentes versoes de uma mesma biblioteca.

# Utilidade
Imagine que você tenha um projeto utilizando a biblioteca PyQt5 na versão **5.15.10** e em outro projeto tenha a versao **5.15.5**. Irá dar conflito, certo?

Para isso, basta criar uma venv em cada um desses projetos, permitindo que os dois se isolem e as versões não entrem em conflitos.

```c
pip install virtualenv // instalando a venv

virtualenv --version // verificando se a venv foi instalada corretamente

virtualenv <nome da venv aqui> 
```