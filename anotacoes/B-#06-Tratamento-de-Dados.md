# Tratamento de Dados
## Manipulação de dados
```
var nome = window.prompt('Qual é o seu nome?')
```
jogar o resultado da execução do comando prompt dentro de uma var

### Concatenação
```
window.alert('Ola, ' + nome + '!')
```
+ soma e concatena (se forem duas strings)
qualquer valor digitado no prompt é caractere, para fazer a soma deve fazer a conversão para o tipo number (se não vai concatenar os dois valores):

## Conversões de Tipos de Dados
```
Number.parseInt(n) 
Number.parseFloat(n)
```
parse - converter, parsear

float - números com ponto decimal, ponto flutuante
- JS é case sensitive
não precisa do Number.

ou apenas Number() que faz a conversão p/ tipo definido
```
Number(window.prompt('Digite um numero: '))
```
prompt por padrão retorna string, então converte pra fazer operação
com Number() é convertido pro tipo que ele recebe, de acordo com o que recebe. nas funções parse é especificado, força p/ converter p/ esse tipo
as vezes pode precisar no momento que seja realmente float, por ex, ai usa o parse

```
String(n) 
n.toString()
```

(number + number) adição
(string + string) concatenação

### Formatando Strings
Template strings, formatador de strings

**Interpolação**
```
`texto caracteres entre crases ${nomevar} com placeholder`

// no lugar de

"O nome é" + name + "e idade é" + age
```
`` delimita as chamadas template strings
${} chamado placeholder

quantos caracteres tem
```
nome.length
```
objeto.atributo
.atributo
.metodo()

passar pra maiúsculas e minúsculas
```
s.toUpperCase() // maiusc. 
s.toLowerCase() // minusc.
```

comandos de saída
```
document.write('') escreve na tela 
document.writeln('') escreve e pula p linha de baixo
```

exemplo de uso:
```
document.write(`var tem ${s.length} letras`)
```

aceita html dentro do write

### Formatando Números
```
n2.toFixed(2) 2 casas 
n2.toFixed(2).replace('.' , ',') trocar um p/ outro
```

formatando valor pra moeda real:
```
n1.toLocaleString('pt-BR', {style: 'currency', currency: 'BRL'})
```
string localizada por parte do mundo, manda localizar string em pt-br, entre {as configuracoes, atributos, um objeto em js} e atributos. BRL, USD, EURL
currency - mostrar em valor monetario

no node inverte e aparece por ex US$ 1,545.50, mas no navegador aparece certo

VSCode

ctrc c ctrl v no arquivo no vscode p duplicar ex ex001 p ex002 com mesmo código

* var let e const - diferenças de escopo

**strings**

'' ou "" tanto faz

`` p interpolação