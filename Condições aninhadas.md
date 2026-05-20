é quando uma condição fica dentro de outra condição

```jsx
if (cond) {
        bloco 1
    } else {
        if (cond2) {
            bloco 2
        } else {
            bloco 3 
        }
}
```

ela é muito útil pra colocar um requisito mínimo, tipo um boolean que, se der true, ele vai liberar uma condição. Ou seja, uma condição que libera outra...