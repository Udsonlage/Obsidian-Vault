Podemos declarar o tipo nos arrays de algumas formas diferentes:

```tsx
let numeros: number[] = [20,30,40]
let numeros: Array<number> = [20,30,40]
let numeros: (number|string)[] = [20,30, "bruno"]
```

Também tem a possibilidade de criar um array que não pode ser alterado, mas ele ainda pode ser manipulado.

```tsx
let numeros: Readonlyarray<number> = [10,20,30]

numeros.push(11) //Não funciona
```