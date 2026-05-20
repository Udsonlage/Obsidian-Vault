## Document Object Model | modelo de objeto de documento

O navegador cria uma “árvore” do HTML para que o JavaScript possa usá-lo.

temos uma hierarquia no DOM:

![[Pasted image 20260520171342.png]]

Os elementos dentro do DOM podem ser reconhecidos e puxados através de alguns termos:

- Parent: É a camada pai, a principal

ParentElement - Dentro do DOM, é o elemento pai.

ParentNode - Dentro do DOM, é o conteúdo que tem dentro do elemento.

- Child: Dentro da camada pai se encontram toda as camadas filho.

childNodes - Dentro do DOM, é o conteúdo do elemento filho.

children - Dentro do DOM, é o elemento filho.

- siblins - São os irmãos. iguais na mesma posição no DOM. Se dentro de uma div temos 5 spans, essas 5 spans são siblins.

```jsx
const main = document.getElementsByTagName('main')
const botao = [...document.querySelectorAll(".curso")]

console.log(main[0].children) //Filhos do main, contando com os conteúdos
console.log(botao[0].parentNode) //Irmãos/ iguais dentro da const botão
```

através dessa hierarquia, podemos selecionar qualquer elemento no javascript:

```jsx
var botao = window.document.selectElementByName('botao')
```

aqui ele está declarando a variável botao selecionando um elemento em HTML através do DOM.

getElementsByTagName() - para selecionar a tag

getElementsByClass() - para selecionar uma class

getElementsById() - para selecionar um id

querySelector() - selecionar de forma específica

## Criando elementos:

Podemos criar elementos HTML pelo Javascript e até mesmo criar ids e class nelas:

creatElement() - Cria uma tag HTML

```jsx
const novoElemento = document.createElement("div")
```

.setAttribute() - Cria um atributo para a tag, como um id, class, src, etc.

```jsx
novoElemento.setAttribute("class","curso")
```

.appendChild() - Adiciona o elemento criado em um pai.

```jsx
main.appendChild(novoElemento)
```

.removeChild() - Remove um elemento de um pai.

```jsx
main.removeChild(remover)
```

Exemplo completo de código:

```jsx

const main = document.querySelector('#principal')
const curso = ["HTML","CSS","Javascript","PHP","React","MySQL"]

curso.map((el) => { //usado para percorrer todos os elementos de curso.
    const novoElemento = document.createElement("div")
    novoElemento.setAttribute("class","curso")
    novoElemento.innerHTML = el

    novoElemento.addEventListener('click', (evt) => {
        const remover = evt.target
        main.removeChild(remover)
    })

    main.appendChild(novoElemento)
})
```