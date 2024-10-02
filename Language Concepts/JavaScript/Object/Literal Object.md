Um objeto literal é uma estrutura de dados usado para armazenar coleções de dados. Em resumo, um objeto literal é uma forma de criar objetos de maneira direta e concisa.

É possível definir um objeto utilizando uma sintaxe simples, usando pares de chave-valor para especificar as propriedades e os métodos.

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
	greet: function() {
		console.log(`Hello World, my name is ${this.name}`)
	}
};

console.log(Person.greet())
// -> Hello World, my name is Cristian
```

### Criando um Objeto (Nova Instancia)
Para criar uma novo objeto, temos que declarar uma instancia:
```javascript
const newObject = new Person()

///
```
