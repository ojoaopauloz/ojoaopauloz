<!DOCTYPE html>
<html>

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>AluraBooks</title>
  <link rel="stylesheet" href="reset.css">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.css" />
  <link rel="stylesheet" href="styles.css">
</head>

<body>
  <header class="cabeçalho">
    <div class="container">
      <input type="checkbox" id="menu" class="container__botao">
      <label for="menu">
        <span class="cabeçalho__menu-hamburguer container__imagem"></span>
      </label>
      <ul class="lista-menu">
        <li class="lista-menu__titulo">Categorias</li>
        <li class="lista-menu__item">
          <a href="#" class="lista-menu__link">Programação</a>
        </li>
        <li class="lista-menu__item">
          <a href="#" class="lista-menu__link">Front-end</a>
        </li>
        <li class="lista-menu__item">
          <a href="#" class="lista-menu__link">Infraestrutura</a>
        </li>
        <li class="lista-menu__item">
          <a href="#" class="lista-menu__link">Business</a>
        </li>
        <li class="lista-menu__item">
          <a href="#" class="lista-menu__link">Design & UX</a>
        </li>
      </ul>
      <img src="img/Logo.svg" alt="Logo da Alurabooks" class="container__imagem">
    </div>
    <div class="container">
      <a href="#"><img src="img/Favoritos.svg" alt="Meus favoritos" class="container__imagem"></a>
      <a href="#"><img src="img/Compras.svg" alt="Carrinhos de compras" class="container__imagem"></a>
      <a href="#"><img src="img/Usuario.svg" alt="Meu perfil" class="container__imagem"></a>
    </div>
  </header>

  <section class="banner">
    <h2 class="banner__titulo">Já sabe por onde começar?</h2>
    <p class="banner__texto">Encontre em nossa estante o que precisa para seu desenvolvimento!</p>
    <input type="search" class="banner__pesquisa" placeholder="Qual será sua próxima leitura?">
  </section>

  <section class="carrossel">
    <h2 class="carrossel__titulo">Novos lançamentos</h2>
    <!-- Slider main container -->
    <div class="swiper">
      <!-- Additional required wrapper -->
      <div class="swiper-wrapper">
        <!-- Slides -->
        <div class="swiper-slide"><img src="img/Apachekafka.svg"
            alt="Livro sobre apache kafka e spring boot da alura books"></div>
        <div class="swiper-slide"><img src="img/Liderança.svg"
            alt="Livro sobre liderança em design design da alura books"></div>
        <div class="swiper-slide"><img src="img/Javascript.svg" alt="Livro sobre javascript assertivo da alura books">
        </div>
        <div class="swiper-slide">
          <img src="img/Guia Front-end.svg" alt="Livro Guia front end" />
        </div>
        <div class="swiper-slide">
          <img src="img/Portugol.svg" alt="Livro sobre portugol" />
        </div>
        <div class="swiper-slide">
          <img src="img/Acessibilidade.svg" alt="Livro sobre acessibilidade" />
        </div>

        <!-- If we need navigation buttons -->
        <div class="swiper-button-prev"></div>
        <div class="swiper-button-next"></div>
      </div>

    </div>

  </section>

  <script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>
  <script>
    const swiper = new Swiper(".swiper", {
      spaceBetween: 10,
      slidesPerView: 3,
      pagination: {
        el: ".swiper-pagination",
        type: "bullets",
      },
    });
  </script>
</body>

</html>
/* http://meyerweb.com/eric/tools/css/reset/ 
   v2.0 | 20110126
   License: none (public domain)
*/

html,
body,
div,
span,
applet,
object,
iframe,
h1,
h2,
h3,
h4,
h5,
h6,
p,
blockquote,
pre,
a,
abbr,
acronym,
address,
big,
cite,
code,
del,
dfn,
em,
img,
ins,
kbd,
q,
s,
samp,
small,
strike,
strong,
sub,
sup,
tt,
var,
b,
u,
i,
center,
dl,
dt,
dd,
ol,
ul,
li,
fieldset,
form,
label,
legend,
table,
caption,
tbody,
tfoot,
thead,
tr,
th,
td,
article,
aside,
canvas,
details,
embed,
figure,
figcaption,
footer,
header,
hgroup,
menu,
nav,
output,
ruby,
section,
summary,
time,
mark,
audio,
video {
    margin: 0;
    padding: 0;
    border: 0;
    font-size: 100%;
    font: inherit;
    vertical-align: baseline;
}

/* HTML5 display-role reset for older browsers */
article,
aside,
details,
figcaption,
figure,
footer,
header,
hgroup,
menu,
nav,
section {
    display: block;
}

body {
    line-height: 1;
}

ol,
ul {
    list-style: none;
}

blockquote,
q {
    quotes: none;
}

blockquote:before,
blockquote:after,
q:before,
q:after {
    content: '';
    content: none;
}

table {
    border-collapse: collapse;
    border-spacing: 0;
}
@import url("styles/header.css");
@import url("styles/banner.css");
@import url("styles/carrossel.css");

:root {
    --cor-de-fundo: #EBECEE;
    --branco: #FFFFFF;
    --laranja: #EB9B00;
    --azul-degrade: linear-gradient(97.54deg, #002F52 35.49%, #326589 165.37%);
    --fonte-principal: "Poppins";
}

body {
    background-color: var(--cor-de-fundo);
    font-family: var(--fonte-principal);
    font-size: 16px;
    font-weight: 400;
}
