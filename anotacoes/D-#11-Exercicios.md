# Exercícios

Modelo HTML com estilo e script externos sendo chamados

* planejar a estrutura do site antes
* bom uma sombra com cor com transparência
* editor de img - exportar - salvar p/ web - PNG24 (melhor forma p web)
* ideia de cada imagem que for usar, pegar uma cor dessa imagem e usar como fundo da página html

pra executar a função quando a página carregar
```
function funcao() {}

<body onload="funcao()">
```

dinamicamente mudar qual imagem mostrar e o fundo da página de acordo com a hora do sistema
```
// hora = 19
var hora = new Date().getHours()
if (hora >= 0 && hora < 12) {
    img.src = 'fotomanha.png'
    document.body.style.background = '#e2cd9f'
} else if (hora >= 12 && hora <= 18) {
    img.src = 'fototarde.png'
    document.body.style.background = '#b9846f'
} else {
    img.src = 'fotonoite.png'
    document.body.style.background = '#515154'
}
```

ano do sistema
```
a = new Date().getFullYear()
```

teste se o input (variável que contém o querySelector que seleciona a tag input do HTML) de ano está vazio ou se o valor informado é maior do que o ano atual do sistema
```
if (input.value.length == 0 || input.value > a)
```

centralizar com CSS no JS
```
var.style.textAlign = 'center'
```

criando uma imagem de forma dinâmica na página
```
var img = document.createElement('img')
img.setAttribute('src', 'arquivo.png')
img.setAttribute('id', 'imagem')

div.appendChild(img)
```
só aparece com o appendChild, que adiciona um elemento
div no caso é uma var que armazena um getElement... que no caso é uma div vazia

* inputs radio precisam ter o mesmo name, se não fica possível marcar duas opções. colocando o mesmo name quando um for selecionado o outro é desmarcado

* formas de ensinar - aprende a mesma coisa de formas diferentes
* as vezes o aluno ñ procura, ai o prof tbm fica desmotivado
* didática incomparável
* depende do esforço

* comentário do YT: A gente para de progredir quando acha que sabe tudo

---

.getFullYear() - ano completo com os 4 dígitos

.value.length == 0 - ver se a caixa de texto não está preenchida

.style.textAlign = 'center' - centralizar no js, sem precisar ir no css

var img = document.createElement('img') | img.setAttribute('id', 'foto') - cria a tag e altera o seu id

.appendChild(img) - adiciona um conteudo/elemento