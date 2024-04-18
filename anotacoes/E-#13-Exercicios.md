# Exercícios

* php aproveita mais o name dos inputs

var ou let só tem diferença de escopo. let - só vai ser local, não vai existir fora do bloco

validação simples se n foi preenchido:
```
if (input.value.length == 0 || outroinput.value.length == 0 || outro.value.length == 0) {}
```

se o passo for igual a zero, mostra um alerta que vai considerar como um e faz passo receber 1 e faz a contagem

* nunca vai programar de uma vez só, "escrever o programa, ele vai rodar de primeira"
* ```<input type="number">``` vai ser string, precisa converter com Number()
* unicode.org/emoji/charts/full-emoji-list.html - u+12... ->  \u{12...} (interpolado entre ``)
* js tenta n mostrar erro p/ pagina, pq considera que está no navegador, online, então não vai mostrar erro pro usuário na execução do script. pode aparecer no console

adicionar elementos dentro de um controle html

adicionar um elemento a um select (ex da tabuada)

p/ criar elemento, qualquer que seja, dentro de js:
```
var  = document.createElement('option')
var.text = '~~~~~' // parte de dentro do option
select.appendChild(var) // adicionar um elemento filho a var q armazena o select. depois de adicionar em cima, cria aqui
```
* ```<select ..... size="10">``` p/ ficar grande e ñ precisar usar o scroll

antes tava q ao fazer de novo, mais uma tabuada, ia mostrando a que pediu junto da anterior.

p/ 'limpar': 
```
var.innerHTML = ''
```
vazio

```
option.value = '1' // adiciona ao value do form - <option value="1">. util no php
```

* aprender a programar - praticar constantemente, ter o maior número de fontes de consulta

* php - linguagem server-side