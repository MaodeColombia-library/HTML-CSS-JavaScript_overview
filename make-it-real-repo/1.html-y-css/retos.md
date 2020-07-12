# Retos

##  ¡Hola HTML!

Este reto es modificar el codigo para que el texto "HTML" aparezca en negrita como se muestra en la siguiente imagen:

![Hello HTML](https://s3.amazonaws.com/makeitreal/hello-html.png)

```markup
<!DOCTYPE html>
<html>
  <head></head>
  <body>  
    ¡Hola HTML!
  </body>
</html>
```

### Instrucciones

1. Modifica el código para que el texto "HTML" aparezca en negrita \(solo la palabra, sin signo de exclamación\).

### Discusión: Hola mundo

La solución es la siguiente:

```markup
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    ¡Hola <strong>HTML</strong>!
  </body>
</html>
```

Existen dos etiquetas que cumplen la misma función de mostrar texto en negrita: `b` y `strong`. Cualquiera de las dos funciona aunque ahora es más común `strong`.

## Etiquetas

Este reto es modificar el código para obtener el siguiente resultado:

![Hypertext](https://s3.amazonaws.com/makeitreal/hypertext.png)

**Nota:** Fíjate que la palabra "párrafo" debe estar en negrita en los dos párrafos. El evaluador espera que uses la etiqueta `strong` .

```markup
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    Este es el título

    Este es el primer párrafo.

    Este es el segundo párrafo.
  </body>
</html>
```

### Instrucciones

1. Modifica el archivo para lograr el resultado esperado usando las etiquetas `h1` y `p`, y `strong`.

### **Discusión:** Etiquetas

```markup
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <h1>Este es el título</h1>

    <p>Este es el primer <strong>párrafo</strong>. </p>

    <p>Este es el segundo <strong>párrafo</strong>.</p>
  </body>
</html>
```

HTML está compuesto de etiquetas. Una etiqueta es una palabra clave encerrada entre `<` y `>`.

Algunas etiquetas necesitan una **etiqueta de cierre** porque pueden contener texto y otras etiquetas anidadas. La **etiqueta de cierre** es muy parecida a una etiqueta, pero lleva un slash `/` antes de la palabra clave \(p.e. `</strong>` es la etiqueta de cierre de `<strong>`\).

En [este enlace](https://www.w3schools.com/tags/default.asp) puedes encontrar la lista de etiquetas de HTML.

## ¡Hypertexto!

Este reto es que el texto **"Ver más"** dentro de el código sea un vínculo \(link\) que nos lleve a [este enlace](http://blog.makeitreal.camp/html-css).

```markup
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <h1>HTML y CSS</h1>

    <p>Para hacer páginas Web necesitas aprender dos lenguajes:
      HTML y CSS. Estos son los lenguajes que los navegadores
      (Firefox, Chrome, Internet Explorer) entienden e interpretan
      para mostrarte lo que ves cuando abres alguna página.</p>

    Ver más
  </body>
</html>
```

### Instrucciones

1. Abre el enlace y copia la URL.
2. Identifica el texto **Ver más** en el codigo y agrega el link.

### **Discusión:** ¡Hypertexto!

La solución es

```markup
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <h1>HTML y CSS</h1>

    <p>Para hacer páginas Web necesitas aprender dos lenguajes:
      HTML y CSS. Estos son los lenguajes que los navegadores
      (Firefox, Chrome, Internet Explorer) entienden e interpretan
      para mostrarte lo que ves cuando abres alguna página.</p>

    <a href="http://blog.makeitreal.camp/html-css">Ver más</a>
  </body>
</html>
```

[Hypertexto](https://www.w3.org/WhatIs.html) \(en inglés hypertext\) significa: texto con vínculos a otros textos. De ahí vienen el nombre **HTML \(Hyper Text Markup Language\)**: un **lenguaje** que nos permite definir la estructura \(**markup**\) de textos \(documentos\) con vínculos a otros documentos \(**hypertexto**\).

**Dato curioso:** Técnicamente deberíamos cambiarle el nombre a HTML por HMML \(Hyper **Media** Markup Language\) porque ahora HTML soporta no solo texto, sino imágenes, audio y video. Pero al parecer nadie ha propuesto el cambio y la verdad no valdría la pena en este momento ;\)

## El título de la página

Este reto es agregarle el título "El movimiento open source" al documento HTML que se encuentra en el codigo como se muestra en la siguiente imagen:

![Open source](https://s3.amazonaws.com/makeitreal/results/open-source.png)

```markup
<!DOCTYPE html>
<html>
  <head>

  <head>
<title>El movimiento open source</title>
</head>

  </head>
  <body>
    <h1>Open Source</h1>
    <p>Open source (código abierto) es un movimiento que se originó por la
      ambigüedad del término <em>free software (software libre)</em>. El
      problema es que en Inglés la palabra <em>free</em> también significa
      <em>gratis</em>, pero open source no necesariamente es gratis.</p>

    <p>El objetivo del movimiento es que todos tengan la capacidad de ver el
      código del software que están adquiriendo. Pero existe mucho software
      open source que no es gratis, especialmente para uso comercial. Un
      ejemplo es <a href="https://source.android.com/">Android</a>, que
      aunque es un proyecto open source, no significa que cualquiera pueda
      comercializar teléfonos con ese sistema operativo.</p>
  </body>
</html>
```

### Instrucciones

1. Agrega el título "El movimiento open source" al codigo.

###  **Discusión:** El título de la página

La solución es

```markup
<!DOCTYPE html>
<html>
  <head>
  <title>El movimiento open source</title>
  </head>
  <body>
    <h1>Open Source</h1>
    <p>Open source (código abierto) es un movimiento que se originó por la
      ambigüedad del término <em>free software (software libre)</em>. El
      problema es que en Inglés la palabra <em>free</em> también significa
      <em>gratis</em>, pero open source no necesariamente es gratis.</p>

    <p>El objetivo del movimiento es que todos tengan la capacidad de ver el
      código del software que están adquiriendo. Pero existe mucho software
      open source que no es gratis, especialmente para uso comercial. Un
      ejemplo es <a href="https://source.android.com/">Android</a>, que
      aunque es un proyecto open source, no significa que cualquiera pueda
      comercializar teléfonos con ese sistema operativo.</p>
  </body>
</html>
```

Un documento HTML tiene dos grandes secciones: el encabezado \(`<head>`\) y el cuerpo \(`<body>`\) como se muestra en el siguiente ejemplo:

```markup
<!DOCTYPE html>
<html>
  <head>
    ...
  </head>
  <body>
    ...
  </body>
</html>
```

La primera línea `<!DOCTYPE html>` le dice al navegador que estamos usando la última versión de HTML, HTML5. Un documento HTML siempre empieza con la etiqueta `<html>`.

En el `<head>` va información que no es visible en la pantalla como el **título del documento**, referencia a otros archivos, etc. En el `<body>` van los elementos visibles en la pantalla.

##  Una deliciosa receta

Este reto es crear una página con la receta de una ensalada. El resultado final debe quedar igual al que se muestra a continuación:

![Result](https://s3.amazonaws.com/makeitreal/results/a-delicious-salad.png)

### Instrucciones

1. En el archivo `index.html` agrega la estructura básica que debe tener todo HTML.
2. El título de la página debe ser `Mis Recetas`.
3. La imagen se encuentra en [https://s3.amazonaws.com/makeitreal/salad.png](https://s3.amazonaws.com/makeitreal/salad.png).
4. Utiliza las etiquetas `h1`, `h2`, `img`, `ul`, `li`, y `p` para crear el contenido de la página.

 **Discusión:** Una deliciosa receta

```markup
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>Mis Recetas</title>
</head>
<body>
  <h1>Receta: Ensalada</h1>
  <img src="https://s3.amazonaws.com/makeitreal/salad.png" alt="Ensalada">

  <h2>Ingredientes</h2>
  <p>Los ingredientes necesarios para preparar la ensalada son los siguientes:</p>
  <ul>
    <li>Pechuga</li>
    <li>Lechuga</li>
    <li>Tomate</li>
    <li>Cebolla</li>
    <li>Maiz</li>
  </ul>

  <h2>Preparación</h2>
  <p>Se pican todos los ingredientes, se mezclan y listo!</p>
</body>
</html>
```

Excelente trabajo Maker!

[HTML \(Hyper Text Markup Lenguage\)](https://es.wikipedia.org/wiki/HTML) fue creado en 1989, junto a [HTTP \(Hyper Text Markup Protocol\)](https://es.wikipedia.org/wiki/Hypertext_Transfer_Protocol), como parte del proyecto [World Wide Web \(WWW\)](https://es.wikipedia.org/wiki/World_Wide_Web). El objetivo inicial de WWW era permitir publicar y compartir documentos académicos dentro de [CERN](https://es.wikipedia.org/wiki/Organizaci%C3%B3n_Europea_para_la_Investigaci%C3%B3n_Nuclear) \(donde se encuentra el acelerador de partículas más grande del mundo\).

HTML permitiría definir la estructura de un documento, es decir, encabezados, párrafos, listas, etc. \(en ese momento no se podían incluir imágenes, video, o audio\). Pero lo realmente novedoso era que HTML permitiría incluir vínculos a otros documentos, creando así una **red de documentos interconectados**.Generalmente, el código HTML \(Hyper Text Markup Language\) viaja a través de HTTP \(Hyper Text Transfer Protocol\). Pero es posible crear un archivo de texto con extensión `.html` y abrirlo en un navegador directamente.

**Nota:** La etiqueta `<meta charset="UTF-8">` dentro de `<head>` se usa para que las tildes funcionen.
