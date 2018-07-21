# Anotações HTML

## Tags 

### `<div>` 
- Uma divisão. Não adiciona significado ao conteúdo 

### `<button>`
- Um elemento que fará alguma ação ao ser clicado 

### `<nav>`
- Representa um elemento de navegação (menu, páginação, etc)

### `<aside>`
- Um bloco que é relacionado ao conteúdo principal, mas não faz  
parte dele

## HTML Semântico 
- Elementos que têm, de fato, um significado específico / relevante 
- Facilita a manutenção e compreensão do documento 
- Indica como programas de leitura de sites utilizados por deficientes  
visuais devem interpretar o conteúdo
- Facilita o reconhecimento de informações e relevância do conteúdo  
por robôs de busca que fazem a indexação da página 
  - É no HTML que os motores de busca e leitores de tela procurarão  
  informações armazenadas em seus reais significados 

## URL's absolutas
- `http://www.nodedosite.com/br/diretorio1/diretorio1/nomearquivo.html`
- São compostas por protocolo + domínio + caminho no servidor  
para a página ou documento 
- Úteis para referenciar sites, ou arquivos que estão hospedados  
em outro servidor, ou que dizem respeito a outro projeto de um  
outro domínio 

## URL's relativas
- `diretorio/nomearquivo.html`
- Caminhos relativos a documentos 
- Localiza o documento à partir do documento atual 
- `.` somente um ponto final indica a pasta atual 
- `..` dois pontos finais indicam a pasta pai da pasta atual 

## URL's relativas à raiz do website 
- Caminhos relativos à raiz do projeto 
- `/diretorio/nomearquivo.html`
- Acessa o arquivo a partir da raiz do projeto 
- Se um arquivo HTML usa links relativos à raiz do site para  
arquivos dependentes (como imagens) e um desses arquivos HTML  
for movido, os links do arquivo dependente em questão ainda  
serão válidos 

## Entidades de caracteres 
- Exibem caracteres especiais 
- [Lista oficial](https://dev.w3.org/html5/html-author/charref)
![image](https://user-images.githubusercontent.com/29297788/42913867-a5ac09bc-8acd-11e8-89a2-5d9f07a629a9.png)
![image](https://user-images.githubusercontent.com/29297788/42913819-6bf0b43e-8acd-11e8-870b-f3944354b3ef.png)