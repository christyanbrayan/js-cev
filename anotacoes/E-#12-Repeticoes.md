# Repetições

* importante entender condição p/ poder fazer uma repetição

a tarefa na hora de programar tem como objetivo conseguir escrever os programas para que parte de um ponto A ao B

pra conseguir atingir os objetivos existem várias formas, assim, existem as estruturas de controle

- sequência
	- +simples
	- executando tarefas sequencialmente até chegar ao objetivo
	- mas nem tudo na programação é feita de uma sequência, as vezes é necessário um teste lógico, há desvios, possibilidades
- condições
	- teste lógico que de acordo com dois valores, v ou f, pode ter duas possibilidades de executar tarefas específicas
- repetições

**Repetições/Laços/Iterações**

começa como as condições. testa uma expressão com uma condição, que vai ter duas possibilidades de resultado: verdadeiro ou falso. Se verdadeiro, não vai seguir p/ proximo bloco, ele vai voltar, fzr um looping, um laço, uma repetição. aí volta, testa de novo, se verdadeiro repete, e continua repetindo enquanto for verdadeiro. quando for falso o laço é quebrado e segue o fluxo natural

laço + simples que existe: quando escolhe as vezes que uma coisa vai acontecer

## Estrutura de repetição com teste lógico no início
```
while (condicao) {

}
```
faz o teste, se for v faz o bloco

testa, executa e faz looping

```
var contador = 1
while (contador <= 6) {
    console.log(`${contador}`)
    c++
}
```
quando escolhe quantas vezes uma coisa vai acontecer

## Estrutura de repetição com teste lógico no final
```
do {

} while (condicao)
```
enquanto for v

```
var contador = 1
do {
  console.log(`${c}`)
  c++
} while (c <= 6)
```

* usar + inteligência do que força bruta

## Estrutura de repetição com variável de controle, inicialização, um teste lógico e o incremento
```
for (inicio; teste; incremento) {

}
```
(var c = 1; c <= 10; c++)

```
var c=1
while (c<=10) {
    c++
}

for (var c=1; c<=10; c++) {
    console.log(c)
}
```

* mesma funcionalidade do while
* preferencial na grande maioria das vezes em que se sabe os limites das execuções

representação visual com fluxograma. trabalhamos com comandos escritos em uma linguagem

"pode misturar estruturas dentro da outra, nao existe limitacao nenhuma pra programacao"

**Modo de Depuração do VSCode**

Ver passo a passo da execução do código

VSCode - Debug - Start Debugging - vai abrir uma área na esquerda e em baixo o Debug Console

Aí pode-se colocar pontos de parada/break points no código (clicando ao lado dos números das linhas, aí vai marcar uma linha)

Em Watch pode adicionar uma variável para ser monitorada

Executa no play verde
