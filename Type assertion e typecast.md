Type assertion é quando temos uma variável com um tipo indefinido, então definimos um tipo quando declaramos um valor para a variável:
```tsx
let nvalor: number;
let uvalor: unknown;

uvalor = 10;

//nvalor = uvalor; diz que o tipo unknown não pode ser atribuido ao tipo number

nvalor = <number>uvalor; //unknown vira tipo number com essa declaração
```
Obs.: Para fazer isso, a variável precisa, antes de tudo, ser do tipo unkown.

## Typecast

Basicamente é a conversão de tipos de forma definitiva.

Para isso, podemos utilizar o `Number()` junto com o parseFloat ou o parseInt para converter uma string para number.

Para converter um number para string, basta usar o método `toString()` .

```tsx
let nvalor: number;
let svalor: string;

nvalor = 10;

svalor = "20";

svalor = Number.parseInt(nvalor) //converte string em number
nvalor = svalor.toString(); //converte number em string
```