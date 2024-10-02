Um objeto literal é uma estrutura de dados usado para armazenar coleções de dados. Em resumo, é uma sintaxe para criar um objeto em JS composto por pares chave-valor, sendo uma maneira leve e eficiente de criar e armazenar matrizes, funções, dados complexos e etc.

# Exemplos

### Criação de um objeto literal
```javascript
const obj = {}

obj.name = 'cristian'

console.log(obj.name) // 'cristian'
```

### Armazenando Funções
Os objetos literais também podem armazenar funções
```js
const Person = {
	name: 'Cristian',
	age: 16,
	hobby: 'Programming',
	greet: () => {
		console.log(`Hello World, my name is ${this.name}`)
	}
};
```

### Criando um Objeto (Nova Instancia)
Para criar uma novo objeto, temos que declarar uma instancia:
```javascript
const newObject = new Person()

///
```
