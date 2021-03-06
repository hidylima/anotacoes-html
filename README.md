# Categorias de conteúdo 
- Cada elemento HTML é membro de uma ou mais categorias de conteúdo.  
Essas categorias agrupam elementos que contém características em  
comum
- Tipos de categorias de conteúdo: 
  - Categorias de conteúdo principal, que descrevem regras comuns  
  de conteúdos compartilhadas entre muitos elementos
    - Metadata content: elementos que pertencem a esta categoria  
    modificam a apresentação ou o comportamento do resto do  
    documento, seta links para outros documentos ou transporta  
    outras informações. 
      - Elementos: 
        - `<base>`
        - `<link>`
        - `<meta>`
        - `<noscript>`
        - `<script>`
        - `<style>`
        - `<title>`
    - Flow content: Seus elementos contém, tipicamente, texto ou  
    conteúdo inbutido
      - Elementos: 
        - `<a>`
        - `<abbr>`
        - `<address>`
        - `<article>`
        - `<aside>`
        - `<audio>`
        - `<b>`
        - `<bdo>`
        - `<bdi>`
        - `<blockquote>`
        - `<br>`
        - `<button>`
        - `<canvas>`
        - `<cite>`
        - `<code>`
        - `<data>`
        - `<datalist>`
        - `<del>`
        - `<details>`
        - `<dfn>`
        - `<div>`
        - `<dl>`
        - `<em>`
        - `<embed>`
        - `<fieldset>`
        - `<figure>`
        - `<footer>`
        - `<form>`
        - `<h1>`
        - `<h2>`
        - `<h3>`
        - `<h4>`
        - `<h5>`
        - `<h6>`
        - `<header>`
        - `<hgroup>`
        - `<hr>`
        - `<i>`
        - `<iframe>`
        - `<img>`
        - `<input>`
        - `<ins>`
        - `<kbd>`
        - `<label>`
        - `<main>`
        - `<map>`
        - `<mark>`
        - `<math>`
        - `<menu>`
        - `<meter>`
        - `<nav>`
        - `<noscript>`
        - `<object>`
        - `<ol>`
        - `<output>`
        - `<p>`
        - `<pre>`
        - `<progress>`
        - `<q>`
        - `<ruby>`
        - `<s>`
        - `<samp>`
        - `<script>`
        - `<section>`
        - `<select>`
        - `<small>`
        - `<span>`
        - `<strong>`
        - `<sub>`
        - `<sup>`
        - `<svg>`
        - `<table>`
        - `<template>`
        - `<textarea>`
        - `<time>`
        - `<ul>`
        - `<var>`
        - `<video>`
        - `<wbr> `
        - e texto.
       - Alguns outros elementos que pertencem a esta categoria,  
       apenas se uma condição específica for realizada: 
         - `<area>`, se for um descendente de um elemento `<map>`
         - `<link>`, se o atributo `itemprop` estiver presente
         - `<meta>`, se o atributo `itemprop` estiver presente
         - `<style>`, se o atributo `scoped` estiver presente
    - Sectioning Content
      - Elementos que criam uma section no esboço atual, que  
      definem escopo dos elementos `<header>`, `<footer>` e  
      heading content.
        - Elementos: 
          - `<article>`
          - `<aside>`
          - `<nav>`
          - `<section>`
      - Não confundir esse modelo de conteúdo com a categoria  
      sectioning root, que isola seu conteúdo do esboço regular 
    - Heading content 
      - Define o título de uma seção, se marcado por um elemento  
      sectioning content, ou implicitamente definido pelo próprio  
      heading content
        - Elementos: 
          - `<h1>`
          - `<h2>`
          - `<h3>`
          - `<h4>`
          - `<h5>`
          - `<h6>`
          - `<hgroup>`
    - Phrasing content 
      - Define o texto e a marcação que ele contém 
        - Elementos: 
          - `<abbr>`
          - `<audio>`
          - `<b>`
          - `<bdo>`
          - `<br>`
          - `<button>`
          - `<canvas>`
          - `<cite>`
          - `<code>`
          - `<data>`
          - `<datalist>`
          - `<dfn>`
          - `<em>`
          - `<embed>`
          - `<i>`
          - `<iframe>`
          - `<img>`
          - `<input>`
          - `<kbd>`
          - `<label>`
          - `<mark>`
          - `<math>`
          - `<meter>`
          - `<noscript>`
          - `<object>`
          - `<output>`
          - `<progress>`
          - `<q>`
          - `<ruby>`
          - `<samp>`
          - `<script>`
          - `<select>`
          - `<small>`
          - `<span>`
          - `<strong>`
          - `<sub>`
          - `<sup>`
          - `<svg>`
          - `<textarea>`
          - `<time>`
          - `<var>`
          - `<video>`
          - `<wbr> `
          - E texto plano que não consista em apenas em caracteres de  
          espaço em branco 
        - Alguns outros elementos que pertencem a esta categoria,  
        apenas se uma condição específica for realizada: 
          - `<a>`, se contém apenas um phrazing content
          - `<area>`, se for descendente de um elemento `<map>`
          - `<del>`, se contém apenas um phrazing content
          - `<ins>`, se contém apenas um phrazing content
          - `<link>`, se o atributo `itemprop` estiver presente
          - `<map>`, se contém apenas um phrazing content
          - `<meta>`, se o atributo `itemprop` estiver presente
  - Categoria relacionada à formulário, que descreve regras em 
  comum para seus elementos 
  - Categoria de conteúdo específico, que descreve raras categorias  
  compartilhadas apenas por alguns elementos, às vezes em apenas um  
  contexto específico 

