A notação Big O serve para calcular a complexidade de um algoritmo, sempre levando em conta o pior dos casos.
| Nome | Notação | Descrição |
| Constante | O(1) | Signfi |

| Nome      | Notação  | Descrição                                                                          |
| --------- | -------- | ---------------------------------------------------------------------------------- |
| Constante | O(1)     | Leva um tempo constante/fixo, independente da quantidade de dados.                 |
| Linear    | O(n)     |                                                                                    |
| Logaritmo | O(log n) |                                                                                    |
| Fatorial  | O(!n)    | Pior complexidade para um algoritmo, pois rapidamente o processo se torna inviável |

# Nome        # Notação       # Descrição

Constante                      O(1)          significa que leva um tempo constante/fixo, independente da quantidade de dados


Linear                             O(n)          no pior dos casos, leva um tempo linear. Quanto maior a quantidade de dados, mais tempo irá levar (horrível para grande quantidade de dados)


Logaritmo                      O(log n)   ótimo para grandes quantidades de dados.
Ex de uso: busca binaria - a cada etapa, elimina a quantidade de dados pela metade


Fatorial                           O(!n)        pior complexidade para um algoritmo, pois rapidamente o processo se torna inviável/lento
Ex de uso: caixeiro viajante ou permutações de uma lista


# Exemplo O(log n) com Busca Binaria
Se eu quero procurar uma palavra no dicionário que contem 240 mil palavras, vou precisar de 240 mil etapas com a busca simples

Com a busca binaria, vou precisar de apenas 18 etapas:

240 K ->120 K -> 60 K -> 30 K -> 15 K -> 7.5 K -> 3950 -> 1875 -> 938 -> 469 -> 235 -> 118 ->59 -> 30 -> 15 -> 8 -> 4 -> 2 -> 1
  


# Outros Links
Outras notações comuns: https://en.wikipedia.org/wiki/Big_O_notation#Orders_of_common_functions

Explicação perfeita de Big O notation: https://pt.stackoverflow.com/questions/56836/definição-da-notação-big-o