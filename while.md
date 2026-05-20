É usado para tarefas que são repetitivas e para deixar o código menor.

exemplo: Ao invés de

```jsx
function comerPizza() {
		comerPizza()
		comerPizza()
		comerPizza()
		comerPizza()
		comerPizza()
		comerPizza()
		comerPizza()
		comerPizza()
}
```

Podemos usar

```jsx
function comerPizza() {
		while(temFatia()) {
				comerPizza()
}
```

while - siginifica “enquanto”. Enquanto houver essa função para fazer, ele irá fazer o que tem no bloco, se não, ele irá terminar a execução do código.