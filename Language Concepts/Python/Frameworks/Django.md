Django é um framework usado em desenvolvimento web. Ele é open-source e gratuito.

Ele separa o processo em duas fases: **Request Phase** e **Response Phase**

![](../../../Images/Python/Django/Pasted%20image%2020240104193000.png)

# Arquitetura
Ele usa a arquitetura **MVT** (**Model View Template**), bem parecida com a **MVC** que é utilizada em C#, Java, PHP e por ai vai.

- **Model**: representa a camada de dados e a logica por trás dos negócios
```python
from django.db import models

class Person(models.Models):
	firstName = models.CharField(max_length=40)
	secondName = models.CharField(max_length=40)
```

Nesse exemplo, estamos definindo uma model chamada **Person**, a qual possui 2 campos: **firstName** e **secondName**.

Cada um desses campos ehh especificado como um atributo da classe 
- **View:** lida com a interface do usuário. No Django, representa a logica que processa as solicitações do usuário e retorna uma resposta.

- **Template:** responsável pela apresentação da informação (semelhante a **view** no MVC). É um arquivo de modelo que define como os dados da **Model** devem ser tratados.

# Links
https://www.djangoproject.com/

https://www.djangoproject.com/start/

https://blog.geekhunter.com.br/django-introducao-ao-framework/

