## COMPONENTS
o que são componentes? Se visitarmos qualquer aplicação web, podemos perceber que todas utilizam os mesmos componentes graficos... componentes graficos que chamamos em ingles de web components. mas então o que exatamente são esse web components?

-avatar
-navbar
-abas dentro de uma pagina para navegar paneis diferentes
-botoes
-formularios
etc.

E quando aprendemos como criar esses componentes, bem, individualmente, o desenvolvimento front end fica bem le, porque fica facil utilizar e reutilizar esses componentes, e combinar todos eles pra criar a nossa aplicação web;

o que vamos hoje é justamente criar uma pequena biblioteca de web components;

Mas antes de começarmos a criar esse componentes eu vou passar com vcs por alguns exemplos dos principais componentes web que podem ser encontrados em algumas aplicações web como por exemplo airbnb, medium, twitter, google etc. 

Logo depois vamos começar criando alguns componentes simples, como botoes e avatars utilizando um css bem simples e a medida que caminhamos, vamos passar para componentes mais complexos que utilizam tecnicas css um pouco mais avançadas para entao criarmos componentes realmente mais avançados.

è interessante lemrbar também que existem componentes para aplicativos de celular assim como aplicativos de desktop - mas hoje nós vamos focar exclusivametne em componentes web ok? O que vamos criar hoje são os componentes que são em encontrados em aplicações web somente.

## UI components
Os web components são blocos elementares do desgins de uma aplicação web. 

## 5 to 10 components to master
a boa noticia é que não existem muitos componentes web - e se você sabe, se vc tem a sua propria biblioteca de entre 5 a 10 componentes, vc ja tem 90% do seu app design feito. e esses componentes existem para serem reutilizados - web designers costumam ganhar mto tempo ao desenvolver uma nova aplicação web utilizando e reutilizando esses componentes, porque não é preciso, necessariamente reinventar a roda toda vez que um projeto novo chega nas mãos desses designers.

## which UI components do you know?
Como já falamos existem:
-avatar
-navbar
-abas dentro de uma pagina para navegar paneis diferentes
-botoes
-formularios
-temos também os headers
- imagens

Agora vou passar com vcs por todos os componentes que vamos criar hoje.

# IMAGES
- avatar (profile pics)
- Thumbnail (borda branca e um box shadow)

## BUTTONS
- descrever cada um com css

## FORMS
Existem varios tipos de forms: sign in, sign up forms, search forms (formularios de busca)
-formulario vertical LOGIN
-formulario inline ou horizontal SEARCH
-chatbox

## TABS (abas)
-utilizados apara navegação
- letras maiusculas e com letter spacing
- aba ativa esta sublinhada
são esses pequenos detalhes q fazem o design eficiente
as abas são utilizadas para o que chamaos de navegação interna
mas existe também uma forma de navegação principal que são os navbars

## navbars
-sempre o logo do lado esquerdo
-do lado direito a foto do profile, e algumas vezes um formulario de busca
a estrutura do navbar é a seguite:
logo do lado esquerdo
profile picure, forlularios e botoes do lado direito

## Banners
esse componente passa pro usuario as informações mais importantes da pagina.
Na maioria dos landing pages vcs vão encontrar um banner. Ele tem:
-nome do produto
- o tagline
call to action que seria clicar num botao de sign up por exemplo e cadstrar seu email

## cards
utilizados para listar os produtos de uma pagina
go to airbnb e dribble

## lists
aqui essas lista parecem cartoes mas são listas, que possuem componentes ricos feita com um bom desgin

## dropdown
é uma forma de navegação que utilizamos ao clicar em um elemento: um botao, ou um avatar

## SETUP + BOILERPLATE

Talk about:
## HTML
-link para o css do bootstrap
-link para o css fontswesome
-link para o nosso proprio stylesheet
-no corpo por enquanto temos somente um H1 com uma classe do bootstrap text-center
-temos link para jquery (precisamos pq o JS do bootstrap utiliza jquery,  por isso precisamos carraegar o jquery antes de carregar o BS)
-temos o link para bootstrap javascript (porque existem componentes estaticos mas tb existem componentes dinamicos e para que esse componentes dinamicos funcionem precisamos carregar o JS do bootstrap)

## css folder
compontes is empty
style.css:
google fonts (2) aqui carregamos 2 fontes. montserrat para os headers e Open sans para o body

## EASY CSS EXAMPLES - code components
----------------------------------------
## CSS Advanced patters

## GRADIENT FILTER
Serve como filtro de uma imagem de backgroud para que o usuario consiga enxergar mehor o texto. Ele trabalha com contraste da imagem que está no background e faz o texo e os itens legiveis para o usuário.
Aqui nos trabalhamos com angulo, com inicio de uma linha e o final dessa linha assim como o inicio e o final das cores. Porque ele vai gradulamente passar de uma cor pra outra utilizando os paramos que nos passarmos distribuindo essas cores na nossa imagem de background  .

Aqui temos a sintaxe
## GRADIENT FILTER
explain
gives examples com yelow and green first

## RELATIVE POSITION / ABSOLUTE / 
## PATTERN 4 SLIDES

## RELATIVE / ABSOLUTE PATTERN card design
agora vamos aplicar essas duas técnicas, tanto do linear gradient para o background image do cartão
como as posições vamos utilizar o padrao das posições relativas e absolutas
nos vamos posicionar o cartao como relative
e vamos posicionar os intens de dentro do cartao como absolute 


BEFORE GRID 
<h2>Card Design</h2>

  <div class="card">
    <span class="card-category">POPULAR</span>
    <div class="card-description">
      <h3>Stripe</h3>
      <p>A cool payment API</p>
    </div>
      <img src="https://source.unsplash.com/random/50x50" alt="" class="avatar-small card-image">
  </div>

  add to bootstrap grid

## FLEXBOX VOCABULARY
Aqui nos temos um flex box com 3 flex items dentro - eles são os filhos do flexbox

## FLEXBOX example 1
esses elementos não podem crescer - valor 0;
esses elementos nao podem dimiuir - valor 0;
eles estao fixados em width de 200px;

## FLEXBOX example 2
aqui nos distibuimos espaços iguais entre os itens; 

## FLEXBOX example 3
aqui nos nao colocamos espaços em volta somente ENTRE os itens

## FLEXBOX example 4
com o align items podemos alinhar os itens baseados em seus axis verticais, e quando coloco center, eles ficaram alinhados verticalmente no centro independentemente de seus tamanhos

## FLEXBOX example 5
aqui temos os mesmos valores para a propriedade flex que usamos nos outros exemplos. Mas percebam que o intem do meio está bem diferente. Nesse caso nos estamos permitindo que esse item cresça. é o que chamando de flex-grow, porque permite que o intem cresça. aqui nao precisamos especificar o with, a largura, pq no caso do flexbox o item vai utilizar todo o espaço disponivel para crescer por isso colocamos auto no lugar de 200px;

## DESIGN TABS

## ITEM LIST DESIGN
descreva as listas o que tem dentro
aqui a descrição vai crescer e empurrar os outro itens