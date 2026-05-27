Type assertion é quando temos uma variável com um tipo indefinido, então definimos um tipo quando declaramos um valor para a variável:
```tsx
let nvalor: number;
let uvalor: unknown;

uvalor = 10;

//nvalor = uvalor; diz que o tipo unknown não pode ser atribuido ao tipo number

nvalor =<number> uvalor; //unknown vira tipo number com essa declaração
```