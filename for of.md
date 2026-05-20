for of - É usado para pegar o elemento de cada array, e não a posição.

```jsx
function f(...valores) { //10 e 5 são jogados aqui por ...
				let res = 0
		    for(const v of valores) { //o v é o valor, não o indice (posição)
        res += v
    }
    return res
}

console.log(f)

var valores = [10, 5]
```