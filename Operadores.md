tipos de operadores

- aritméticos
- atribuição
- relacionais
- lógicos
- ternário

## **aritméticos:** +

/ % ** (potência)

operadores binários são que precisamos de 2 elementos para a operação ex.: 5 + 2

precedência (ordem)

- ()
- **
- *, /, %, +, -
- +, -

```jsx
var a = 5 + 3 //8
var b = a % 5 //3
var c = 5 * b ** 2 //45
```

**Auto atribuições:**

ele pode se colocar na própria variável pra fazer um calculo

```jsx
var n = 3
n = n + 4
n = n - 5
n = n * 4
```

podemos simplificar

```jsx
var x = 2
x += 3
```

operador de incremento simplifica mais ainda:

```jsx
var x = 4
x++
```

**relacionais:**

<

> = <= == !=

```jsx
5 > 2 = true
7 < 4 = false
8 >= 8 = true
9 <= 7 = false
5 == 5 = true //== é sinal de igual na programação
4 != 4 = false //!= é sinal de diferente
5 === '5' = false //=== é sinal de extamente igual
5 !== '5' = true //!== é sinal de totalmente diferente
```

**lógicos:**

! negação && conjunção || disjunção

```jsx
 5 > 2 && 5 == 2 = false //se uma das duas contas der errado, dá false
 6 < 7 || 2 === '2' = true //se uma das duas contas der errado, ele dá true mesmo assim
```

Ordem de usar cada operador no código

() ** /

> < >= ! && ||

**Ternário:**

? :

Isso parece muito com a lógica de if e else, mas de uma forma muito simples.

```jsx
var media = 5.5
media >= 6? 'aprovado' : 'reprovado'
//"média é maior ou igual a 6? Se sim, 'aprovado', se não, 'reprovado'."
```

Spread:

…

Serve para pegar os elementos do array e jogar dentro de uma função ou outro array

```jsx
var n1 = [10, 20, 30]
var n2 = [11, 22, 33, 44]
var n3 = [...n1] //esses ... repetem o array de var n1

console.log(`n3: ${n3}`) // 
```

```jsx
const jogador1 = {nome: 'Udson', vida: 200, força: 300}
const jogador2 = {nome: 'Gui', vida: 250, magia: 500}
const jogador3 = {...jogador1, ...jogador2}

console.log(jogador3) //console não adiciona os dois const, mas sim o último e ele replica as infos que não estão repetidas nos objetos
```