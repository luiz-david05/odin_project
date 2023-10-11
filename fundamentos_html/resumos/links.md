## Elementos de ancoragem

```html
<a href="https://www.google.com">Google</a>
```

A tag `<a>` é a tag de abertura e fechamento, o atributo `href` é o atributo de ancoragem, e o valor do atributo é o link para onde o usuário será redirecionado ao clicar no link.

Abrir link em uma nova aba:

```html
<a href="https://www.google.com" target="_blank">Google</a>
```

rel é o atributo de relação, e o valor do atributo é o tipo de relação que o link tem com a página atual.

```html
<a href="https://www.google.com" target="_blank" rel="noopener noreferrer">Google</a>
```

Por quê precisamos do rel="noopener noreferrer" para abrir links em uma nova aba? Razões de segurança. A prevenção de phishing é uma delas. O rel="noopener noreferrer" é uma medida de segurança para evitar que o site que você está abrindo em uma nova aba tenha acesso ao site que você está navegando atualmente.

Note que estará tudo bem se esquecer de usar, mas é uma boa prática de segurança. A maioria dos navegadores modernos já fazem isso automaticamente, mas é sempre bom lembrar.

target= "_blank" sempre deve ser usado com rel="noopener noreferrer".


## Links absolutos e relativos

Geralmente, existem dois tipos de links que vamos criar:

1. Links para outras páginas na internet
2. Links para outras páginas do nosso próprio site

## Links absolutos

Links para páginas em outros sites na internet são chamados de links absolutos. Um típico link absoluto é feito com as seguintes partes: protocol://domain/path. Um link absoluto vai conter o protocolo e o domínio de destino.

Exemplos de links absolutos:

```html
<a href="https://www.google.com">Google</a>
<a href="https://www.theodinproject.com/about">theodinproject</a>
```

## Links relativos

Links para páginas do nosso próprio site são chamados de links relativos. Links relativos não incluem o nome de domínio. 

No mesmo diretorio do arquivo index.htlm, crie um novo arquivo de titulo about.html e adicione o seguinte conteúdo:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>About</title>
</head>

<body>
    <h1>About</h1>
    <p>This is the about page.</p>
</body>
</html>
```

Agora, no arquivo index.html, adicione o seguinte link:

```html
<body>
  <h1>Homepage</h1>
	<a href="https://www.theodinproject.com/about">click me</a>

	<a href="about.html">About</a>
</body>
```

Isso funciona porque o index e o about estão no mesmo diretório. Se você mover o arquivo about.html para um diretório diferente, o link não funcionará mais.

Mas nos usualmente queremos organizar melhor o nosso website. Normalmente, poderiamos ter apenas o index.html no diretório raiz e todos os outros arquivos em outros diretórios. 


```html	
<body>
  <h1>Homepage</h1>
  <a href="./pages/about.html">About</a>
</body>
```