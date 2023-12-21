# Sumario
- [Definição](#Definição)
- [**Exemplo de código em C que demonstra o conceito de ponteiros e vetores (arrays)**](#**Exemplo%20de%20código%20em%20C%20que%20demonstra%20o%20conceito%20de%20ponteiros%20e%20vetores%20(arrays)**)
- [Perguntas](#Perguntas)
- [Links](#Links)

# **Definição**
Em resumo, os ponteiros apontam para um endereço de memoria com algum tipo de objeto lá.

Em outras palavras, dá pra dizer que os ponteiros são as coordenadas da sua casa (longitude e latitude). Com elas, qualquer um consegue identificar onde fica a sua casa (nesse contexto, a casa seria um objeto)

O tamanho do ponteiro também varia de arquitetura para arquitetura.
Em arquiteturas de 16 bits, ele possui o tamanho de 2 bytes. Em arquiteturas de 32 bits (a mais usada antigamente), ele possui 4 bytes. A arquitetura de 64 bits (usada hoje em dia), ele possui 8 bytes. 

Porem, é quase impossível estourar a alocação de memoria de uma arquitetura de 64 bits com um ponteiro, pois ela permite endereçar 16 ExaBytes na memoria

- 1 ExaByte equivale a 1.000.000.000.000.000.000 Bytes

# **Exemplo de código em C que demonstra o conceito de ponteiros e vetores (arrays)**

```c
#include <stdio.h>

int main() {
    char *ptr; 
	// criando um ponteiro que pode armazenar o endereco de memoria de uma variavel do tipo 'char'
	
    int i;
    char vet[5] = {'a', 'b', 'c', 'd', 'e'};
    // criando um vetor do tipo 'char' que contem 5 elementos
    
    ptr = vet;
    // A variavel ponteiro ptr aponta para o primeiro elemento do vetor
    
	// o ponteiro ptr pode ser utilizado para manipular o vetor 'vet', 
	// seja fazendo uma iteracao em cima dele ou manipulando seus elementos
	
    for (i = 0; i < sizeof(vet) / sizeof(vet[0]); i++) {
        printf("\nVet[%d] = %c ptr = %c", i, vet[i], *ptr);
        ptr++;
    }
    
    return 0;
}

// retorno do for com interacao em um vetor:
// Vet[0] = a ptr = a
// Vet[1] = b ptr = b
// Vet[2] = c ptr = c
// Vet[3] = d ptr = d
// Vet[4] = e ptr = e
```

**Imagem que ilustra o exemplo acima (com alocação de memoria)**
![](../../../Images/C/Pointers/Pasted%20image%2020231220231619.png)


# **Perguntas**

## [Arrays são ponteiros?](https://pt.stackoverflow.com/questions/91336/arrays-s%c3%a3o-ponteiros)

NÃO.
- Array é previamente uma alocação de memoria de elementos contínuos, não contendo mais de um tipo de dado
- Ponteiro é uma referencia para algum local de memoria, apontando para um endereço

https://c-faq.com/aryptr/index.html

## [Como uma variável é apontada para um ponteiro?](https://pt.stackoverflow.com/questions/91365/como-uma-vari%c3%a1vel-%c3%a9-apontada-para-um-ponteiro)

```c
int array[5] = {1, 2, 3, 4, 5};
int *ptr = array
```
O valor de A é convertido para um ponteiro que aponta para o primeiro elemento do array

Seria a mesma coisa se tivesse escrito desse jeito:
```c
int *ptr = &(array[0]); // apontando para o primeiro elemento do vetor de 5 posições
```


# **Links**
https://www.codingame.com/playgrounds/24988/programacao-c/ponteiros-e-vetores
(foi nesse link onde eu peguei a imagem de ilustração)

https://pt.stackoverflow.com/questions/266756/o-que-são-ponteiros

https://pt.stackoverflow.com/questions/57006/alocação-de-objetos-e-ponteiros

https://pt.stackoverflow.com/questions/91365/como-uma-variável-é-apontada-para-um-ponteiro