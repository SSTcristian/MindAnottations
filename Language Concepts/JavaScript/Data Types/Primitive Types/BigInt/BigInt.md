Foi introduzido no ECMAScript 2020 (ES11) e é usado para representar números inteiros muito grandes que não podem ser represetnados pelo tipo [Number](Number.md)

Diferente do tipo [Number](Number.md), ele não pode ser usado com o método `Math` 

# Sintaxe

```js
const big = BigInt(007199254740991)


const alsoHuge = BigInt(9007199254740991);
// 9007199254740991n


const bigString = BigInt("9007199254740991");
// 9007199254740991n


const bigHex = BigInt("0x1fffffffffffff");
// 9007199254740991n


const hugeOctal = BigInt("0o377777777777777777");
// 9007199254740991n

const hugeBin = BigInt(
  "0b11111111111111111111111111111111111111111111111111111",
);
// 9007199254740991n

```