# Variáveis e Tipos Primitivos

## Comentários
Simbologia, símbolos de comentários
```
// em uma única linha
```

```
/*
    + de uma linha de código
*/
```
quem comenta bem os seus códigos, mantém ele bem documentado. ajuda a lembrar depois de mt tempo tbm.
p/ depuração tbm. ver como que o programa está funcionando, pra ignorar um comando
ou mesmo p explicar p/ que serve um comando

## Variáveis
guardar dados p/ usar mais p/ frente, na memória do computador
= op. de atribuição. lê-se "receber"

var, let ou const, nome (indentificador), = e valor

**var ou let**
```
var name = '~~~'
var name = null
```

**Regras pra identificador**

começo com _, letra ou $, sem número
letras ou números
acentos e símbolos (de PI por exemplo)
sem espaços entre as palavras
sem palavras reservadas (que o js usa como comando)
maiúsculas e minúsculas fazem diferença
nomes coerentes

## Tipos Primitivos (Data Types) Primordiais

**string**

cadeia de caracteres. pra armazenar um cpf por ex
```
'string'
"string"
`string`
```

**number**

n diferencia, a priori, inteiros e reais (com ponto flutuante)
- dois valores internos: Infinity e NaN (not a number)

**boolean**

valor booleano, true ou false

tipos primitivos primordias - number, string e boolean

**Outros**
- dois valores internos do tipo number: Infinity e NaN (not a number)
- null (sem nada dentro, nulo, considerado objetct tbm)
- undefined
- object (js é ling orientada a objeto)
	- tipo interno que é object - array, o vetor
- function (é tbm considerado um tipo primitivo no js, que tbm funciona no paradigma funcional)

### typeof
"tipo de"
```
typeof nomeVar
typeof 6
```
var/valor (quando é valor direto e n dentro de uma var, js chama de numero literal)

retorna o tipo

```
// typeof 6
// 'number'

// typeof 6.5
// 'number'

// typeof "string"
// 'string'

// typeof []
// typeof {}
// 'object'

// typeof function(){}
// 'function'

// typeof undefined
//'undefined'

// typeof NaN
// typeof Infinity
// 'number'

// typeof null
// 'object'
```

na var n define o tipo primitivo, essa var pode aumentar e diminuir conforme programa vai rodando (tipagem dinâmica)

### Node no VSCode:
ctrl + shift + crase p abrir terminal no VSCode
```
> node
> ctrl + l
> .exit
```
+ terminais abertos fica lento, e só são fechados mesmo com o .exit