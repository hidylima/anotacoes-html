# Anotações HTML

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