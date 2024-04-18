# Funções

JS funciona sob o paradigma funcional, funciona como uma linguagem funcional

toda função:

* precisa de uma chamada, que pode ser automatizada
* pode ter, ou não, um conjunto de parâmetros
* tem uma ação envolvida
* pode, ou não, ter um retorno

**Funções**

são ações executadas assim que são chamadas, ou em decorrência de algum evento

pode receber parâmetros e retornar um resultado
```
function acao(params) {
}
acao(5)

function acao(params) {
    return
} 
acao(5)
```
params - parametro formal. 5 - é um parâmetro real, mas essa nomenclatura é só formalidades

pode ter + de um return dentro de um function, dentro de ifs por exemplo, só precisa que apenas um deles seja executado (dentro de um)

se a função tem return pra mostrar o resultado da função precisa atribuir a chamada da função a uma variável e mostrar a var, ou mostrar direto a chamada da função num console.log por ex

soma(x, y) mas se n passar um valor, ficaria undefined em um. qualquer valor somado com undefined - Nan (not a number)

se n passar, pode fzr com que considere:

(x = 0, n2=0) parametros já pré-definidos/parâmetros opcionais

```
function soma(n1=0, n2=0) {
```

tem como jogar uma funcao dentro dentro de uma var
```
let v = function(x) {
    return x
}

console.log(v(5))
```
passou pra uma variável um parâmetro e ele conseguiu executar uma função

há também a sintaxe da arrow function (funcoes arrow/flecha =>)

maneira recursiva, recursividade

uma recursão acontece quando uma funcao chama ela mesma

cria uma funcao e dentro dela possui uma chamada p ela mesma

ex do fatorial
```
function fatorial(n) {
  if (n == 1) {
    return 1
  } else {
    return n * fatorial(n-1)
  }
}
```

* "faz o içamento" function em cima ou em baixo