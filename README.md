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







