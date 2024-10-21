No geral, a complexidade ciclomática "*serve para mensurar a complexidade de um determinado módulo (seja uma função, uma classe, um método...), a partir da contagem do número de caminhos independentes que ele pode executar até o seu fim.* 

Em outras palavras, o resultado dessa complexidade nos mostra quantos testes o código precisa executar para verificar todos os fluxos possíveis que tal ação pode tomar.

**Exemplo:**

![](https://i0.wp.com/artesoftware.com.br/wp-content/uploads/2019/09/23560-complexidade-ciclomatica-sorveteria-impl2.png?resize=712%2C329&ssl=1)

## CALCULO

Para calcularmos ela, existem 3 formas diferentes:

- Usando a notação de um [grafo de fluxo](https://pt.wikipedia.org/wiki/Grafo_de_fluxo_de_controle);
- Usando [fluxograma](https://pt.wikipedia.org/wiki/Fluxograma);
- Com **análise estática** do código, usando uma ferramenta que automatize essa tarefa.

Possuindo um grafo de fluxo ou um fluxograma, possuímos então 3 maneiras para mensurar a complexidade ciclomática:

1. **V(G) = R** - onde **R** é o número de regiões do grafo de fluxo.
2. **V(G) = E – N + 2** - onde **E** é o número de arestas (setas) e **N** é o número de nós do grafo G.
3. **V(G) = P + 1** - onde **P** é o número de nós predicados contidos no grafo G (só funciona se os nós predicado tiverem no máximo duas arestas saindo.)

(exemplo com a notação de grafo de fluxo)
![](https://d2m498l008ebpa.cloudfront.net/2017/02/grafo.png)

# LINKS
[Complexidade ciclomática, análise estática e refatoração | Blog da TreinaWeb](https://www.treinaweb.com.br/blog/complexidade-ciclomatica-analise-estatica-e-refatoracao)