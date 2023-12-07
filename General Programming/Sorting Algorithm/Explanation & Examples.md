# `Métodos Simples`

## Inserction Short
Percorre um vetor (int) da esquerda para direita, ordenando os elementos um por um.

Possui complexidade de `O(n²)`. Método de ordenação estável

## Selection Short
A ordenação por seleção ou selection short consiste em selecionar o menor item e colocar na primeira posição, selecionar o segundo menor item e colocar na segunda posição, seguindo esses passos até que reste apenas um elemento. 

Para todos os casos (melhor, médio e pior caso), possui complexidade de `O(n²)` e não é um algoritmo estável.

# `Métodos Eficientes`

## QuickSort
O Algoritmo QuickSort, criado por _C. A. R. Hoare_ em 1960, é o método de ordenação interna mais rápido que se conhece para uma ampla variedade de situações.

Provavelmente é o mais utilizado. Possui complexidade `O(n²)` no pior caso e `O(n log n)` no melhor e médio caso e não é um algoritmo estável.

## Merge Short
O algoritmo divide o problema em pedaços menores, resolve cada pedaço e depois junta (merge) os resultados. O vetor é dividido em duas partes iguais , que serão cada uma dividas em duas partes, e assim até ficar um ou dois elementos cuja ordenação é trivial. 

Possui complexidade de `O(n log n)` para todos os casos

## Shell Short
Ele permite a troca de registros distantes um do outro, diferente do algoritmo de ordenação por inserção que possui a troca de itens adjacentes para determinar o ponto de inserção.

A complexidade do algoritmo é desconhecida, ninguém ainda foi capaz de encontrar uma fórmula fechada para sua função de complexidade e o método não é estável.

