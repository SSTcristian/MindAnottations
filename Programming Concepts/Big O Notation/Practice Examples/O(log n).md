# **EXEMPLOS DE O(log n) - LOGARÍTMICA COM C SHARP**

```ts
const nums: number[] = [1, 2, 3, 4, 10, 25, 60, 80, 100]

const esquerda: number = 0

let direita = nums.length - 1 // pelo array começar do 0, temos que tirar 1 para contar como 8

let target = 25

let count = 0

while(esquerda <= direita) {
    let meio = (esquerda + direita) / 2;
    
    count++
    
    console.log(meio);
    break;
    
    if(nums[meio] == target) {
        console.log('Numero encontrado -> ' + target)
    }
    
    if (nums[meio] > target) {
        direita = meio - 1
    }

}
```