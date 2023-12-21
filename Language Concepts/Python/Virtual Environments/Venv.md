Uma venv nada mais é do que um ambiente virtual isolado. Ela serve para isolar o projeto de outros, permitindo que baixemos diferentes versões de uma mesma biblioteca.

# Utilidade
Imagine que você tenha um projeto utilizando a biblioteca Selenium na versão **5.15.10** e em outro projeto tenha a versão **3.0.0**, essas duas versões irão causar conflito em algum momento.

Para isso, basta criar uma venv em cada um desses projetos, permitindo que os dois se isolem e as versões não entrem em conflitos.

```c
pip install virtualenv // instalando a venv

virtualenv --version // verificando se a venv foi instalada corretamente

virtualenv <nome da venv aqui>

<nome_da_virtualenv>/Scripts/Activate // ativando a venv

deactivate // comando para desativar
```