# HTML – Estrutura e Elementos

## Tags Semânticas de Estrutura
```
<header>     <!-- Cabeçalho -->
<nav>        <!-- Menu de navegação -->
<main>       <!-- Conteúdo principal -->
<section>    <!-- Seção de conteúdo -->
<article>    <!-- Conteúdo independente -->
<aside>      <!-- Conteúdo lateral -->
<footer>     <!-- Rodapé -->
```
Uso: organização semântica do layout da página.

## Tags de Texto
```
<h1> a <h6>   <!-- Títulos -->
<p>          <!-- Parágrafo -->
<br>         <!-- Quebra de linha -->
<hr>         <!-- Linha horizontal -->
<strong>     <!-- Texto forte -->
<em>         <!-- Ênfase -->
<span>       <!-- Container inline -->
```
Uso: formatação e organização textual.

## Links e Imagens
```
Links
<a href="https://exemplo.com">Link</a>

Imagens
<img src="imagem.jpg" alt="Descrição da imagem">
```
Uso: navegação e exibição de imagens.

## Áudio em HTML5
```
<audio controls preload="metadata" autoplay loop>
  <source src="audio.mp3" type="audio/mpeg">
</audio>
``` 

### Principais Atributos
controls: exibe controles  
autoplay: inicia automaticamente  
loop: reprodução contínua  
preload: controle de carregamento  


## Vídeo em HTML5
```
<video width="600" poster="capa.jpg" controls autoplay>
  <source src="video.mp4" type="video/mp4">
</video>
```
### Atributos Importantes
width: largura do vídeo  
poster: imagem de capa  
controls: controles visíveis  
autoplay: reprodução automática  

## Incorporação de Vídeos Externos
```
<iframe src="https://www.youtube.com/embed/ID_DO_VIDEO"></iframe>
```
Uso: inserir vídeos do YouTube ou Vimeo sem hospedar arquivos.

////////////////////////////////////////////////////////////////

# CSS – Formas de Aplicação

## Seletores CSS
```
p { }          /* Seletor de tag */
#id { }        /* Seletor por ID */
.classe { }    /* Seletor por classe */
```

## Display e Tipos de Elementos
```
display: block;
display: inline;
display: inline-block;
```
Block: ocupa linha inteira (div, p, section)  
Inline: ocupa apenas o conteúdo (span, a)  
Inline-block: mistura dos dois  

## Gradientes
```
background-image: linear-gradient(to right, red, blue);
```
Uso: fundos estilizados.

## Tipografia no CSS
```
Fontes
font-family: Arial, Helvetica, sans-serif;

Tamanho
font-size: 1em;
font-size: 16px;

Peso e Estilo
font-weight: bold;
font-style: italic;

Shorthand
font: italic bold 2em Arial, sans-serif;
```

## Google Fonts
```
@import url('https://fonts.googleapis.com/css2?family=Open+Sans');

body {
  font-family: 'Open Sans', sans-serif;
}
```

## Pseudo-classes
```
a:hover { }
a:visited { }
a:active { }
:first-child { }
:nth-child(2) { }
```
Uso: estados especiais de elementos.

## Pseudo-elementos
```
p::before { }
p::after { }
p::first-letter { }
p::first-line { }
```
Uso: estilizar partes específicas do elemento.

## Flexbox
```
.container {
  display: flex;
  justify-content: center;
  align-items: center;
}
```
### Propriedades Comuns
display: flex  
flex-direction  
justify-content  
align-items  
flex-wrap  
Uso: layouts responsivos e alinhamento eficiente.

## Modelo de Caixas
heigth  
width
padding
border
outline
margin


## Tipos de Caixa
box-level: ocupa 100% da tela, contem quebra de linha automática (div; h1-h6; p; main; header; nav; article; aside; footer; form; video)

inline-level: ocupa o tamanho necessário, não contem quebra de linha automatica (span; a; code; small; strong; em; sup; sub; label; button; input; select)


////////////////////////////////////////////////////////////////


# COMANDOS CSS

## Estrutura Básica do CSS
```
seletor {
  propriedade: valor;
}
```
Funcionalidade:
Define qual elemento será estilizado (seletor) e como ele será apresentado (propriedades).  
O CSS funciona aplicando regras visuais aos elementos HTML.

## Seletores
### Seletores Básicos
```
#    = id
.    = class
:    = pseudo-class
::   = pseudo-element
>    = children
```
Funcionalidade:  
p → aplica estilo a todas as tags `<p>`  
#id → aplica estilo a um único elemento  
.classe → aplica estilo a vários elementos com a mesma classe  

