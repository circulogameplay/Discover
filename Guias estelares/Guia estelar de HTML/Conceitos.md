## O que é HTML

* Hypertext Markup Language (Linguagem de marcação de texto)
* NÃO é uma linguagem de programação
* Linguagem na forma de escrever, tendo sintaxe e semântica

## Comentários

* Comentários servem para nos ajudar a não nos perder em nossos códigos, sendo bem simples abrir um comentário, dessa forma:

```html
    <!-- comentários -->
```
* OBS: O que há em um comentário não afetará o código.

## Anatomia de Tags

* As Tags funcionam da seguinte forma:

```html
    <h1> TÍTULO </h1>
```
* Você faz a abertura delas, coloca o nome da Tag e as fecha como no exemplo. No caso dessa Tag, seu conteúdo é a de título, juntando a abertura, fechamento e o conteúdo, teremos um Elemento HTML.

* Há também Elementos vazios que diferente do exemplo acima não se fecha daquela forma, mas assim:

* Essa sendo para imagem possuindo atributos

```html
    <img src=" " alt=" ">
```

## Atributos

* Atributos booleanos: não precisam de conteúdo (verdadeira ou falso)

```html
    <input type="text" disabled>
```
* Aspas: recomendado apenas o uso das aspas duplas, para não desencadear problemas no código

## Atributos Globais

* Atributos apicáveis em todas as tags.
* Class - classificar as tags; aplicar estilo CSS; acessar com o JavaScript.
```html
    <div class="conteúdo">
    </div>
```
* Contenteditable - editar o conteúdo da pag; não mantido após salvar
```html
    <div contentedtable="true">
    </div>
```
* Data - expandir os tipos de atributos que podem ser usados para fazer mais lógica no JavaScript; utilizado em CSS também. Pode ser escrito com ou sem "-"
```html
    <div data-qualquercoisaaqui="">
    </div>
```
* Hidden — usado para esconder uma Tag.

* Id — usado apenas 1 por Tag para identificação; usado CSS e JS
```html
    <div id="texto">
        conteúdo
    </div>

    <div id="texto2">
        conteúdo
    </div>
```
* Style — aplica a estilização na Tag, normalmente não se usa "style" dentro da Tag, mas sim em arquivos externos.
```html
    <div style="color: red">
```
* Tabindex - usado para ordenar o Tab na página.
```html
    <div tabindex="3">
    </div>

    <div tabindex="1">
    </div>

    <div tabindex="2">
    </div>
```
* Title —  definir um título para a Tag, quando colocamos o mouse descansando em cima do conteúdo da página.


Se você quiser estudar outros Atributos Globais vá ao site https://developer.mozilla.org/pt-BR/ .


## Alinhamento Hierarquia

* Colocar uma tag dentro da outra = ALinhamento
* Não é qualquer tag que podemos colocar dentro de outra
* Existe uma hierarquia

```html
    <p> 
        <em>texto<em>
        <p> texto2</p> 
    </p>  
```
* Tag <"em"><"/em"> (ênfase no texto) é pertencente a Tag <"p"><"/p"> (criar um parágrafo)
* Há um fluxo, tags lidas de cima para baixo
* Posicionamento de elementos: tag <"em"><"/em"> não está em uma outra linha como na tag <"p"><"/p">, existem tags que quebram a linha, então mesmo que colocarmos a tag <"p"><"/p"> uma do lado da outra, visualmente vai dar quebra de linha.
 
## Caracteres Reservados
* Caracteres reservado são caracteres usados no próprio HTML, não podendo utilizar nas tags, pois dão erro.
* Precisamos trocar por outra forma de escrever
```html
    <p>
        &lt;
        os espaços 
        &gt;
        &amp;
        
        <br>
        &quot; que colocamos    
        &quot;
        <br>
        &apos; além das quebras de linha são
        ignorados
    </p> 
```

## Anatomia Documento

```html
    <!DOCTYPE html>
    <html>
        <head>
            <meta charset="utf-8">
            <title>Anatomia do Documento</title>
        </head>

        <body>
            <h1>Título</h1>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Officiis saepe similique perferendis mollitia a assumenda doloribus omnis, quidem tempore accusamus repudiandae. Accusamus, rem dolorum ad repellendus distinctio blanditiis praesentium nulla?
            </p>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Officiis saepe similique perferendis mollitia a assumenda doloribus omnis, quidem tempore accusamus repudiandae. Accusamus, rem dolorum ad repellendus distinctio blanditiis praesentium nulla?
            </p>
        </body>
    </html>
```
O padrão seria esta forma.

* <"!DOCTYPE html"> — diz ao navegador que estamos a trabalhar com HTML 5.
* <"html"><"/html"> — o próprio HTML, elemento raiz, o inicio da cadeia.* <"head"><"/head"> — contém configurações importantes para página, mas não ainda o que o usuário vai ver.
* <"meta"> — onde vai representar vários tipos de metadados da página.

* <"title"><"/title"> — título da página.
* <"body"><"/body"> — onde haverá conteúdo visual da página.


Se quiser facilitar tudo digitando ! o emmet irá completar automaticamente.

## Criando Projetos

Estaremos vendo como criar um projeto html.

Abrindo o explorador de arquivos do seu computador, indo na parte de usuário > documentos e criará a pasta do projeto, e arrastará para o VSCode.

Você pode criar arquivos, por exemplo: index.html, ou criar pastas.