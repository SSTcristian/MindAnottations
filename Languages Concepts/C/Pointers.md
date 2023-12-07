Em resumo, os ponteiros apontam para um endereço de memoria com algum tipo de objeto lá.

Em outras palavras, dá pra dizer que os ponteiros são as coordenadas da sua casa (longitude e latitude). Com elas, qualquer um consegue identificar onde fica a sua casa (nesse contexto, a casa seria um objeto)

```c
#include <stdio.h>

int main() {
 char *ptr; // criando um ponteiro que pode armazenar o endereco de memoria de uma variavel do tipo 'char'

 char vet[5] = {'a', 'b', 'c', 'd', 'e'}; // criando um vetor do tipo 'char' que contem 5 elementos

 ptr = vet;  // A variavel ponteiro ptr aponta para o primeiro elemento do vetor

// o ponteiro ptr pode ser utilizado para manipular on vetor 'vet', seja fazendo uma iteracao em cima dele ou manipulando seus elemtentos

for (i = 0; i < vet; i++) {
	  printf("\nVet[%d] = %c ptr = %c", i, vet[i], *ptr); // o conteudo do vetor acessada variavel e pelo ponteiro
	  ptr++;
	}
}
```

[Exemplo do código com ponteiros apontando para um endereço de memoria](https://www.codingame.com/servlet/fileservlet?id=41409364165150)
![](https://www.codingame.com/servlet/fileservlet?id=41409364165150)

Nesse codigo, 