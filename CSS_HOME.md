# CSS HOME

CSS es un lenguaje que describe el estilo de un documento HTML.

CSS describe cómo deben mostrarse los elementos HTML.

Este tutorial le enseñará CSS de básico a avanzado.

### Ejemplos en cada capítulo

Este tutorial de CSS contiene cientos de ejemplos de CSS.

Con nuestro editor en línea, puede editar el CSS y hacer clic en un botón para ver el resultado.

#### Ejemplo CSS

```css
body {
  background-color: lightblue;
}

h1 {
  color: white;
  text-align: center;
}

p {
  font-family: verdana;
  font-size: 20px;
}
```
:computer:

## CSS Introduction

### ¿Qué es el CSS?

* **CSS** significa **C** ascading **S** tyle **S** heets
* CSS describe **cómo se deben mostrar los elementos HTML en la pantalla, papel o en otros medios**
* CSS **ahorra mucho trabajo** . Puede controlar el diseño de varias páginas web a la vez
* Las hojas de estilo externas se almacenan en **archivos CSS**

### Demostración CSS - Una página HTML - ¡Múltiples estilos!

Aquí mostraremos una página HTML que se muestra con cuatro hojas de estilo diferentes. Haga clic en los enlaces ""Stylesheet 1", "Stylesheet 2", "Stylesheet 3", "Stylesheet 4" a continuación para ver los diferentes estilos:

<img src="images/1-page-1.png">

<img src="images/1-page-2.png">

<img src="images/1-page-3.png">

<img src="images/1-page-4.png">

<img src="images/1-page-5.png">

### ¿Por qué usar CSS?

CSS se utiliza para definir estilos para sus páginas web, incluido el diseño, el diseño y las variaciones de visualización para diferentes dispositivos y tamaños de pantalla.

#### Ejemplo CSS

```css
body {
  background-color: lightblue;
}

h1 {
  color: white;
  text-align: center;
}

p {
  font-family: verdana;
  font-size: 20px;
}
```

:computer:

### CSS resolvió un gran problema

¡HTML nunca tuvo la intención de contener etiquetas para formatear una página web!

HTML fue creado para **describir el contenido** de una página web, como:

`<h1>` Este es un encabezado `</h1>`

`<p>` Este es un párrafo. `</p>`

Cuando se agregaron etiquetas como `<font>` y atributos de color a la especificación HTML 3.2, comenzó una pesadilla para los desarrolladores web. El desarrollo de sitios web grandes, donde se agregaron fuentes e información de color a cada página, se convirtió en un proceso largo y costoso.

Para resolver este problema, el Consorcio World Wide Web (W3C) creó CSS.

¡CSS eliminó el formato de estilo de la página HTML!

### ¡CSS ahorra mucho trabajo!

Las definiciones de estilo se guardan normalmente en archivos externos `.css`.

¡Con un archivo de hoja de estilo externo, puede cambiar el aspecto de un sitio web completo cambiando solo un archivo!

## Sintaxis CSS

### Sintaxis CSS

Un conjunto de reglas CSS consta de un selector y un bloque de declaración:

<img src="images/1-sintaxis.png">

El selector apunta al elemento HTML que desea diseñar.

El bloque de declaración contiene una o más declaraciones separadas por punto y coma.

Cada declaración incluye un nombre de propiedad CSS y un valor, separados por dos puntos.

Una declaración CSS siempre termina con un punto y coma, y los bloques de declaración están rodeados por llaves.

#### Ejemplo

En este ejemplo, todos los elementos `<p>` estarán alineados al centro, con un color de texto rojo:

```css
p {
  color: red;
  text-align: center;
}
```

:computer:

Ejemplo explicado

* `p` es un **selector** en CSS (apunta al elemento HTML que desea diseñar: `<p>`).
* `color`es una propiedad y `red`es el valor de la propiedad
* `text-align`es una propiedad y `center`es el valor de la propiedad

## CSS Selectors (Selectores CSS)

Los selectores CSS se utilizan para "encontrar" (o seleccionar) los elementos HTML que desea diseñar.

Podemos dividir los selectores CSS en cinco categorías:

* **Simple selectors** (seleccione elementos basados en name, id, class)
* **Combinator selectors** (seleccione elementos basados en una relación específica entre ellos)
* **Pseudo-class selectors** (seleccione elementos basados en un cierto estado)
* **Pseudo-elements selectors** (seleccionar y diseñar una parte de un elemento)
* **Attribute selectors** (seleccione elementos basados en un atributo o valor de atributo)

