A regra do termo dominante diz que o **termo que cresce mais rápido** vai sobrepor ao **termo que cresce mais devagar**.

Em outras palavras, a medida que **n** se torna muito grande, algum termo eventualmente irá dominar todos os outros termos na expressão.



# EXEMPLO
Dado um tempo **O(n² + 3n + 2)**, qual é o termo dominante dele?

> *Resposta* : 
> Primeiro, temos que remover as constantes (todos os números sem o **n** ao lado - ou seja, o 2)
> Agora, temos que comparar os dois termos - **n²** e **3n**, para verificar qual cresce mais rápido
> o **n²** múltiplica o *n* ao quadrado, então em 

#### SIMPLIFICANDO
- **Constantes são ignoradas**: **3n** é tratado como **n**, e 2 é simplesmente ignorado.
- 
- **Focamos no termo com a maior taxa de crescimento**: Neste caso, é **n²**.

#### CONCLUSÃO
O termo dominante de **O(n² + 3n + 2)** é **n²**, porque ele cresce mais rapidamente do que os outros termos quando *n* aumenta. Assim, a complexidade de tempo é simplificada para **O(n²)**.
