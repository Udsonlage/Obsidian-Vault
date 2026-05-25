window.location - Usando para direcionar para uma determinada página.

```jsx
window.location = "https://www.google.com.br"
```

replace - troca a url atual pela próxima, e deleta o histórico da anterior.
```jsx
window.location.replace("https://www.google.com.br")
```

assign - passa para a próxima url, mas não deleta a anterior do histórico.
```jsx
window.location.assign("https.//www.google.com.br")
```

reload - recarrega a página.
```jsx
window.location.reload() //é void
```

