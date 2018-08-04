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
  - `<command>`
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
  - `<keygen>`
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
  - `<command>`
  - `<datalist>`
  - `<dfn>`
  - `<em>`
  - `<embed>`
  - `<i>`
  - `<iframe>`
  - `<img>`
  - `<input>`
  - `<kbd>`
  - `<keygen>`
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
`<form>` 
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