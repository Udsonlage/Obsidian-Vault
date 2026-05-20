No typescript podemos declarar uma variável com mais de um tipo usando |

```tsx
let vteste: string | number;
vteste = "Udson";
vteste = 25;
```

Se não quisermos especificar um tipo na variável, podemos usar o any

```tsx
let vteste: any;
vteste = "Udson";
vteste = 25;
```