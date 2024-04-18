# Introdução
**Fundamentos Principais da Linguagem**

## Conceito Client x Server
Dispositivos como computadores e celulares estão do lado do cliente. Precisam de dados, dados estes disponibilizados por servidores, máquinas de alta performance que fornecerão tais dados que serão acessados.

Para acessar - navegadores.
Uma URL é digitada, a infraestrutura da internet responde exatamente para qual servidor será desviado, com uma série de tecnologias envolvidas.

O servidor é uma máquina com sistema operacional, pastas com arquivos, diretórios internos. Usuário solicita para o servidor um determinado arquivo, como uma foto, texto, vídeo ou documento HTML, que por sua vez envia uma cópia que o navegador web irá trabalhar para gerar o efeito visual, gerar o site propriamente dito.

De uma maneira bem resumida é assim que a web funciona. Tecnologias para clientes querem um bando de arquivos que serão enviados pelas tecnologias do seu lado, para servidores com suas tecnologias próprias do seu lado também.

JS surgiu como uma tecnologia para clientes, client-side, mas que hoje também funciona para servidores.

## Website
Tecnologias Relacionadas

Grande maioria das vezes são compostos por três tecnologias no lado do cliente, que rodam no dispositivo do cliente. Servidores por sua vez possuem várias. Base para desenvolvimento de sites (comparação com um jornal com jornalista, designer e programador):

**HTML - conteúdo** (por si só não se vende, precisa de uma visão atraente), prover textos, imagens, vídeos. Textos e marcações que existem nesses textos. Uma marca específica para transformar um texto em um título, que será um pouco maior do restante dos textos. Inserir uma imagem, mídia. O conteúdo bem organizado e não bonito.

**CSS - estilo**, design. Cores, tamanhos e posições dos componentes, dimensionar formatos diferentes para diferentes telas. Deixar visualmente agradável. Pega os textos e deixa mais agradável.

**JS - interações**. Ao aproximar o mouse (evento) em uma imagem fazer com que apareça um texto explicativo, ao clicar expandir ela e escurecer o fundo. Grande poder, inclusive de modificar HTML e CSS. É uma linguagem de programação, ao contrário das anteriores que são tecnologias de construção de sites. (No exemplo do jornal seria a engenharia da entrega do jornal, pensar em que áreas entregar mais ou menos jornal, tratar das configurações de cada uma das coisas da entrega, a integração entre as empresas de fabricação e distribuição do jornal, segurança da entrega).

Funcionam em conjunto, peças fundamentais. Compõem a parte de cliente da grande maioria dos sites, que não conseguiriam existir sem.

## Demonstração

Com o inspecionar do Chrome, janela do devtools destacada - settings - debugger -  [x] disable js.

Pra ver como os sites se comportam. Google por exemplo, fica até com o estilo afetado, parecendo a versão antiga do site. Não há mais o autocomplete da caixa de busca (que usa outras tecnologias em conjunto, como o AJAX) e nem a rolagem infinita na página de imagens, agora fica pra passar pra próxima página com aquele contador do rodapé. Sem JS o YT fica sem os vídeos, e também sem a rolagem infinita no feed. Dependem do JS, da interação.

No console:
```
alert('Olá, mundo!')

document.body.style.background = 'black'
document.querySelector('tag#id').style.filter = 'grayscale(100%)'
document.querySelector('tag#id').style.visibility = 'hidden'
document.querySelector('tag.class').innerText = 'novo texto'
```
Assim, altera o JS que já chegou na minha máquina/dispositivo. Só pra minha máquina nesse momento o site fica alterado. Ao atualizar, pede que o servidor reenvie

---

- "JS baseado no Ecma";
- Programação não é muito fácil, mas também não é muito difícil;
- Com a prática, saber a base do JS;
- Só aprende quando pratica, digita;
- Começo não pode sair correndo, se não o tombo acaba sendo grande, e as frustrações começam a aparecer;
