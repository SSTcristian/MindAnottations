Em resumo, os ponteiros apontam para um endereço de memoria com algum tipo de objeto lá.

Em outras palavras, dá pra dizer que os ponteiros são as coordenadas da sua casa (longitude e latitude). Com elas, qualquer um consegue identificar onde fica a sua casa (nesse contexto, a casa seria um objeto)

```c
#include <stdio.h>

int main() {
 char *ptr; // criando um ponteiro que pode armazenar o endereco de memoria de uma variavel do tipo 'char'
 int i;
 char vet[5] = {'a', 'b', 'c', 'd', 'e'}; // criando um vetor do tipo 'char' que contem 5 elementos

 ptr = vet;  // A variavel ponteiro ptr aponta para o primeiro elemento do vetor

// o ponteiro ptr pode ser utilizado para manipular o vetor 'vet', seja fazendo uma iteracao em cima dele ou manipulando seus elementos

for (i = 0; i < vet; i++) {
	  printf("\nVet[%d] = %c ptr = %c", i, vet[i], *ptr);
	  ptr++;
	}
}

// retorno do for com interacao em um vetor:
// Vet[0] = a ptr = a
// Vet[1] = b ptr = b
// Vet[2] = c ptr = c
// Vet[3] = d ptr = d
// Vet[4] = e ptr = e
```

## **Imagem que ilustra a alocação de um objeto em um endereço da memoria**
![](https://www.codingame.com/servlet/fileservlet?id=41409364165150)




# Links
https://www.codingame.com/playgrounds/24988/programacao-c/ponteiros-e-vetores

https://pt.stackoverflow.com/questions/266756/o-que-são-ponteiros

https://pt.stackoverflow.com/questions/91336/arrays-são-ponteiros

https://pt.stackoverflow.com/questions/57006/alocação-de-objetos-e-ponteiros

https://pt.stackoverflow.com/questions/91365/como-uma-variável-é-apontada-para-um-ponteiro