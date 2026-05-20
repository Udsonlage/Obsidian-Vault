Enumeradores

É um conjunto de dados que podemos utilizar ou classificar por valores numerais ou textuais.

Ele é como um objeto:

```
enum dias{

    domingo = 0,

    segunda = 1,

    terça = 2,

    quarta = 3,

    quinta = 4,

    sexta = 5,

    sabado = 6

}
```

Assim como um objeto, temos a chave, que representa o nome e o valor atribuído à chave.

Não precisamos obrigatoriamente atribuir um valor à chave. Se não colocarmos, ele será atribuído com números, começando a partir do zero.

```
enum users{
	USER,
	ADM,
	DEV,
}

console.log(user.DEV) // 2
```

Também podemos declarar um enum como um tipo e usar esse valores como se fosse uma tipagem muito específica.

```
const usuarios: users = DEV;
// Só aceita os valores que estão dentro do enum
```