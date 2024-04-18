# Introdução ao DOM

**VSCode**
Extensão Watch in Chrome no VSCode e VSCode Watch in Chrome no Chrome
Ctrl+Shift+P

-watch in chrome

Ou Live Server

Arquivo - salvamento automático (sempre útil)

Extensão Node Exec no VSCode (pra habilitar a tecla F8 pra rodar o código js pelo node)

## Document Object Model
vertente web do JS, pro qual a linguagem foi criada

poderosa ferramenta que já está dentro do navegador

conjunto de objetos do JS

p/ tratamento de componentes visuais

**Modelo de Objetos para Documentos**

basicamente um conjunto de objetos dentro do navegador, que vai dar acesso aos componentes internos do website

n funciona dentro do node

presente quando se está executando js dentro do navegador

**Árvore Dom**

começa da raiz, o navegador:

window

tudo dentro do js está dentro de um objeto DOM chamado window, a janela do navegador

dentro há vários objetos, alguns deles:: location (localização do site. url, pagina atual, anterior), document (documento atual), history (vai guardando de onde veio e p/ onde vai , que facilita a navegação dentro do site)

Na árvore hierárquica há os parents (pai/mae) e os childs

```
document
↓
html ↓ head (↓ meta, title ), body (↓ h1, p ↓ strong (podendo ter mais de 1), span)
dentro de cada há outros objetos, os filhos
```

- importante conseguir montar na cabeça a🎄, pq vai precisar acessar os seus componentes

**Acessando**
```
window.document.body
window.document.write(' ') // escreve sobre o documento
```
por js, por dom, adicionou componente

ñ é a melhor maneira de fazer isso, mas é a mais simples

há como mostrar coisas:
```
window.document.write(window.document.charset) // retorna utf-8
                      window.navigator.appName // retorna netscape
                      window.document.URL
```
consegue buscar algumas configurações da página

há várias formas de navegar por esses componentes, entre os elementos (toda e qualquer coisa que aparece no DOM)

há como selecionar elementos p/ poder navegar dentro da árvore dom, selecionando um componente. há vários métodos para isso:

**Alguns Métodos de Acesso**
- por marca (tag)
	- document.getElementsByTagName('p')[0]
		- consegue fazer acesso a todos os componentes
		- quando é no plural tem que indicar qual componente vai usar. 0 - 1º, 1 - 2º...
		- write(p1.innerText)
			- escreve o texto dentro do p, q no caso foi jogando dentro de uma var
		- p.style.color = 'blue'
			- possibilidades com a var que recebe o metodo get
		- innerText e innerHTML
			- primeiro só mostra o texto, sem a formatacao html, como por exemplo um strong
			- no alert o segundo n funciona, mostra as tags como se fossem texto, e n as formata
			- quando faz p.innerText = ' ' substitui o conteudo pelo que houver entre ''. manda modificar por js usando o dom
- por id
	- getElementById('')
		- ```<div id=""></div>```
- por nome
	- getElementsByName('')[]
		- ```<div name=""></div>```
- por classse
	- getElementsByClassName('')[]
		- ```<div class=""></div>```
- por seletor
	- querySelector('div#msg')
	- querySelectorAll()
		- +recente, com a sintaxe do css, e + recomendado
		- 2 - plural
		- .class #id

quer selecionar quando tem + de um objeto da mesma classe ou nome - por marca, por nome

quer selecionar um objeto ou uma familia deles - id