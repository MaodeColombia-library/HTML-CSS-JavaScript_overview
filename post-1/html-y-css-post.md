---
description: de este post que esta no estoy de acuerdo con las mal llamadas "etiquetas"
---

# HTML y CSS \(post\)

![](../.gitbook/assets/html5-css3.png)

Para hacer páginas Web necesitas aprender dos lenguajes: **HTML** y **CSS**. Estos son los lenguajes que los navegadores \(Firefox, Chrome, Internet Explorer\) entienden e interpretan para mostrarte lo que ves cuando abres alguna página.

**HTML** se usa para definir **la estructura** de la página \(títulos, párrafos, tablas, listas, vínculos, formularios, imágenes, etc.\) y **CSS** se usa para **aplicarle el estilo** \(color de fondo, márgenes entre los elementos, tamaño de las fuentes, bordes, etc.\).

### Etiquetas <a id="etiquetas"></a>

**HTML** está compuesto de etiquetas. Una etiqueta es una palabra clave encerrada entre `<` y `>`. Por ejemplo, `<hr>` es una etiqueta que pinta una línea horizontal como la siguiente :

**Algunas etiquetas necesitan una etiqueta de cierre** porque pueden contener texto y otras etiquetas. La etiqueta de cierre lleva un slash \(/\) antes de la palabra clave. Por ejemplo, la etiqueta `<p>` se utiliza para definir un párrafo y necesita una etiqueta de cierre `</p>` cuando termina el párrafo:

```text
<p>
  Este es un párrafo <em>importante</em>.
</p>
```

En este ejemplo hemos definido un párrafo que contiene texto y una etiqueta `<em>` con más texto.

### La estructura de una página Web <a id="la-estructura-de-una-p&#xE1;gina-web"></a>

Una página Web \(documento HTML\) tiene dos grandes secciones: el encabezado \(`<head>`\) y el cuerpo \(`<body>`\) como se muestra en el siguiente ejemplo:

```text
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

En el `<head>` va **información que no es visible en la pantalla** como el título del documento, referencia a otros archivos, etc. En el `<body>` van los elementos visibles en la pantalla. Generalmente, el código **HTML** \(Hyper Text Markup Language\) viaja a través de **HTTP** \(Hyper Text Transfer Protocol\). Pero es posible crear un archivo con extensión `.html` y abrirlo en un navegador directamente.

### CSS <a id="css"></a>

Con **CSS \(Cascading Style Sheets\)** le podemos dar formato a los elementos **HTML**. Por ejemplo, la siguiente regla cambia el color de la fuente de los párrafos a azul:

```text
p {
  color: blue;
}
```

Una regla en **CSS** está compuesta de un selector y un bloque con una o más declaraciones. En este ejemplo `p` es el selector y `color: blue;` es una declaración.

Las reglas CSS se pueden ubicar en varios lugares:

* En el atributo `style` de cualquier etiqueta \(en este caso no es necesario el selector\).

  ```text
  <p style="color:blue;">Hola Mundo</p>
  ```

* En la etiqueta `<style>`, dentro de la sección `<head>` del documento HTML.

  ```text
  <!DOCTYPE html>
  <html>
    <head>
      <style>
        p {
          color: blue;
        }
      </style>
    </head>
    ...
  </html>
  ```

* En otro archivo que se referencia en el `<head>` del documento HTML.

  ```text
  <!DOCTYPE html>
  <html>
    <head>
      <link rel="stylesheet" href="style.css">
    </head>
    ...
  </html>
  ```

En general, es preferible crear otro archivo con el código **CSS** y referenciarlo desde el documento **HTML**.

### Selectores CSS <a id="selectores-css"></a>

En una regla **CSS**, el selector es el que nos permite especificar a qué elementos les queremos aplicar las declaraciones \(los estilos\).

Los selectores se pueden especificar por varios criterios, los más importantes son: **por el nombre de la etiqueta, la clase de la etiqueta, o el id de la etiqueta**. Por ejemplo, mira el siguiente código HTML:

```text
<p>La introducción es que ... </p>
<p id="content">El contenido es que ... </p>
<p class="conclusion">La conclusión es que ... </p>
```

¿Cómo podemos cambiarle el color de la fuente al párrafo marcado con la clase “conclusion”? La respuesta es usando **la clase como selector**:

```text
.conclusion {
  color: blue;
}
```

¿Cómo podemos cambiarle el color de la fuente al párrafo marcado con el id “content”? La respuesta es usando el **id como selector**:

```text
#content {
  color: blue;
}
```

¿Cómo podemos cambiarle el tamaño de la letra a todos los párrafos? La respuesta es usando **el nombre de la etiqueta como selector**:

```text
p {
  color: blue;
}
```

Como te puedes dar cuenta de estos ejemplos, las clases se seleccionan usando el prefijo `.`, los id’s se seleccionan usando el prefijo `#`, y las etiquetas no necesitan prefijo.Los selectores son talvez la parte más compleja, y más importante, a la hora de aprender HTML y CSS.

Los selectores se pueden encadenar. Por ejemplo, la siguiente regla le cambia el color de la fuente a todos los elementos `span` que estén dentro de un párrafo y tengan la clase `info`.

```text
p span.info {
  color: blue;
}
```

### Más recursos <a id="m&#xE1;s-recursos"></a>

* [Dash - General Assembly](https://dash.generalassemb.ly/)
* [HTML - Codecademy](https://www.codecademy.com/tracks/web)
* [HTML Tutorial - W3Schools](https://www.w3schools.com/html/default.asp)
* [CSS Tutorial - W3Schools](https://www.w3schools.com/css/default.asp)
* [CSS Dinner - Para que practiques los selectores!](https://flukeout.github.io/)

{% embed url="https://blog.makeitreal.camp/html-css/" %}

