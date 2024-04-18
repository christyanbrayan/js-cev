# Operadores

**Famílias de operadores**
- Aritméticos
- Atribuição
- Relacionais
- Lógicos
- Ternário

## Aritméticos
```
+ - * / % **
```
são operadores binários (de 2 operandos)

divisão real -> 5/2 = 2.5

5%2 = 1 (resto da divisão inteira)

** potência

**Precedência de Operadores**
- ```()``` muda a ordem de precedência
- ```**```
- ```* / %``` (mesma ordem. executa na ordem da esquerda pra direita)
- ```+ -```

## Atribuição

atribuição simples
```=```
(recebe)

no node ao fazer só atribuição vai retorna undefined pq ele calcula o valor mas n mostrou na tela ainda

**auto-atribuição** - a própria variável

```
n = 3
n = n +4
```
```
n = n +4 → n += 4 (simplificada)
deixa de ser um e passa a valer...
```
```+= -= *= /= **= %=```

### Incremento
```x = x + 1 → x += 1 → x++ (pós-incremento)```
aparece o valor, e se mostrar de novo aparece o novo somado. p/ aparecer direto - ```++x (pré-incremento)```

pré e pós - questão de ordem

faz + diferença na programação avançada

pós-decremento e pré-decremento também

## Relacionais
```> < >= <= == !=```
p/ toda expressão que tenha op. relacional, o resultado vai ser booleano
* ñ igual/diferente

* operações com relacionais e aritméticos, os aritméticos são feitos primeiro

**Relacionais de Identidade**

```
5 == 5 true
5 == '5' true
5 === '5' false
5 === 5 true
```

op. de identidade/igualdade restrita

testa se é idêntico: mesmo valor e tipo

## Lógicos
```!``` negação/nao

operador unário: só tem um operando
!true / false / expressao que vai retornar true ou false

`&&` conjunção/e lógico

`||` disjunção/ou lógico

também são operadores binários: dois valores lógicos um de cada lado

**Precedência Geral**
```
↓ () ** / ... todos os op. aritméticos
↓ > < == .... relacionais (n tem ordem, quem aparecer primeiro, leitura da esq. p/ direita →)
↓ lógicos (na ordem:)
↓ !
↓ &&
↓ ||
```

## Ternário
```
? :
teste ? true : false
3 partes, junta 3 operadores
blocos
```

```
var res = x % 2 == 0 ? 5: 9
```
se x = 8, res = 5

sempre último a ser feito na precedência