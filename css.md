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
p { }
#id { }
.classe { }
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

## Box Model (Modelo de Caixa)
width  
height  
padding  
margin  
border  

Funcionalidade:
Todo elemento HTML é uma caixa, composta por:
Conteúdo  
Padding (espaço interno)  
Border (borda)  
Margin (espaço externo)  
O Box Model controla tamanho, espaçamento e organização visual.

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

## Flexbox
### Container Flex
```
display: flex;
justify-content;
align-items;
flex-direction;
```
Funcionalidade:
Cria layouts flexíveis, responsivos e alinhados, facilitando:
Centralização
Distribuição de espaço
Ajuste automático de elementos

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

## Cores
```
color;
background-color;
```
Funcionalidade:
Define cores de texto e fundo, influenciando:
Identidade visual
Acessibilidade
Experiência do usuário

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

## Cursor
`cursor: pointer;`
Funcionalidade:
Indica visualmente interatividade ao usuário.

## Opacidade e Filtros
```
opacity;
filter;
```
Funcionalidade:
Cria efeitos visuais como transparência, desfoque e escala de cinza.

## Media Queries
`@media`
Funcionalidade:
Permite criar layouts responsivos, adaptando o site a diferentes telas.

## Variáveis CSS
```
--variavel
var()
```
Funcionalidade:
Centraliza valores reutilizáveis, facilitando manutenção e padronização.

## Reset CSS
```
* {
  margin: 0;
  padding: 0;
}
```
Funcionalidade:
Remove estilos padrões do navegador para garantir consistência visual.
