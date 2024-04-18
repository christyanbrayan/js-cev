# Próximos Passos

**Conceitos**
- fundamentos
	- evolução, paradigma client-server, Node
- variáveis e tipos de dados
	- conceitos de qualquer linguagem. tipos primitivos
- operadores
	- aritméticos, lógicos e relacionais
- condições
	- simples, composto, aninhado, operador switch
- repetições
	- while, do while, for
- arrays
	- variáveis compostas
- functions
	- paradigma funcional
- DOM
	- fazer o JS falar com o HTML e o CSS manipulando os componentes visuais, pegando dados do formulário

**Próximos**
- javascript funcional. foco em functions (mt importante p/ ling)
	- arrow functions
	- callbacks
	- funções anônimas
	- iife
- objetos
	- (pq tbm é ling. oo)
- modularização
	- (modularizar o código em arquivos separados, reutilizar códigos)
- RegEx
	- (expressões regulares)
	- bom pra validação de dados
- JSON
- AJAX
- NodeJS
	- (fzr os scripts rodarem no servidor)
	- possibilita aprender bibliotecas e frameworks

JS é uma ling. multiparadigma

## Introdução a Objetos

declaração de um array
```
let num = [5, 8, 4]
```
array no js é heterogêneo. aceita valores de tipos diferentes

por padrão os índices são numéricos, começando do zero. fixo.

pra coisas mais avançadas começa a ficar um pouco limitado

**Objeto**

declaração
```
let amigo = { ,  ,  ,  }
```
consegue colocar identificadores literais (ficando + fácil de visualizar inclusive)
```
let amigo = {nome: 'José', sexo: 'M', peso: 85.4, engordar(p){} }
```
último item tem uma função dentro
+ detalhado e + possibilidades do que o array

Objetos são variáveis (que guardam valores, atributos) que podem guardar funcionalidades (métodos)

* em js o array é um objeto e o objeto é um objeto. são estruturas da mesma classe, que vieram da mesma origem

```
let amigo = {
	nome: 'José',
	sexo: 'M',
	peso: 85.4,
	engordar(p=0) {
		console.log('Engordou')
		this.peso += p
	}
}
```

acessando os elementos
```
amigo.engordar(2)
```
a própria variável amigo tem funcionalidades dentro dela. leva a programação a outro patamar, coloca funções dentro de variáveis

tipo
```
console.log(typeof amigo)
```
retorna object

```
console.log(amigo) // retorna { nome: 'Jose', se.... }
console.log(amigo.nome) // acessando os elementos, no caso mostrando o atributo

console.log(`${amigo.nome} pesa ${amigo.peso}Kg`)
```
