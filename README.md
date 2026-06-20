![](./img/banner.png)

# HTML5 - CSS3



## Requisitos

- Computador ou notebook
- Sistema Operacional: Linux, Windows ou Mac
- IDE: Sublime Text ou VS-Code
- Browser: Firefox, Google Chrome ou Edge
- Editor de imagens: Gimp
- Git e conta no Github



![](/home/sergio/Documentos/dev/html-css/exercicio/ex003/logo_html5.png)

## HTML

- Hiper Text Markup Language - Linguagem de Marcação de Hipertexto
- Responsável pela estrutura do conteúdo do documento
  - texto
  - imagem
  - video
  - áudio



![](/home/sergio/Documentos/dev/html-css/exercicio/ex003/img/logo_css3.png)

## CSS

- Cascading Style Sheet - Folha de Estilos em Cascata

- Responsável pela formatação de estilos
  - fontes
  - cores
  - espaçamento
  - alinhamento
  - tamanho
  - bordas
  - sombras



## HTTP-SERVER

Para o desenvolvimento com editores de código que não possuem a ferramentas como o live server do VS-Code podemos usar um pacote node para criar um servidor web que pode ser acessado por usuários na rede local.

Para distros Linux da família Debian:

```$ sudo apt install node-http-server```

Para subir o servidor:

```$ http-server```

De qualquer dispositivo que esteja conectado na mesma rede basta digitar o endereço IP que será fornecido:

http://127.168.1.0:8080



## Snnipet

Código básico para iniciar uma página:

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>Parágrafos</title>
</head>
<body>
	conteúdo...
</body>
</html>
```



## Inserindo emojis &#x1F61C;

Acessar http://emojipedia.org e copiar o código ( U+1F61C) na aba de informação técnica. No HTML inserir no formato &#x1F61C e terminar com ponto e vírgula.

_Obs.: funciona bem com emojis mais comuns_.



## Imagens

* A imagem não deve ultrapassar 100 kb
* Usar formatos jpeg, png ou webp
* Para imagens grandes de background usar jpeg que possui melhor compactação
* Para imagens que vão ficar sobrepostas e precisam de transparência usar png
* Preferencialmente produzir imagens nos diversos tamanhos de uso

### Carga de imagens

```html
<body>
	<h1>Testando carga e Imagens</h1>
	<p>Abaixo você vai ver uma imagem que está na mesma pasta.</p>
	<img src="./logo_html5.png" alt="logotipo HTML5">
	<p>Podemos carregar imagens que estão em subpastas.</p>
	<img src="./img/logo_css3.png" alt="logotipo CSS3">
	<p>Também podemos carregar imagens externas.</p>
	<img src="https://upload.wikimedia.org/wikipedia/commons/9/99/Unofficial_JavaScript_logo_2.svg" alt="logotipo Javascript" width="200px">
</body>
```



## Favicon

Ícone de identificação da página que é exibido na lateral esquerda da aba do navegador.

Para baixar um pacote de favicon com arte própria:

http://iconarchive.org

Para criar um favicon 

http://favicon.io

Preferência para o formato svg, ico ou png.

Para adicionar o ícone precisamos inserir a tag link no head do arquivo html.

``` html
<link rel="shortcut icon" href="./favicon.svg" type="image/x-icon">
```



 ## Heading (Cabeçalho)

Títulos por ordem de relevância:

```html
<h1>Título 1</h1>
<h2>Título 2</h2>
<h3>Título 3</h3>
<h4>Título 4</h4>
<h5>Título 5</h5>
<h6>Título 6</h6>
```



## Semântica no HTML5

O HTML semântico torna o código HTML com a responsabilidade exclusiva pelo significado conteúdo, formatações de estilo como cor, alinhamento, espaçamento, fonte, tamanho passam a ser de responsabilidade apenas do CSS.

Tags e atributo obsoletos:

```html
<html>
	<head>
		<title>Site em HTML4</title>
	</head>
	<body bgcolor="blue">
		<center><h1>Exercício de site em HTML4</h1></center>
		<marquee behavior="scroll" direction="right">
			<h2>Teste de Marquee - Tag HTML4 obsoleta</h2>
		</marquee>
		<p><font color="white">Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea eius nam facilis maxime vel soluta beatae magnam neque quasi id, eos hic nulla, eveniet, quae sed modi praesentium placeat error!</font></p>
		<p>Eu moro na <u>Rua dos Capixabas, 229 Botafogo - Rio de Janeiro</u></p>
	</body>
</html>
```

### Formações

```html
<body>
	<h1>Principais formatações</h1>
	<h2>Negrito / Destaque</h2>
	<p>Nessa frase temos um <b>termo em negrito</b> usando a tag B (não semântica).</p>
	<p>Nessa frase temos um <strong>termo em negrito</strong> usando a tag STRONG (semântica).</p>
	<h2>Itálico / Ênfase</h2>
	<p>Nesta frase, temos um termo em <i>itálico usando</i> a tag I (não semântica)</p>
	<p>Nesta frase, temos um termo em <em>itálico usando</em> a tag EM (semântica)</p>
	<h2>Texto marcado</h2>
	<p>Podemos criar também <mark style="background-color:lime;">um texto marcado</mark> usando a tag MARK.</p>
	<p>E no outro parágrafo, temos <mark>outro texto marcado</mark> no final.</p>
	<h2>Texto grande e pequeno</h2>
	<p>Estamos criando um <big>texto grande</big> e um <small>texto pequeno</small> nesse parágrafo.</p>
	<h2>Texto Deletado</h2>
	<p>Podemos marcar <del>um texto como excluído</del> para identificar que ele deve ser lido, mas não considerado.</p>
	<h2>Texto Inserido</h2>
	<p>Podemos marcar <ins>um texto como inserido</ins> para dar uma ênfase e indicar que ele foi adicionado depois.</p>
	<p>Existe também o <u>sublinhado</u> com a tag U (não semântica).</p>
	<h2>Texto Sobrescrito</h2>
	<p>Para inserir coisa do tipo x<sup>20</sup>	 + 3.</p>
	<h2>Texto Subscrito</h2>
	<p>Para inserir coisas do tipo H<sub>2</sub>O.</p>
