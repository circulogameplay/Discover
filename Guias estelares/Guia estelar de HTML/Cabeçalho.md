## Head

* Parte não visível pelo navegador
* Onde se faz configurações
* Contém informações como o título, links para o css, para o favicon

```html
    <head></head>
```

## Meta

* Serve para definir metadados - codificação de caracteres especiais e portabilidade para dispositivos mobiles;
* Normalmente virá com o atributo "name", e com o atributo charset.

```html
<head>
    <!-- codificação de caracteres especiais -->
    <meta charset="UTF-8">

    <!-- portabilidade para dispositivos mobiles -->
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
```

## Favicon

* Abreviação para "favorite icon";
* Ícones dos favoritos

* Uso da tag <"link"> com o atributo rel="icon" e depois o href="" para mostrar onde está o ícone;

```html
    <!--
    <link> para ícones personalizados
    -->

    <!-- favicon básico -->
    <link rel="icon" href="/icons/icon-48x48.png?v=cfca599cb367ccaf7377d56ddc7542f5"/>

    <!-- iPhone não-Retina, iPod Touch e dispositivos Android 2.1+: -->
    <link rel="apple-touch-icon-precomposed" href="https://developer.cdn.mozilla.net/static/img/favicon57.a2490b9a2d76.png">

    <!-- iPad de primeira e segunda geração: -->
    <link rel="apple-touch-icon" sizes="48x48" href="/icons/icon-48x48.png?v=cfca599cb367ccaf7377d56ddc7542f5"/>

    <link rel="apple-touch-icon" sizes="72x72" href="/icons/icon-72x72.png?v=cfca599cb367ccaf7377d56ddc7542f5"/>

    <link rel="apple-touch-icon" sizes="96x96" href="/icons/icon-96x96.png?v=cfca599cb367ccaf7377d56ddc7542f5"/>

    <!-- iPhone com tela retina de alta resolução: -->
    <link rel="apple-touch-icon" sizes="144x144" href="/icons/icon-144x144.png?v=cfca599cb367ccaf7377d56ddc7542f5"/>

    <!-- iPad de terceira geração com tela retina de alta resolução: -->
    <link rel="apple-touch-icon" sizes="192x192" href="/icons/icon-192x192.png?v=cfca599cb367ccaf7377d56ddc7542f5"/>

    <link rel="apple-touch-icon" sizes="256x256" href="/icons/icon-256x256.png?v=cfca599cb367ccaf7377d56ddc7542f5"/>

    <link rel="apple-touch-icon" sizes="384x384" href="/icons/icon-384x384.png?v=cfca599cb367ccaf7377d56ddc7542f5"/>

    <link rel="apple-touch-icon" sizes="512x512" href="/icons/icon-512x512.png?v=cfca599cb367ccaf7377d56ddc7542f5"/>
```

## Meta SEO

* Metas importantes para SEO (Search Engine Optimization ou motores de busca, como o Google)

### Já vimos

```html
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
``` 

### Temos o de autor, para definir o autor da página (possuir propriedade)

```html
    <meta name="author" content="Mayk Brito">
```

### Descrição de sites

```html
    <meta name="description" content="Um website para iniciantes em programação">
```

### Dizer para o robô do google o que quer que ele faça

```html
    <meta name="robots" content="index, follow">        
```


## Meta Social

* Existem metadados personalizados por empresas de redes sociais, como Facebook, que criou o Open Graph, que é um tipo de metadado se quisermos colocar um tipo de conteúdo especial, caso queiramos compartilhar o link da nossa página no Facebook.

* Exemplos: imagens, descrição, texto e outros

```html
    <head>
        <!-- Open Graph: facebook -->
        <meta property="og:image" content="https://cdn-images-1.medium.com/max/92/1*TkXVfLTwsHdwpUEjGzdi9w@2x.jpeg">
        <meta property="og:description" content="Aqui vem um texto para ser mostrado ao compartilhar no facebook">
        <meta property="og:title" content="Um site da Rocketseat">

        <!-- twitter -->
        <meta name="twitter:title" content="Rocketseat">
    </head>
```