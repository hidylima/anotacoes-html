# Anatomia de um elemento html 
![grumpy-cat-small](https://user-images.githubusercontent.com/29297788/43359652-1c286ff8-927c-11e8-97cf-d101772ccab9.png)

# Atributos de elementos HTML
![grumpy-cat-attribute-small](https://user-images.githubusercontent.com/29297788/43359655-40a23436-927c-11e8-9e5e-08ec1d87fda3.png)
- O valor do atributo é especificado entre as aspas duplas 

## Atributos booleanos 
- São atributos sem valores 
- Podem ter somente um valor, que geralmente é o mesmo nome  
do atributo: `disabled="disabled"`

# `<!DOCTYPE html>`
- Declarada no topo de documentos HTML
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
- Não e adequado para datas específicas que não podem ser  
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

# `<div>` 
- Uma divisão. Não adiciona significado ao conteúdo 

# `<button>`
- Um elemento que fará alguma ação ao ser clicado 

# `<nav>`
- Representa um elemento de navegação (menu, páginação, etc)

# `<aside>`
- Um bloco que é relacionado ao conteúdo principal, mas não faz  
parte dele

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