# Condições

todos os códigos até então: códigos sequenciais

agr ñ segue mais linhas verticais apenas, há desvios, desvio condicional (faz parte dos fundamentos da programação. condição/estrutura de controle)

ñ mais executando em ordem, um após o outro

**Tipos de Condição**

## Condição Simples
```
if (condicao) {
    true
}
```
## Condição Composta
```
if (condicao) {
	// sendo true
} else {
	// sendo false
}
```

automatizando a programação

### Indentação
Técnica de organização de código. Vem de "indent" em inglês, que quer dizer recuo.

* no node ñ há como usar o document.write pq ñ está dentro do navegador, então se usa o console.log() pra escrever no próprio terminal

* ``` var.innerHTML = '~~~~~' e depois outro, tem que colocar: var.innerHTML += '~~~~~~~' se n, apaga/sobrescreve o anterior ```

* {bloco}

* prática - fundamental em qualquer coisa

## Condições Aninhadas
condições uma dentro da outra

composta com outras condições dentro

amplia as possibilidades

pode ter vários níveis

```
if () {
    //
} else {
    if () {
    } else {
    }
}

↓

if () {
    //
} else if () {

} else {

}
```

raciocínio dos ifs:
```
if (idade < 16) {
    pass
} else {
    if (idade >= 16 && idade < 18) {
        pass
    }
}

↓
if (idade < 16) { 
    pass 
} else { 
    if (idade < 18) { 
        pass 
    } 
} 
```
já está implicito, se a idade não for menor que 16 obviamente ela é maior ou igual, então não precisa testar isso. seria inflar o código, escrever coisas desnecessárias

## Condição Múltipla
serve p/ valores fixos

mt útil no mundo da programação, principalmente quando quer trabalhar com valores fixos, mas ñ serve mt p/ intervalos de valores

de uma expressão testa vários valores

ñ é aplicável p/ todo tipo de situação

```
switch() {
    case 1:
        //
        break;
    case var:
        //
        break;
    default:
        //
}
```
(expressao) e ñ condicao. ñ tem como testar intervalos, e nem colocar operadores e, ou, nesse caso só com o if.

case valor ou var: break é necessário, se n após passar por um valor, que pode ser oq era esperado, continuará executando os outros comandos até encontrar um break (isso vem do C)

default - como se fosse o else do if. break no default é opcional.

só funciona com números inteiros e caracteres/'strings'

limitado, mas útil em situações pontuais

if - p/ toda situação

switch - util p/ situacoes pontuais, especificas

* o código pode ñ apresentar erro (sintático), mas pode ter de lógica
* ñ existe na programação só uma opção p/ poder fazer as coisas
* programacao - como bike, ñ pode dizer que é difícil se nunca andou

Pegando hora do sistema
```
var agora = new Date()
var hora = agora.getHours()
console.log(`Agora são exatamente ${hora} horas.`)
```
pega do sistema que estiver rodando o script, seja cliente ou servidor

com semana:
```
var agora = new Date()
var diaSem = agora.getDay()

/*
	0 - Dom
	1 - Seg
	2 - Ter
	3 - Qua
	4 - Qui
	5 - Sex
	6 - Sáb
*/

console.log(diaSem)
```
