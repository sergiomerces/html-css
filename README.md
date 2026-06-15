![](./img/banner.png)

# HTML5 - CSS3



## Requisitos

- Computador ou notebook
- Sistema Operacional: Linux, Windows ou Mac
- IDE: Sublime Text ou VS-Code
- Browser: Firefox, Google Chrome ou Edge
- Editor de imagens: Gimp
- Git e conta no Github



## HTML

- Hiper Text Markup Language - Linguagem de Marcação de Hipertexto
- Responsável pela estrutura do conteúdo do documento
  - texto
  - imagem
  - video
  - áudio



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

```
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