Esta página explicará los selectores CSS más básicos.

### El CSS element Selector (Selector de elementos CSS)

El selector de elementos selecciona elementos HTML en función del nombre del elemento.

#### Ejemplo

Aquí, todos los elementos `<p>` de la página estarán alineados al centro, con un color de texto rojo: 

```css
p {
  text-align: center;
  color: red;
}
```

:computer:

### El CSS id Selector Selector id CSS)

El selector `id` utiliza el atributo `id` de un elemento HTML para seleccionar un elemento específico.

El `id` de un elemento es única dentro de una página, por lo que el selector `id` se usa para seleccionar un elemento único!

Para seleccionar un elemento con un `id` específico, escriba un carácter hash (#), seguido de la identificación del elemento.

#### Ejemplo

La siguiente regla CSS se aplicará al elemento HTML con `id = "para1"`: 

```css
#para1 {
  text-align: center;
  color: red;
}
```

:computer:

**Nota:** ¡Un id name no puede comenzar con un número!

### El CSS class Selector (Selector class)

El selector class selecciona elementos HTML con un atributo `class` específico.

Para seleccionar elementos con una clase específica, escriba un carácter de punto (.), Seguido del nombre de la clase.

#### Ejemplo

En este ejemplo, todos los elementos HTML con `class = "center"` serán rojos y alineados al centro: 


```css
.center {
  text-align: center;
  color: red;
}
```

:computer:

También puede especificar que solo los elementos HTML específicos se vean afectados por una clase.

#### Ejemplo

En este ejemplo, solo los elementos `<p>` con `class = "center"` estarán alineados al centro: 

```sh
p.center {
  text-align: center;
  color: red;
}
```

:computer:

Los elementos HTML también pueden referirse a más de una clase.

#### Ejemplo

En este ejemplo, el elemento `<p>` se diseñará de acuerdo con `class = "center"` y a `class = "large"`: 

```sh
<p class="center large">This paragraph refers to two classes.</p>
```

:computer:

**Nota:** ¡Un nombre de clase no puede comenzar con un número!

### El CSS Universal Selector

El selector universal (`*`) selecciona todos los elementos HTML en la página.

#### Ejemplo

La siguiente regla CSS afectará a cada elemento HTML en la página: 

```css
* {
  text-align: center;
  color: blue;
}
```

:computer:


### El CSS Grouping Selector (Selector de Agrupación)

El selector de agrupación selecciona todos los elementos HTML con las mismas definiciones de estilo.

Mire el siguiente código CSS (los elementos `h1`, `h2` y `p` tienen las mismas definiciones de estilo):

```css
h1 {
  text-align: center;
  color: red;
}

h2 {
  text-align: center;
  color: red;
}

p {
  text-align: center;
  color: red;
}
```

Será mejor agrupar los selectores para minimizar el código.

Para agrupar selectores, separe cada selector con una coma.

#### Ejemplo

En este ejemplo, hemos agrupado los selectores del código anterior: 

```css
h1, h2, p {
  text-align: center;
  color: red;
}
```

:computer:

### ¡Ponte a Prueba con Ejercicios!

:computer: :computer: :computer: :computer:

### Todos CSS Simple Selectors

Selector | Example | Example description
---------|---------|--------------------
`.class` | `.intro` | Selecciona todos los elementos con `class = "intro"`
`#id` | `#firstname` | Selecciona el elemento con `id="firstname"`
`*` | `*` | Selecciona todos los elementos.
`element` | `p` | Selecciona todos los elementos `<p>`
`element,element,..` | `div, p` | Selecciona todos los elementos `<div>` y todos los elementos `<p>`

## Como Añadir CSS

Cuando un navegador lee una hoja de estilo, está formateará el documento HTML de acuerdo con la información en la hoja de estilo.

### Tres Formas de Insertar CSS

Hay tres formas de insertar una hoja de estilo:

* CSS externo
* CSS interno
* CSS en línea

### CSS externo

¡Con una hoja de estilo externa, puede cambiar el aspecto de un sitio web completo cambiando solo un archivo!

Cada página HTML debe incluir una referencia al archivo de hoja de estilo externo dentro del elemento `<link>`, dentro de la sección de encabezado(head) .

#### Ejemplo

Los estilos externos se definen dentro del elemento `<link>`, dentro de la sección `<head>` de una página HTML:

```css
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
<body>

  <h1>This is a heading</h1>
  <p>This is a paragraph.</p>

</body>
</html>
```

:computer:


Se puede escribir una hoja de estilo externa en cualquier editor de texto y se debe guardar con una extensión .css.

El archivo externo .css no debe contener ninguna etiqueta HTML.

Así es como se ve el archivo "mystyle.css":

#### "mystyle.css"

```css
body {
  background-color: lightblue;
}

h1 {
  color: navy;
  margin-left: 20px;
}
```

**Nota**: No agregue un espacio entre el valor de la propiedad y la unidad (como `margin-left: 20 px;`). La forma correcta es: `margin-left: 20px;`

### CSS interno

Se puede usar una hoja de estilo interna si una sola página HTML tiene un estilo único.

El estilo interno se define dentro del elemento `<style>`, dentro de la sección del encabezado.

#### Ejemplo

Los estilos internos se definen dentro del elemento `<style>`, dentro de la sección `<head> de una página HTML:
  
```css
<!DOCTYPE html>
<html>
<head>
  <style>
    body {
      background-color: linen;
    }

    h1 {
      color: maroon;
      margin-left: 40px;
    }
  </style>
</head>
<body>

  <h1>This is a heading</h1>
  <p>This is a paragraph.</p>

</body>
</html>
```

:computer:

### CSS Inline

Se puede usar un estilo inline para aplicar un estilo único para un solo elemento.

Para usar estilos inline, agregue el atributo `style` al elemento relevante. El atributo `style` puede contener cualquier propiedad CSS.

#### Ejemplo

Los estilos inline se definen dentro del atributo `style` del elemento relevante:

```css
<!DOCTYPE html>
<html>
<body>

  <h1 style="color:blue;text-align:center;">This is a heading</h1>
  <p style="color:red;">This is a paragraph.</p>

</body>
</html>
```

:computer:

**Tip**: Un estilo inline pierde muchas de las ventajas de una hoja de estilo (al mezclar contenido con presentación). Use este método con moderación.

### Múltiples Hojas de Estilo (Style Sheets)

Si se han definido algunas propiedades para el mismo selector (elemento) en diferentes hojas de estilo, se utilizará el valor de la última hoja de estilo leída. 

Suponga que una **hoja de estilo externa** tiene el siguiente estilo para el elemento `<h1>`:

```css
h1 {
  color: navy;
}
```

Luego, suponga que una **hoja de estilo interna** también tiene el siguiente estilo para el elemento `<h1>`:
  
```css
h1 {
  color: orange;   
}
```

#### Ejemplo

Si el estilo interno se define **después** del enlace a la hoja de estilo externa, los elementos `<h1>` serán `"orange"`:

```css
<head>
  <link rel="stylesheet" type="text/css" href="mystyle.css">
  <style>
    h1 {
      color: orange;
    }
  </style>
</head>
```

:computer:

#### Ejemplo

Sin embargo, si el estilo interno se define **antes** del enlace a la hoja de estilo externa, los elementos `<h1>` serán `"navy"`: 
  
```css
<head>
  <style>
    h1 {
      color: orange;
    }
  </style>
  <link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
```

:computer:

### Orden en Cascada

¿Qué estilo se usará cuando haya más de un estilo especificado para un elemento HTML?

Todos los estilos de una página se "encadenarán" en una nueva hoja de estilo "virtual" según las siguientes reglas, donde el número uno tiene la máxima prioridad:

1. Estilo en línea (dentro de un elemento HTML)
2. Hojas de estilo externas e internas (en la sección head)
3. Navegador predeterminado

Por lo tanto, un estilo en línea tiene la máxima prioridad y anulará los estilos externos e internos y los valores predeterminados del navegador.

:computer:

### ¡Ponte a prueba con ejercicios!

:computer: :computer: :computer: :computer:

## CSS Comments
## CSS Colors
## CSS Backgrounds
## CSS Borders
## CSS Margins
## CSS Padding
## CSS Height/Width
## CSS Box Model
## CSS Outline
## CSS Text
## CSS Fonts
## CSS Icons
## CSS Links
## CSS Lists
## CSS Tables
## CSS Display
## CSS Max-width
## CSS Position
## CSS Overflow
## CSS Float
## CSS Inline-block
## CSS Align
## CSS Combinators
## CSS Pseudo-class
## CSS Pseudo-element
## CSS Opacity
## CSS Navigation Bar
## CSS Dropdowns
## CSS Image Gallery
## CSS Image Sprites
## CSS Attr Selectors
## CSS Forms
## CSS Counters
## CSS Website Layout
## CSS Units
## CSS Specificity
