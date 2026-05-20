usamos condições para criar caminhos alternativos baseado nas respostas que o JavaScript recebe.

if - literalmente “se”. A condição começa nele.

else - literalmente “se não”. Acontece caso o if não for uma alternativa.

else if - aqui, para não finalizarmos com o else, usamos o else if para continuar com outras possibilidades.

## Condição Simples:

é a condição que só tem um if e else

```jsx
var tempo = 29

if (tempo >= 30) {
    console.log('Está quente!')
} else {
    console.log('Está frio!')
}
```


## Condição múltipla

usada para quando temos muitas possibilidades dentro de uma opção só

```jsx
var estacao = 'sol' //Os valores que são colocados aqui precisam estar nas possibilidades de case.

switch(estacao) {
    case 'sol':
        console.log('É verão')
        break
    case 'frio':
            console.log('É inverno')
        break
    case 'chuva':
            console.log('É outono')
            break
    case 'fresco':
            console.log('É primavera')
        break
    default:
        console.log('ERRO')
        break
}
```

switch - é o que define a condição múltipla.

case - cada case colocado é uma possibilidade que seria colocada na variável.

abaixo do case, ele vira um bloco onde colocamos os códigos da condição.

break - usado para, se caso a condição terminar em tal case, ele não pular para os cases de baixo. Se isso acontece, o js coloca o case que parou junto com os de baixo.

defaut - é como se fosse o “se não” no switch. Se não aparecer nenhuma das opções de case.