</body>
```



### Outras formatações

```html
<body>
	<h1>Outras formatações</h1>
	<h2>Código-fonte</h2>
	<p>O comando <code>document.getElementById('teste')</code> é escrito em linguagem Javascript.</p>
	<pre>
		<code>
		num = int(input('Digite um número'))
		if num % 2 == 0:
			print(f'O número {num} é PAR')
		else:
			print(f'O número {num} é ÍMPAR)
	</code>
	</pre>
	<h2>Citações</h2>
	<p>Como diria o pai de um amigo: <q>o computador é um burro muito rápido</q>.</p>
	<h2>Citação completa</h2>
	<p>Segundo Jeff Noble, no seu livro HTML para leigos:</p>
	<blockquote cite="#">
		E diferença entre elementos inline e um bloco de texto é importante. Os elementos HTML neste capítulo descrevem os blocos de texto.
	</blockquote>
	<h2>Abreviações</h2>
	<p>Estou estudando <abbr title="HyperText Markup Language">HTML</abbr> e <abbr title="Cascading Syle Sheet">CSS</abbr>. Estou adorando!</p>
	<h2>Texto Invertido</h2>
	<p><bdo dir="rtl">Estou aprendendo em criar coisas em HTML.</bdo></p>
</body>
```



## Listas

### Listas Ordenadas

```html
	<h2>Listas ordenadas</h2>
	<ol type="1" start="1">
		<!--Types 1 A a I i-->
		<li>Acordar</li>
		<li>Ligar para o João</li>
		<li>Tomar café</li>
		<li>Escovar os dentes</li>
		<li>ir para a faculdade</li>
		<li>Almoçar</li>
		<li>Ir para o trabalho</li>
		<li>Voltar para casa</li>
		<li>Jantar</li>
		<li>Dormir</li>
	</ol>
```



### Listas Não Ordenadas

```html
<h2>Listas não ordenadas</h2>
	<ul type="square">
		<!--Types disc circle square-->
		<li>Pão</li>
	    <li>Leite</li>
	    <li>Tomate</li>
	    <li>Manteiga</li>
	    <li>Arroz</li>
	    <li>Feijão</li>
	</ul>
```



### Listas de Definição

```html
<dl>
	<dt>HTML</dt>
	<dd>Linguagem de marcação para a criação do conteúdo de um site.</dd>
	<dt>CSS</dt>
	<dd>Linguagem de marcação para a criação de design de um site</dd>
	<dt>Javascript</dt>
	<dd>Linguagem de programação para a a criação de interatividade de um site</dd>
</dl>
```



## Links

Links são a essência da internet são por eles (hyperlinks) que acessamos outras páginas.

O atributo _target_ pode assumir os valores _self para carregar o link na mesma janela ou _blank para carregar o conteúdo em uma nova aba.

### Link externo

```html
<p>Você pode acessar o meu <a href="https://github.com/sergiomerces/" target="_blank" rel="external">repositório público no Github</a></p>
```



### Link interno

```html
<p>Esta é a primeira página do site. Se você quiser, pode acessar também a minha <a href="./page002.html" rel="next">Segunda página</a></p>

<p><a href="index.html" rel="prev">Voltar para a primeira página.</a></p>
```



### Link para download

```html
<a href="./artigo.pdf" type="application/pdf">Baixar o artigo em PDF</a>

<a href="./artigo.zip" type="application/zip">Baixar o artigo compactado ZIP</a>
```



## Imagens Dinâmicas

Como os usuários acessam a internet em dispositivos com diferentes tamanhos de tela, é preciso pensar na adaptabilidade das imagens para que possam ser carregadas de forma eficiente em dispositivos de telas grandes como em telas pequenas.

Para isso tenha versões em tamanhos diferentes das imagens que fará uso no site.

```html
<h1>Imagem dinâmica</h1>
	<p>Tente abrir esse site em vários dispositivos diferentes ou simplesmente aumente e diminua o tamanho do seu navegador.</p>
	<picture>
		<source media="(max-width: 750px)" srcset="./img/foto-p.png" type="image/png">
		<source media="(max-width: 1050px)" srcset="./img/foto-m.png" type="image/png">
		<img src="./img/foto-g.png" alt="Imagem flexível">
	</picture>
```

Usamos a tag <picture> para informar que ali será exibida uma imagem. Devemos manter a escrita da maior para a menor imagem ou o inverso, nesse exemplo vamos usar a maior imagem como padrão e com a tag <source> informamos na ordem quais são as outras imagens que queremos para cada tamanho de tela.
