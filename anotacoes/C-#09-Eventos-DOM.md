# Eventos DOM

DOM - facilitador que existe dentro do navegador, dentro do HTML5 p/ dar acesso aos elementos diretamente para o js.

sem ele teria mt dificuldade p/ poder acessar os elementos da página

Eventos - tudo aquilo que possa acontecer ou fazer com um elemento (div, por ex)

o que pode acontecer de + comum é com mouse:

**com mouse**

* mouseenter - dispara ao aproximar dentro, ao mouse entrar no elemento
* mousemove - dispara várias vezes enquanto move dentro do elemento
* mousedown - clique e segura
* mouseup - depois do clique e segura, solta o botao do mouse
* click - clique e solta rapidamente
* mouseout - mover o mouse pra fora do elemento

Event reference - MDN

**Disparando um Evento**

p/ tratar um evento - funcao/funcionalidade

## Função JS

função anônima (ñ tem nome)
```
function {
    bloco
}
```
p/ que o metodo possa funcionar precisa de um nome p/ funcoes de evento (geralmente acoes que podemos fzr)

```
function nomeAcao() {
    bloco
}
```
pode-se passar, opcionalmente, 1 ou + parametros

**Configurando Eventos**

na parte HTML
```
<div id="" onevento="nomeAcao()"
	   onclick=""
	   onmouseenter=""
	   onmouseover=""
```

```
function nomeAcao() {
    // só vai ser executado ao ser chamado, que por sua vez vai ocorrer quando o evento for acionado
}
```

diretamente no JS
```
<div id="nome">

var = getElement.....
var.addEventListener('click', clicar)
                     'evento', function
```
dispara eventos utilizando ouvidores que ficam prestando atenção dentro do próprio js

códigos/linhas que só vão ser executadas quando o evento ocorrer. {} de linhas - bloco

antes - carregava a página e os códigos eram executados automaticamente

agora - um código só vai ser ocorrer quando clicar dentro da div, por ex.

só executada quando um determinado evento ocorrer

* Quando algo n rodar, pode-se verificar qual foi o erro no console do navegador, que detecta erros utilizando o dev tools, clicando no simbolo de circulo vermelho com um numero dentro
* ```<input ....> var.value``` - valor da caixa, que foi digitado na caixa de texto
* caixa de texto do html vai ser sempre em formato de texto
* ```var.innerHTML = `~~~~ ${} ~~~~~` ```  escreve