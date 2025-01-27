# **EXEMPLOS DE O(log n) - LOGARÍTMICA COM TYPESCRIPT**

```ts
const nums: number[] = [5, 10, 30, 55, 66, 90, 100, 120, 200]

const esquerda: number = 0

let direita = nums.length - 1 // pelo array começar do 0, temos que tirar 1 para contar como 8

let target = 200

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