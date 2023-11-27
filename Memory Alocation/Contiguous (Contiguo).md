# Definição Real
É um modelo de alocação que atribui memorias de forma contigua.

- **Vantagens:**
    - Acesso rápido à memória, já que os endereços (pedras) são consecutivos.
    - Implementação relativamente simples.
- **Desvantagens:**
    - Fragmentação interna: O espaço não utilizado entre as alocações pode levar a desperdício de memória.
    - Dificuldade em acomodar processos de tamanho variável (pequeno, médio e grande).

# Explicação como se eu fosse um Neandertal (CHAT-GPT)
## **Alocação de Memória Contígua:**

- **Igual a uma parede de caverna:** Imagine uma parede de caverna longa e reta. Cada pedra na parede é como um espaço de memória consecutivo. Os dados ficam todos juntinhos, um do lado do outro, como pedras enfileiradas.
    
- **Na prática:** É como se todos os lugares para guardar coisas fossem uns coladinhos nos outros. Se eu quero guardar cinco coisas, coloco uma ao lado da outra, e elas ficam numa linha, bem organizadas.

- Desvantagem: 
	Então, imagina caverna com muitas pedras. Alocação de memória contígua é como organizar essas pedras todas em uma fila, uma do lado da outra. 
	
	Agora, desvantagem disso é que, às vezes, quando guardamos coisas pequenas entre as pedras grandes, sobra um espacinho. É como se colocasse uma frutinha entre duas pedronas, mas fica um espaço vazio, e isso não é aproveitado.
	
	Assim, essa fila pode ter pedras grandes e pequenas, mas entre elas pode ter espaços inúteis. Esses espaços vazios podem ser desperdício, tipo ter buracos na fila. Isso pode ser um problema se a caverna ficar cheia de buracos e não tiver espaço suficiente para guardar mais coisas.
	
	Então, a desvantagem da alocação contígua é que, às vezes, fica um espacinho inútil entre as pedras, e isso pode ser como ter buracos na parede da caverna.

