# Variáveis Compostas

**Variável Composta/Array/Vetor**

variáveis simples - só conseguem armazenar um valor por vez

compostas - capazes de armazenar vários valores em uma mesma estrutura. ñ perde os valores anteriores p/ guardar os novos. guarda vários valores, identificados por uma chave/índice, um identificador numérico
sempre começa com zero

```
let num = []
let num = [5,8,4]
           0 1 2
num[3] = 6
```
especifica o índice, coloca o valor no indice. se ñ existe essa posição, ele cria

um vetor é composto de elementos, um elemento de um vetor é um par que agrupa no espaço da memória o valor colocado dentro deele e identificado por um índice
um vetor é uma variável que tem vários elementos, cada elemento é composto por seu valor e por uma chave de identificação

adicionando valor ao último índice
```
var.push(7)
```
método interno

pra saber o comprimento (qtd)
```
var.length
```
sem parênteses. é atributo, e n metodo

ordenar
```
var.sort()
```
em ordem crescente os valores

percurso em vetores
```
for () {
}
ou
for (  in  ) {

} // + simplificado nas versões + atuais. otimizado p/ vars compostas e objetos (só funciona com eles tbm)
```
mostrando com estrutura de repetição

percurso p/ exibicao de vetores
* todo array em js é um objeto

buscar valores dentro de um vetor
```
num.indexOf(7)
```
procura onde está o valor e retorna a chave onde o valor se encontra

se n tiver, retorna -1, que significa que n encontrou nenhuma ocorrência