### Seletor Universal
`* { }`
Funcionalidade:  
Seleciona todos os elementos da página, muito usado para resetar estilos padrões do navegador.

### Seletores Combinados
```
div p { }
div > p { }
div + p { }
div ~ p { }
```
Funcionalidade:  
div p → elementos dentro de outro  
div > p → filhos diretos  
div + p → próximo irmão  
div ~ p → irmãos seguintes  

Usados para controle preciso da hierarquia HTML.

## Display
```
display: block;  
display: inline;  
display: inline-block;  
display: none;  
```
Funcionalidade:
block → ocupa linha inteira  
inline → ocupa apenas o conteúdo  
inline-block → permite tamanho customizado  
none → remove o elemento da tela  
Controla como os elementos se comportam no layout.

## Visibilidade
```
visibility: hidden;
```
Funcionalidade:
Esconde o elemento sem remover o espaço ocupado, diferente do display: none.

## Posicionamento
`
position: static | relative | absolute | fixed | sticky;
`

Funcionalidade:
static → padrão  
relative → referência para posicionamento interno  
absolute → posiciona em relação ao pai  
fixed → fixa na tela    
sticky → mistura de relative + fixed  
Usado para controle avançado do layout.

## Z-Index
`z-index: 10;`
Funcionalidade:
Controla quem fica na frente de quem quando elementos se sobrepõem.

### Itens Flex
```
flex-grow;
flex-shrink;
flex-basis;
order;
```
Funcionalidade:
Define como cada item se comporta dentro do container, controlando crescimento, ordem e tamanho.

## Grid Layout
```
display: grid;
grid-template-columns;
gap;
```
Funcionalidade:
Cria layouts em linhas e colunas, ideal para páginas complexas como dashboards e galerias.

## Tipografia
```
font-family;
font-size;
font-weight;
line-height;

@import url('fontes do google';)

@font face{
  font-family:'Android';
  src: url('/') format('opentype');
  font-weight: normal;
}
```
Funcionalidade:
Controla fonte, tamanho, peso e espaçamento, impactando diretamente a legibilidade e estética.

## Texto
```
text-align;
text-transform;
text-decoration;
letter-spacing;
```
Funcionalidade:
Define formatação textual, alinhamento, capitalização e espaçamento entre letras.

## Backgrounds
```
background-image;
background-size;
background-position;
```
Funcionalidade:
Controla imagens de fundo, repetição, posição e adaptação ao elemento.

## Gradientes
```
linear-gradient();
radial-gradient();
```
Funcionalidade:
Cria transições suaves entre cores, usadas para fundos modernos e efeitos visuais.

## Bordas e Sombras
```
border;
box-shadow;
text-shadow;
```
Funcionalidade:
Bordas delimitam elementos
Sombras criam profundidade e destaque visual

## Overflow
`overflow: hidden | auto | scroll;`
Funcionalidade:
Controla o que acontece quando o conteúdo excede o tamanho da caixa.

## Listas
`list-style;` 
Funcionalidade:
Remove marcadores, personaliza listas e cria menus visuais.

## Pseudo-classes
```
:hover
:active
:focus
:nth-child()
```
Funcionalidade:
Aplica estilos baseados em ações do usuário ou posição do elemento.

## Pseudo-elementos
```
::before
::after
```
Funcionalidade:
Permitem criar elementos visuais extras sem alterar o HTML.

## Transições
`transition;`
Funcionalidade:
Cria animações suaves ao mudar propriedades (hover, foco, clique).

## Transformações
`transform: scale | rotate | translate;`
Funcionalidade:
Altera posição, rotação e tamanho sem quebrar o layout.

## Animações
```
@keyframes
animation
```
Funcionalidade:
Cria animações completas e contínuas, controlando tempo e repetição.

## Media Queries
`@media`
Funcionalidade:
Permite criar layouts responsivos, adaptando o site a diferentes telas.

## Variáveis CSS
```
--variavel
var()

:root{
  --x: y;
}
```
Funcionalidade:
Centraliza valores reutilizáveis, facilitando manutenção e padronização.

## Responsividade
```
extensão: window resizer  
min-width: 320px; //menor tela possível
max-width: 800px; //após a máxima disponível

<picture> //para imagem
  <source media="(max-width: 600px)" srcset="url-img">
  <img src="url-outra-img" alt="Exemplo">
  </picture>
```