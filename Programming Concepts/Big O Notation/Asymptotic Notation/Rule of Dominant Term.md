A regra do termo dominante diz que o **termo que cresce mais rápido** vai sobrepor ao **termo que cresce mais devagar**.

Em outras palavras, a medida que **n** se torna muito grande, iremos pegar o termo que cresce mais *devagar*, ou seja, o pior termo (em questão de tempo) daquela notação.

![](../../../Images/Programming%20Concepts/Big%20O%20Notation/Pasted%20image%2020241120210018.png)


*(imagens de [Iniciando com a notação Big O.](https://www.toniesteves.com/introduction-to-big-o-notation))*

# EXEMPLO
Dado um tempo **O(n² + 3n + 2)**, qual é o termo dominante dele?

> *Resposta* : 
> - Primeiro, temos que remover as constantes (todos os números sem o **n** ao lado - ou seja, o 2). Porém, não podemos remover os expoentes (como o ² )
> 
> - Agora, temos que comparar os dois termos - **n²** e **3n**, para verificar qual cresce mais rápido.
> 
> - **n²**: Este termo múltiplica o *n* ao quadrado. Por exemplo, se *n* é igual a 10, então *n x n* é igual a *100*. [Veja mais clicando aqui](O(n²).md).
> 
> - **3n:** Este termo também cresce, mas não tão rapidamente quanto **n²**. Ele aumenta proporcionalmente a *n* (linearmente). Ou seja, se *n =10*, então será *n x 3*, o que nos retorna *10*.
> 
> - Sabendo disso, o *pior* termo dessa notação é o **n²** e, consequentemente, cresce mais rapidamente do que os outros termos quando *n* aumenta.
> - Portanto, o termo dominante/complexidade de tempo dessa notação é [O(n²)](O(n²).md).

#### SIMPLIFICANDO
- **Constantes são ignoradas**: **3n** é tratado como **n**, e 2 é simplesmente ignorado.

- **Focamos no termo com a maior taxa de crescimento**: Neste caso, é **n²**.

#### CONCLUSÃO
O termo dominante de **O(n² + 3n + 2)** é **n²**, porque ele cresce mais rapidamente do que os outros termos quando *n* aumenta. Assim, a complexidade de tempo é simplificada para **O(n²)**.



# "TERMO CRESCE MAIS RAPIDAMENTE"
*vou deixar algumas anotações aqui pq de começo nao entendi mt bem essa frase*

"Quando dizemos que "um termo cresce mais rapidamente", estamos nos referindo a como o valor desse termo aumenta à medida que *n* (o tamanho da entrada) se torna maior. Essa ideia está relacionada à **taxa de crescimento** da função matemática que descreve o termo."

![](../../../Images/Programming%20Concepts/Big%20O%20Notation/Pasted%20image%2020241119004305.png)