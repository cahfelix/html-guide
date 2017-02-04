# HTML Styleguide 

## Boas práticas no HTML5

É muito importante tornar o HTML mais fácil de entender e  se manter.

A ideia desse repositório é ser um local para que eu e outros desenvolvedores possamos participar e contribuir com padronizações e melhores práticas no HTML5.



### Fique de olho na aspas de seu código
Sempre use aspas duplas para suas classes e ids.

```html
<!-- Bom -->
<section class="container">

<!-- Ruim -->
<section class='container'>
```

### Fique de olho na indentação
Utilize indentação de dois espaços	

```html
<!-- Bom -->
<section class="container">
  <ul class="listagem">
    <li class="item">
      <a class="link">

<!-- Ruim-->
<nav class="navbar">
      <ul class="listagem">
            <li class="item">
                  <a class="link">
```


### Ordene seus atributos
Atributos HTML devem vir nesta ordem específica para facilitar a leitura do código.

- class
- id, name
- data-*
- src, for, type, href
- title, alt
- aria-*, role


```html
<a class="..." id="..." data-toggle="modal" href="#">
  Example link
</a>

<input class="form-control" type="text">

<img src="..." alt="...">

```


### Não especifique o type
Não há necessidade de especificar um ```type``` quando incluimos arquivos CSS e JavaScript como ```text/css``` e ```text/javascript```

```html
<!-- Bom -->
<link rel="stylesheet" href="assets/css/style.css">
<script src="scripts.min.js"></script>

<!-- Ruim -->
<link rel="stylesheet" type="text/css" href="assets/css/style.css">
<script type="text/JavaScript" src="scripts.min.js"></script>
```

Dica: insira todos os arquivos JavaScripts antes de fechar o ```<body>```final do documento para melhorar a performance de sua página, já os CSS insira no head do seu site

