Primeiro, quero destacar um dos maiores problemas do Javascript.

Quando declaramos uma variável, podemos mudar o valor atribuído a ela (menos o const), mas uma coisa interessante, é que o Javascript não liga pra diferenciação dos tipos primitivos.

No Javascript, podemos fazer isso:

```typescript
let nome = "Udson";
nome = 10

console.log(nome) //10
```

A variável continua sendo uma string, mas podemos escrever um number que a variável recebe esse valor.

Além disso, o Javacript consegue somar strings, na verdade juntá-las (concatenação).

```typescript
let valor1 = "2"
let valor2 = 5

console.log(valor1 + valor2) // "25"
```

Com o Typescript, evitamos isso, pois ele não aceita um tipo diferente da qual foi declarado antes.

```typescript
let nome = "Udson"; //string
nome = 10 //dá erro dizendo que nome tem o tipo string.
```

Uma ferramenta muito interessante é poder declarar uma tipagem até mesmo sem precisar declarar um valor:

```tsx
let nome: string;
nome = "Udson"

let idade: number = 25;

console.log(nome) // "Udson"
console.log(idade) // 25
```