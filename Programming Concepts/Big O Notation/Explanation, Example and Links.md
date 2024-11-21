A notação Big O serve para calcular a complexidade de um algoritmo, sempre levando em conta o pior dos casos.

| **Nome**  | **Notação** |                                  **Descrição**                                  |                                           **Exemplo**                                           |
| :-------: | :---------: | :-----------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------: |
| Constante |    O(1)     |       Leva um tempo constante/fixo, independente da quantidade de dados.        |              Busca linear em um array (quando você já sabe a posição do elemento).              |
|  Linear   |    O(n)     | leva um tempo linear. Quanto maior a quantidade de dados, mais tempo irá levar. | Busca simples em um array. Quando temos que percorrer todo o array/lista para achar o elemento. |
| Logaritmo |  O(log n)   |                    Ótimo para grandes quantidades de dados.                     |            busca binaria - a cada etapa, elimina a quantidade de dados pela metade.             |
| Fatorial  |    O(!n)    |    Pior complexidade, pois rapidamente o processo se torna inviável ou lento    |                       caixeiro viajante ou permutações de uma lista.<br>                        |



# **Exemplo O(log n) com Busca Binaria**
Se eu quero procurar uma palavra no dicionário que contem 240 mil palavras, vou precisar de 240 mil etapas com a busca simples

Com a busca binaria, vou precisar de apenas 18 etapas:

240 K ->120 K -> 60 K -> 30 K -> 15 K -> 7.5 K -> 3950 -> 1875 -> 938 -> 469 -> 235 -> 118 ->59 -> 30 -> 15 -> 8 -> 4 -> 2 -> 1
  


# **LINKS**
Outras notações comuns: https://en.wikipedia.org/wiki/Big_O_notation#Orders_of_common_functions

Explicação perfeita de Big O notation: https://pt.stackoverflow.com/questions/56836/definição-da-notação-big-o