![content_categories_venn](https://user-images.githubusercontent.com/29297788/43872422-0234a7da-9b58-11e8-9465-d892a224cc87.png)

# `itemprop`
- Utilizado para adicionar propriedades a um item. 
- Todo elemento HTML pode ter este atributo especificado 
- Consiste em um par de nome e valor 
- Cada par de nome e valor é chamado de propriedade 
- Um grupo de uma ou mais propriedades forma um item 
- Os valores das propriedades são ou um texto ou uma URL  
e pode ser associadas a uma grande variedade de elementos  
incluindo:
  - `<audio>`
  - `<embed>`
  - `<iframe>`
  - `<img>`
  - `<link>`
  - `<object>`
  - `<source>`
  - `<track>`
  - `<video>`

```html
  <div itemscope itemtype="http://schema.org/Movie">
    <h1 itemprop="name">Avatar</h1>
    <span>Director:
      <span itemprop="director">James Cameron</span>
      <span>(born August 16, 1954)</span>
      <span itemprop="genre">Science Fiction</span>
      <a href="../movies/avatar-theatrical-trailer.html" itemprop="trailer">Trailer</a>
  </div>
```

![itemprop html hypertext markup language mdn](https://user-images.githubusercontent.com/29297788/43873784-737f1a3c-9b5e-11e8-839d-516a3c94f0ba.png)

# Anatomia de um elemento html 
![grumpy-cat-small](https://user-images.githubusercontent.com/29297788/43359652-1c286ff8-927c-11e8-97cf-d101772ccab9.png)

# Atributos de elementos HTML
![grumpy-cat-attribute-small](https://user-images.githubusercontent.com/29297788/43359655-40a23436-927c-11e8-9e5e-08ec1d87fda3.png)
- O valor do atributo é especificado entre as aspas duplas 

# Atributos booleanos 
- São atributos sem valores 
- Podem ter somente um valor, que geralmente é o mesmo nome  
do atributo: `disabled="disabled"`

# Conteúdo de fluxo / flow content 
- Elementos que tipicamente **contém** texto ou conteúdo imbutido 
  - `<a>`
  - `<abbr>`
  - `<address>`
  - `<article>`
  - `<aside>`
  - `<audio>`
  - `<b>`
  - `<bdo>`
  - `<bdi>`
  - `<blockquote>`
  - `<br>`
  - `<button>`
  - `<canvas>`
  - `<cite>`
  - `<code>`
  - `<data>`
  - `<datalist>`
  - `<del>`
  - `<details>`
  - `<dfn>`
  - `<div>`
  - `<dl>`
  - `<em>`
  - `<embed>`
  - `<fieldset>`
  - `<figure>`
  - `<footer>`
  - `<form>`
  - `<h1>`
  - `<h2>`
  - `<h3>`
  - `<h4>`
  - `<h5>`
  - `<h6>`
  - `<header>`
  - `<hgroup>`
  - `<hr>`
  - `<i>`
  - `<iframe>`
  - `<img>`
  - `<input>`
  - `<ins>`
  - `<kbd>`
  - `<label>`
  - `<main>`
  - `<map>`
  - `<mark>`
  - `<math>`
  - `<menu>`
  - `<meter>`
  - `<nav>`
  - `<noscript>`
  - `<object>`
  - `<ol>`
  - `<output>`
  - `<p>`
  - `<pre>`
  - `<progress>`
  - `<q>`
  - `<ruby>`
  - `<s>`
  - `<samp>`
  - `<script>`
  - `<section>`
  - `<select>`
  - `<small>`
  - `<span>`
  - `<strong>`
  - `<sub>`
  - `<sup>`
  - `<svg>`
  - `<table>`
  - `<template>`
  - `<textarea>`
  - `<time>`
  - `<ul>`
  - `<var>`
  - `<video>`
  - `<wbr>`

- Alguns outros elementos pertencem a essa categoria, mas somente se uma condição específica é realizada:
  - `<area>`, se for um descendente de um elemento `<map>`
  - `<link>`, se o atributo itemprop estiver presente
  - `<meta>`, se o atributo itemprop estiver presente
  - `<style>`, se o atributo scoped estiver presente

# Phrasing content / conteúdo fraseado 
- Elementos que definem o texto e a marcação que ele contém 
  - Séries desse tipo de elemento compõem parágrafos 
- Elementos
  - `<abbr>`
  - `<audio>`
  - `<b>`
  - `<bdo>`
  - `<br>`
  - `<button>`
  - `<canvas>`
  - `<cite>`
  - `<code>`
  - `<datalist>`
  - `<dfn>`
  - `<em>`
  - `<embed>`
  - `<i>`
  - `<iframe>`
  - `<img>`
  - `<input>`
  - `<kbd>`
  - `<label>`
  - `<mark>`
  - `<math>`
  - `<meter>`
  - `<noscript>`
  - `<object>`
  - `<output>`
  - `<progress>`
  - `<q>`
  - `<ruby>`
  - `<samp>`
  - `<script>`
  - `<select>`
  - `<small>`
  - `<span>`
  - `<strong>`
  - `<sub>`
  - `<sup>`
  - `<svg>`
  - `<textarea>`
  - `<time>`
  - `<var>`
  - `<video>`
  - `<wbr>`
- Alguns outros elementos pertencem a essa categoria, mas somente se uma condição específica é realizada:
  - `<a>`, se contém somente conteúdo fraseado
  - `<area>`, se for um descendente de um elemento `<map>`
  - `<del>`, se contém somente conteúdo fraseado
  - `<ins>`, se contém somente conteúdo fraseado
  - `<link>`, se o atributo itemprop estiver presente
  - `<map>`, se contém somente conteúdo fraseado
  - `<meta>`, se o atributo itemprop estiver presente

# `<!DOCTYPE html>`
- Declarada no topo de documentos HTML
- Todos os outros elementos devem ser descendentes dele 
- Garante que o browser faça um esforço na tentativa de seguir  
as especificações relevantes, em vez de usar um modo de  
renderização diferente e que seja incompatível com algumas  
especificações 
- Deixa o navegador ciente em que versão HTML está o arquivo  
(HTML5)

# `<html>`
- Envolve todo o conteúdo da página 
- É o elemento raiz da página HTML 

# `<head>`
- Container para conteúdos não-visíveis para o usuário 
  - Palavras-chave
  - Descrição
  - CSS 
  - Conjunto de caracteres
- Pode ser filho apenas do elemento `<html>`
- Elementos que podem ser usados dentro de um `<head>` element
  - `<title>`
  - `<base>`
  - `<link>`
  - `<style>`
  - `<meta>`
  - `<script>`
  - `<noscript>`

# `<meta charset="utf-8">`
- Define o tipo de codificação dos caracteres que o documento  
deve usar 
- utf-8 inclui a maioria dos caracteres das línguas humanas  
conhecidas
  - Lida com qualquer tipo de conteúdo textual inserido no  
  documento

# `<title>`
- Define o título da página, geralmente mostrado na aba do  
browser 
- Descreve a página ao ser salva nos favoritos 

# `<body>` 
- Container do conteúdo a ser mostrado aos usuários visitantes  
da página 
  - Texto
  - Imagens
  - Vídeos
  - Jogos
  - Áudio

# `h1` - `h6`
- Heading / cabeçalho
- São implementados em 6 níveis 
  - `h1` é o mais importante
  - `h6` é o de menor importância 
- Descreve o topico da seção em que ele está 
- Fontes pequenas não devem ser sinônimos de níveis menores 
- Pular níveis de heading deve ser evitado 
- Toda página deve ter, pelo menos, 1 heading de primeiro  
nível
- Cada `<section>` **deve** ter sua própria hierarquia de heading  
(exemplo) 

```html
<section>

  <h1>Forest elephants</h1> 

  <section>
    <h1>Introduction</h1>
    <p>Nesta seção, nós discutimos os menores elefantes florestais conhecidos.<p>
  </section>

  <section>
    <h1>Habitat</h1>
    <P>Elefantes florestais não vivem em árvores mas entre eles.</p> 
  </section>

  <aside>
    <p>Bloco publicitário</p>
  </aside>

</section>

<footer>
  <p>(c) 2010 O Exemplo de empresa</p>
</footer>
```

# `<!-- comentário -->`
- Ignorados pelo navegador
- Invisíveis para o usuário

# `p`
- Representa um parágrafo de texto 
- Possui display block 

# `br`
- Produz uma quebra de linha no texto 
- Útil para escrever poemas, endereços e outros tipos de  
texto onde a divisão de linhas é significante 

# `<blockquote>`
- Citação de bloco 
- Indica que o texto incluído é uma **longa** citação 
  - `<q>` é o elemento usado para uma **curta** citação 
- Conteúdo permitido
  - Flow content
- Pais permitidos
  - Qualquer elemento que aceita flow content
- Visualmente renderizado com recuo 
  - Pode ser alterado com a propriedade `margin`, do CSS 
- A URL da fonte da citação pode ser passada, através  
do atributo `cite="URLadress"`
- Uma representação textual da fonte pode ser passada  
usando o elemento `<cite>`

```html
<blockquote cite="https://www.huxley.net/bnw/four.html">
  <p>Words can be like X-rays, if you use them properly – they'll go through anything. You readand you're pierced.</p>
</blockquote>
<cite>– Aldous Huxley, Brave New World</cite>
```

![b](https://user-images.githubusercontent.com/29297788/43620554-a4b28440-96a9-11e8-9342-874d2ae91704.png)

```html
<blockquote cite="https://tools.ietf.org/html/rfc1149">
  <p>Avian carriers can provide high delay, low
    throughput, and low altitude service.  The
    connection topology is limited to a single
    point-to-point path for each carrier, used with
    standard carriers, but many carriers can be used
    without significant interference with each other,
    outside of early spring.  This is because of the 3D
    ether space available to the carriers, in contrast
    to the 1D ether used by IEEE802.3.  The carriers
    have an intrinsic collision avoidance system, which
    increases availability.</p>
</blockquote>
```

# `<q>`
- Usado para citações curtas, inline 
- Renderiza o elemento com aspas 
  - Podem ser retiradas com estilos CSS 
- Filhos permitidos:
  - Phrasing content / conteúdo fraseado 
- Pais permitidos:
  - Qualquer elemento que aceite phrasing content.
- A URL da fonte da citação pode ser passada, através  
do atributo `cite="URLadress"` 

```html
<p>
  <q cite="https://www.mozilla.org/en-US/about/history/details/">According to Mozilla's Website,Firefox 1.0 was released in 2004 and became a big success.
  </q>
</p>
```

```html
<p>
  In <cite>2001: A Space Odyssey</cite>, Dave asks HAL to open the pod bay door and HAL answers: 
  <q cite="https://www.imdb.com/title/tt0062622/quotes/qt0396921">
    I'm sorry, Dave. I'm afraid I can't do that.
  </q>
</p>
```
![hal](https://user-images.githubusercontent.com/29297788/43541931-01535674-95a2-11e8-8877-9f24f958b80d.png)


# `<cite>`
- Descreve uma referência à um trabalho artístico citado 
  - Livros 
  - Filmes 
  - Teatro
  - Redação
  - Poema
  - Partitura
  - Música
  - Roteiro
  - Séries de TV
  - Game
  - Escultura
  - Pintura
  - Opera
  - Musical
  - Programa de computador
  - Website
  - Blog post ou comentário
  - Forum post ou comentário
  - Um tweet
  - Declaração oral 
- Deve incluir o título **ou** a uma URL do trabalho 
- Usado para incluir uma referência à fonte do material citado  
contido em um elemento `<blockquote>` ou `<q>`
- Renderizado em itálico, por default 
- Inclui apenas atributos globais 
- Conteúdo permitido: Phrasing content
- Pais permitidos: qualquer elemento que aceite phrasing content 

```html
<p>
  More information can be found in <cite>[ISO-0000]</cite>
</p>
```

![cite the citation element html hypertext markup language mdn](https://user-images.githubusercontent.com/29297788/43541667-5758e224-95a1-11e8-8054-a91b31b41523.png)

```html
  <blockquote>
    <p>It was a bright cold day in April, and the clocks were striking thirteen.</p>
    <footer>
      First sentence in
      <cite>
        <a href="http://www.george-orwell.org/1984/0.html" target="_blank">
          <i>Nineteen Eighty-Four</i>
        </a>
        by George Orwell (Part 1, Chapter 1)
      </cite>
    </footer>
  </blockquote>
```

![q](https://user-images.githubusercontent.com/29297788/43621136-4104e8fe-96ac-11e8-9372-e0c5e8c76ef5.png)

# `<address>`
- Fornece informações de contato para seu ancestral  
`<article>` ou `<body>` mais próximo 
  - No segundo caso, se aplica ao documento inteiro 
- Fornece informação semântica adicional 
- Deve incluir o nome da pessoa, grupo ou organização para  
qual as informações de contato se referem 
- Torna as informações de contato apropriadas para qualquer  
contexto 
  - Informação de contato de uma empresa no header da página
  - Indicar um autor de um artigo, dentro de um `<article>`
- Pode incluir qualquer tipo de informação de contato  
necessária 
  - Endereço físico
  - URL
  - E-mail
  - Telefone
  - Redes Sociais 
  - Coordenadas Geográficas
- Em casos de endereços arbitrários, que não são relacionados às  
informações para contato, utilizar um elemento `<p>`
- Não deve conter mais informações além das informações de contato 
- Comumente posicionado dentro do elemento `<footer>` da sessão  
atual 

```html
<address>
    Voce pode contatar o autor em <a href="http://www.somedomain.com/contact">www.somedomain.com</a>.<br>
    Se encontrar qualquer bug, por favor <a href="mailto:webmaster@somedomain.com">contate o administrador do site</a>.<br>
    Você tambem pode querer nos visitar:<br>
    Mozilla Foundation<br>
    1981 Landings Drive<br>
    Building K<br>
    Mountain View, CA 94043-0801<br>
    USA
  </address>
```

# `<time>`
- Apresenta datas e horas 
- Representa o tempo nos formatos: 
  - 24 horas
  - Data do calendário gregoriano
- Não é adequado para datas específicas que não podem ser  
calculadas 
- Não deve ser utilizado em datas anteriores ao calendário  
gregoriano 
- Atributo datetime
  - Indica a hora e a data do elemento
  - Deve ser uma data válida, com uma string de tempo  
  opcional
- Atributo pubdate 
  - Atributo booleano que especifica que a data e hora  
  especificados pelo elemento é a data da publicação de  
  um documento
  - O documento ao qual se aplica é o elemento de `<article>`  
  ancestral mais próximo ou o documento como um todo 
  - Caso seja `true`, o elemento `<time>` deve possuir uma  
  data correspondente 
  - Cada elemento `<time>` indicando uma data de publicação  
  deve ser o único elemento `<time>` que faz isso para esse  
  documento

```html
<p>O show começa às <time>20:00</time>.</p>
```

```html
<article>
  <p>Esse artigo foi criado em <time pubdate>2018-07-29</time></p>
</article>
<!-- formato ANO-MÊS-DIA -->
```

```html
<article>
  <p>O show é em <time datetime="2018-07-15 23:00">Julho de 2018</time></p>
</article>
<!-- formato ANO-MÊS-DIA -->
```

# `<details>`
- Usado em casos onde o usuário irá obter informações adicionais 
- Clicável, expande e colapsa informações 
- Elementos filhos permitidos 
  - Um elemento `<summary>`, seguido por elementos `flow content`
- Pode receber o atributo `open="open"`
  - Boolean
  - Indica se os detalhes são mostrados ao usuário ao **carregar**  
  a página 
  - Se omitido, os detalhes não são mostrados ao carregar a página 

```html
<details open="open">
  <summary>alguns detalhes</summary>
  <p>Mais informações sobre os detalhes</p>
</details>
```

![details](https://user-images.githubusercontent.com/29297788/43499849-ea2f5fa2-9523-11e8-88da-4e6ed38a3286.png)

# `<summary>`
- Utilizado como sumário ou legenda para o conteúdo de um elemento  
`<details>`
- Elementos pais permitidos 
  - `<details>`
- Elementos filhos permitidos 
  - Elementos do tipo phrasing content 

# `<div>` 
- Uma divisão. Não adiciona significado ao conteúdo 

# `<button>`
- Um elemento que fará alguma ação ao ser clicado 

# `<nav>`
- Representa um elemento de navegação (menu, páginação, etc)

# `<aside>`
- Um bloco que é relacionado ao conteúdo principal, mas não faz  
parte dele

# `<footer>`
- Representa um **rodapé para o conteúdo da seção-pai** mais próxima,  
que pode ser 
  - `<article>`
  - `<aside>`
  - `<nav>`
  - `<section>`
  - `<blockquote>`
  - `<body>`
  - `<details>`
  - `<fieldset>`
  - `<figure>`
  - `<td>`
- Característico por conter informações sobre
  - O autor da seção
  - Direitos autorais 
  - Links para documentos relacionados 
- Não deve ser um descendente de um `<address>`, `<header>` ou outro  
elemento `<footer>`
- Dicas 
  - Informações sobre o autor devem ser envolvidas em um `<address>`,  
  que pode ser filho do `<footer>`

```html
<footer>
  Algumas informações de copyright ou talvez alguma informação do autor de um article?
</footer>
```

# HTML Semântico 
- Elementos que têm, de fato, um significado específico / relevante 
- Facilita a manutenção e compreensão do documento 
- Indica como programas de leitura de sites utilizados por deficientes  
visuais devem interpretar o conteúdo
- Facilita o reconhecimento de informações e relevância do conteúdo  
por robôs de busca que fazem a indexação da página 
  - É no HTML que os motores de busca e leitores de tela procurarão  
  informações armazenadas em seus reais significados 

# URL's absolutas
- `http://www.nodedosite.com/br/diretorio1/diretorio1/nomearquivo.html`
- São compostas por protocolo + domínio + caminho no servidor  
para a página ou documento 
- Úteis para referenciar sites, ou arquivos que estão hospedados  
em outro servidor, ou que dizem respeito a outro projeto de um  
outro domínio 

# URL's relativas
- `diretorio/nomearquivo.html`
- Caminhos relativos a documentos 
- Localiza o documento à partir do documento atual 
- `.` somente um ponto final indica a pasta atual 
- `..` dois pontos finais indicam a pasta pai da pasta atual 

# URL's relativas à raiz do website 
- Caminhos relativos à raiz do projeto 
- `/diretorio/nomearquivo.html`
- Acessa o arquivo a partir da raiz do projeto 
- Se um arquivo HTML usa links relativos à raiz do site para  
arquivos dependentes (como imagens) e um desses arquivos HTML  
for movido, os links do arquivo dependente em questão ainda  
serão válidos 

# Entidades de caracteres 
- Exibem caracteres especiais 
- [Lista oficial](https://dev.w3.org/html5/html-author/charref)
![image](https://user-images.githubusercontent.com/29297788/42913867-a5ac09bc-8acd-11e8-89a2-5d9f07a629a9.png)
![image](https://user-images.githubusercontent.com/29297788/42913819-6bf0b43e-8acd-11e8-870b-f3944354b3ef.png)

# `<fieldset>`
- Elemento usado para agrupar, por partes, elementos dentro de um  
`<form>`: 
  - `<legend>`, `<input>`, `<label>`
- Aceita atributos: 
  - `disabled` (exemplo 3)
    - Atributo booleano
    - Caso setado, todos os elementos de formulário descendentes do  
    `<fieldset>` serão desabilitados, ou seja, não serão editáveis,  
    submetidos e receptíveis à eventos do browser 
    - Browsers renderizam, por default, o elemento esmaecido 
    - Elementos de formulário dentro de um descendente `<legend>`  
    não são desabilitados
  - `form`
    - Pega o valor do ID do elemento `<form>` que é desejado que  
    o `<fieldset>` faça parte, mesmo que ele não esteja dentro do  
    formulário.
      - Caso não especificado, o valor default é o do ID do  
      `<form>` pai mais próximo 
  - `name`
    - Nome associado com o grupo 
- Deve conter um `<legend>` como primeiro filho 
  - É o label fo `<fieldset>`
- Estilo de renderização padrão
  - `display: block;`
  - Borda de 2px ao redor do conteúdo
  - Padding
  - Se tem `<legend>`, ele é sobreposto na borda superior 
- Categorias de conteúdo: 
  - Flow content
  - Sectioning root
  - Listed
  - Form-associated
- Conteúdo permitido
  - `<legend>` opcional
  - Flow-content 
- Pais permitidos
  - Qualquer elemento que aceite flow-content
- Funções ARIA permitidas
  - group
  - presentation

```html
  <form>
    <fieldset>
      <legend>Choose your favorite monster</legend>

      <input type="radio" id="kraken" name="monster">
      <label for="kraken">Kraken</label><br>

      <input type="radio" id="sasquatch" name="monster">
      <label for="sasquatch">Sasquatch</label><br>

      <input type="radio" id="mothman" name="monster">
      <label for="mothman">Mothman</label><br>
    </fieldset>
  </form>
```

![fieldset](https://user-images.githubusercontent.com/29297788/43621620-dbd44120-96ae-11e8-8383-285153f82ef5.png)

fieldset simples: 

```html
  <form action="#">
    <fieldset>
      <legend>Simple fieldset</legend>
      <input type="radio" id="radio">
      <label for="radio">Spirit of radio</label>
    </fieldset>
  </form>
```

![simple-fieldset](https://user-images.githubusercontent.com/29297788/43679664-20c30a86-97ff-11e8-84ea-b04c65fd1fb1.png)

exemplo 3:

```html
  <form action="#">
    <fieldset disabled>
      <legend>Disabled fieldset</legend>
      <div>
        <label for="name">Name: </label>
        <input type="name" id="text" value="Chris">
      </div>
      <div>
        <label for="pwd">Archetype: </label>
        <input type="password" id="text" value="Wookie">
      </div>
    </fieldset>
  </form>
```

![disabled-fieldset](https://user-images.githubusercontent.com/29297788/43679684-e95e7994-97ff-11e8-9a6b-1f5068ca31ab.png)

# `<meta>`
- Representa metadata que não pode ser representada por outros  
elementos meta relacionados, como `<base>`, `<link>`, `<script>`,  
`<style>` ou `<title>` 
  - Metadata é uma informação que descreve uma informação 
    - Um documento HTML é uma informação, mas também  
    pode conter metadata em seu elemento `<head>`,  
    que descreve o documento, por exemplo, quem o escreveu  
    e seu sumário
- Não possui tag de fechamento
- Categorias de conteúdo 
  - Conteúdo de metadata
  - Se o atributo `itemprop` estiver presente, flow content e  
  phrasing content
- Conteúdo permitido
  - Nenhum. É um elemento vazio
- Pais permitidos
  - Para `<meta charset>` e `<meta http-equiv>`, um elemento  
  `<head>`
    - Se `http-equiv` não for uma declaração de codificação,  
    também pode estar dentro de um elemento `<noscript>`, se  
    dentro de um elemento `<head>`
- Funções ARIA permitidas 
  - Nenhuma 
- Atributos 
  - Contém os atributos globais 
  - O atributo `name` possui um significado específico para o elemento  
  `<meta>`
  - O atributo `itemprop` não deve ser setado no mesmo elemento `<meta>`  
  que tem qualquer atributo `name`, `http-equiv` ou `charset`
  - `charset` declara a codificação dos caracteres da página 
    - Comumente usado com o valor UTF-8, codificação mais comum  
    utilizada na internet 
  - `content` contém o valor para os atributos `http-equiv` ou  
  `name`, dependendo de qual for usado 
  - `http-equiv` contém o nome de um header HTTP 
    - Define uma instrução que altera o comportamento entre  
    servidor e browser 
    - O valor da instrução é definido dentro do atributo `content`  
    e pode ser um dos seguintes valores: 
      - `"content-security-policy"` permite que autores da página  
      definam uma polítia de privacidade para a página atual.  
      Políticas de privacidades especificam, em sua maioria,  
      servidores permitidos e pontos de scripts que ajudam na  
      proteção contra ataques de scripting cross-sites 
    - `"refresh"` especifica: 
      - A quantidade de segundos até a página ser recarregada (o  
      atributo `content` deve ser um número inteiro positivo) -  
      exemplo 2
      - A quantidade de segundos até a página redirecionar para  
      outra página (o atributo `content` deve ser um número inteiro  
      positivo, seguido pela string `';url='` e uma url válida).  
      Exemplo 1
      - `"X-UA-Compatible"` define para qual versão do Internet  
      Explorer a página deve ser renderizada 
  - `name` define o nome de uma parte de metadados em nível  
  de documento
    - Não deve ser setado caso um dos atributos abaixo já estejam  
    especificados: 
      - `itemprop`
      - `http-equiv`
      - `charset`
    - É associado ao valor contido no atributo `content`
    - Valores possíveis: 
      - `application-name` define o nome da aplicação que  
      está rodando na página web. 
        - Browsers podem usá-lo para identificar a aplicação.  
        É diferente do elemento `<title>`, que normalmente contém  
        o nome da aplicação, mas também pode conter informações  
        como o ome do documento ou status.
        - Páginas web simples não devem definir um `application-name`
      - `author` define o nome do autor da página
      - `description` contém um curto e preciso sumário do  
      conteúdo da página 
        - Alguns browsers usam a descrição como descrição  
        default de páginas favoritadas 
      - `generator` contém o identificador do software que  
      gerou a página 
      - `keywords` contém palavras relevantes sobre o conteúdo  
      da página, seperadas por vírgulas 
      - `referrer` controla o header HTTP Referer, anexado para  
      enviar requests do documento 
      - `creator` define o nome do criador do documento, como  
      a organização ou instituição. Se houver mais de um,  
      diversos elementos `<meta>` devem ser utilizados 
      - `googlebot` sinônimo do `robots`. É seguido apenas pelo  
      Googlebot, o rastreador de indexação do google 
      - `publisher` define o nome do editor / publicador do  
      documento 
      - `robots` define o comportamento que rastreadores  
      cooperativos, ou "robôs", devem usar com a página.  
      Separa valores por vírgula
      - `viewport` dá dicas sobre o tamanho inicial da tela.  
      Usada apenas por dispositivos mobile. 
        - Define as regras de dimensões e escala para a tela  
        (exemplo 3)
- Deve ser a primeira tag filha do elemento `head`

exemplo 1:

```html
  <!-- Redireciona a página após 3 segundos -->
  <meta http-equiv="refresh" content="3;url=https://www.mozilla.org/pt-BR/">
```

exemplo 1.1: 

```html
  <!-- Redireciona a página imediatamente -->
  <meta http-equiv="refresh" content="0;url=https://www.mozilla.org/pt-BR/">
```

exemplo 2:

```html
  <!-- Recarrega a página após 2 segundos -->
  <meta http-equiv="refresh" content="2">
```

exemplo 3: 

```html
<meta name="viewport" content="width=device-width, initial-scale=1">
```