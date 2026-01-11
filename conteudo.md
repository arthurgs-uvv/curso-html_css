# HTML – Estrutura e Elementos

## Estrutura Básica de um Documento HTML
```
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Título da página</title>
</head>
<body>
</body>
</html>
```
Uso: estrutura mínima obrigatória de qualquer página HTML.

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


# CSS – Formas de Aplicação

## CSS Inline
```
<p style="color: blue;">Texto</p>
```
Uso: estilização pontual (evitar sempre que possível).

## CSS Interno
```
<style>
  body {
    background-color: lightgray;
  }
</style>
```
Uso: páginas únicas ou estilos específicos.

## CSS Externo (Recomendado)
```
<link rel="stylesheet" href="style.css">

body {
  font-family: Arial, sans-serif;
}
```
Uso: reutilização, organização e manutenção.

## Seletores CSS
```
p { }          /* Seletor de tag */
#id { }        /* Seletor por ID */
.classe { }    /* Seletor por classe */

Diferença entre ID e Class
id → único
class → reutilizável
```

## Box Model (Modelo de Caixa)
```
div {
  width: 300px;
  padding: 10px;
  margin: auto;
  border: 1px solid black;
}
```
### Propriedades
width: largura  
padding: espaço interno  
margin: espaço externo  
border: borda  

## Display e Tipos de Elementos
```
display: block;
display: inline;
display: inline-block;
```
Block: ocupa linha inteira (div, p, section)  
Inline: ocupa apenas o conteúdo (span, a)  
Inline-block: mistura dos dois  

## Cores no CSS
```
Cores Nomeadas
color: blue;

RGB
color: rgb(255, 0, 0);

Hexadecimal
color: #ff0000;

HSL
color: hsl(120, 100%, 50%);
```

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

## Classes, IDs, DIV e SPAN
```
<div class="container">
  <span class="destaque">Texto</span>
</div>

.container { }
.destaque { }
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
