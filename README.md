### MÓDULO SOBRE HTML, CSS Y RESPONSIVE DESIGN

1. ¿Qué significa HTML y cuál se su función en el desarrollo web?
    - **HTML**: HyperText Markup Language. Es un lenguaje de marcado que se usa para el desarrollo de páginas de internet. Es el que da la estructura a la página web. 
    - **HTML5**: Es la última versión de HTML. Tiene nuevas etiquetas semánticas como: header, nav, section, article, footer, etc. 

    <strong>Algunas definiciones</strong>

    - **Etiquetas**: Se utilizan para definir la estructura del documento y el contenido de la página web. Se escriben entre corchetes angulares <>. 
    - **Elementos**: Son las etiquetas con su contenido. 
    - **Atributos**: Son las características de las etiquetas. Se escriben dentro de la etiqueta. 
    - **Anidamiento**: Es cuando una etiqueta está dentro de otra etiqueta. 
2.  ¿Cuál es la estructura básica de un documento HTML? Describir las etiquetas 
esenciales.

    - **Estructura básica de un documento HTML**: 
    ```html
    <!DOCTYPE html>
    <html>
    <head>
        <meta charset="utf-8">
        <title>Titulo de la página</title>
    </head>
    <body>
        <p>Mi primer párrafo</p>
    </body>
    </html>
    ```
    **Etiquetas más usadas en HTML**: 
    - **`<p>`**: Párrafo. 
    - **`<h1> a <h6>`**: Títulos. 
    - **`<ul>`**: Lista desordenada. 
    - **`<ol>`**: Lista ordenada. 
    - **`<li>`**: Elemento de una lista. 
    - **`<a>`**: Enlace. 
    - **`<img>`**: Imagen. 
    - **`<table>`**: Tabla. 
    - **`<tr>`**: Fila de la tabla. 
    - **`<td>`**: Columna de la tabla. 
    - **`<div>`**: División o sección de la página. 
    - **`<span>`**: Se utiliza para agrupar texto y aplicarle estilos. 
    - **`<strong>`**: Es para poner el texto en negrita
    - **`<em>`**: Emphasis (accentuación).

    **Etiquetas semánticas**: 
    - **`<header>`**: Encabezado de la página. 
    - **`<nav>`**: Barra de navegación. 
    - **`<section>`**: Sección de la página. 
    - **`<article>`**: Artículo. 
    - **`<aside>`**: Contenido relacionado. 
    - **`<footer>`**: Pie de página.
3.  ¿Qué es CSS y cuál es su proposito en el desarrollo web?

    CSS, Cascading Style Sheets, es un lenguaje utilizado para describir cómo se debe presentar los elementos HTML.
    Los archivos CSS son lenguajes de hojas de estilo que permiten personalizar la apariencia de un sitio web. Estos archivos se utilizan para definir estilos, como colores, fuentes, espaciado, tamaño, etc. 

4. ¿Qué son selectores CSS, cuáles son los principales tipos de selectores y porqué es importante entender la especificidad en el contexto de las hojas de estilo en cascada (CSS)? Describir al menos tres tipos de selectores CSS y cómo la especificidad afecta a la aplicación de estilos en un proyecto de desarrollo web Frontend. Proporcionar ejemplos de situaciones en las que se utiliza la especificidad de selectores para resolver conflictos de estilos.

    Los selectores CSS son patrones utilizados para seleccionar los elementos a los que se desea aplicar un estilo. 
    Existen los selectores de tipo, de clase, de ID, de atributo, etc. 

    La especificidad es un concepto importante en CSS que determina qué estilos se aplican a un elemento cuando hay conflictos de estilo. Por ejemplo, si tienes dos reglas CSS que se aplican al mismo elemento pero tienen diferentes selectores, la regla con el selector de mayor especificidad se aplicará.

    1. **Selector de tipo**: Este selector selecciona elementos por su nombre de etiqueta. Por ejemplo, `p { color: red; }` seleccionará todos los elementos `<p>` y les aplicará un color de texto rojo.

    2. **Selector de clase**: Este selector selecciona elementos por su atributo de clase. Por ejemplo, `.mi-clase { color: blue; }` seleccionará todos los elementos con la clase `mi-clase` y les aplicará un color de texto azul.

    3. **Selector de ID**: Este selector selecciona un elemento por su atributo de ID. Por ejemplo, `#mi-id { color: green; }` seleccionará el elemento con el ID `mi-id` y le aplicará un color de texto verde.

    La especificidad de los selectores puede ser utilizada para resolver conflictos de estilos. Por ejemplo, si tienes un elemento con una clase y un ID, y tienes reglas CSS que se aplican a ambos, la regla con el selector de ID (que tiene mayor especificidad) se aplicará.

    ```css
    selector {
    propiedad: valor;
    propiedad: valor;
    propiedad: valor;
    }
    ```
5.  Explicar las diferencias entre los estilos en línea (inline), estilos internos (embedded) y 
estilos externos (external) en CSS. Indicar cuál de los tres estilos es el recomendado 
usar y por qué.

    Los estilos en CSS pueden ser aplicados de tres formas diferentes: en línea (inline), internos (embedded) y externos (external). Cada uno tiene sus propias características y usos.

    1. **Estilos en línea (Inline)**: Los estilos en línea se aplican directamente a los elementos HTML utilizando el atributo `style`. Por ejemplo: `<p style="color: red;">Este es un párrafo.</p>`. Los estilos en línea tienen la mayor especificidad en CSS, lo que significa que sobrescribirán cualquier otro estilo aplicado al mismo elemento. Sin embargo, los estilos en línea no son reutilizables y pueden hacer que el código HTML sea difícil de leer y mantener.

    2. **Estilos internos (Embedded)**: Los estilos internos se definen en la sección `<head>` de un documento HTML utilizando la etiqueta `<style>`. Los estilos internos se aplican a todo el documento HTML, pero no son reutilizables en otros documentos HTML.

    3. **Estilos externos (External)**: Los estilos externos se definen en un archivo CSS separado que luego se vincula al documento HTML utilizando la etiqueta `<link>`. Los estilos externos son reutilizables en múltiples documentos HTML y son la mejor opción para sitios web grandes y aplicaciones web, ya que permiten una separación clara entre la estructura (HTML) y la presentación (CSS) de la página.

    El uso de estilos externos es generalmente el método recomendado para aplicar CSS, ya que ofrece la mayor reutilización y mantenibilidad. Sin embargo, los otros métodos pueden ser útiles en ciertas situaciones, como cuando se necesita un estilo específico para un solo elemento (estilos en línea) o cuando se está creando una página HTML simple que no requiere un archivo CSS separado (estilos internos).
6. ¿Qué es flexbox y cómo se utiliza para el diseño de páginas web?
7. Explicar cómo se emplean las propiedades flexbox y explicar la función de las 
principales propiedades en la creación de diseños flexibles

    `Respuesta para 6 y 7.` 

    Es un modelo de diseño en CSS que permite organizar y alinear elementos de manera eficiente en diferentes tamaños de pantalla y resoluciones.

    Para utilizar flexbox, se establece un contenedor como flex utilizando la propiedad display: flex;. Los elementos hijos de este contenedor se convierten automáticamente en elementos flexibles y se pueden alinear y distribuir utilizando diversas propiedades de flexbox.

    ```css
    .contenedor {
        display: flex;
        justify-content: space-between;
    }

    .contenedor > div {
        flex: 1;
    }
    ```
    En este ejemplo, todos los elementos div hijos del contenedor se distribuirán uniformemente a lo largo del eje principal del contenedor. Cada div tomará un espacio igual dentro del contenedor gracias a la propiedad flex: 1;.

8. ¿Qué es CSS Grid Layout y en qué se diferencia de flexbox?
9. Proporcionar un ejemplo de cómo crear una cuadrícula sencilla con CSS Grid.

    `Respuesta para 8 y 9`

    Al igual que flexbox este es un modelo que permite controlar tanto las filas como las columnas de la estructura de la página. A diferencia de Flexbox, que es principalmente un modelo de diseño unidimensional (aunque puede manejar dos dimensiones hasta cierto punto), Grid es ideal para diseños que requieren un control más avanzado en ambas dimensiones.

    ```css
    .contenedor {
        display: grid;
        grid-template-columns: auto auto auto;
        grid-gap: 10px;
    }

    .contenedor > div {
        background-color: #ddd;
        padding: 10px;
    }
    ```

    En este ejemplo, el contenedor se configura como una cuadrícula con tres columnas de igual ancho (auto auto auto) y un espacio de 10px entre las celdas de la cuadrícula (grid-gap: 10px). Cada div hijo del contenedor se colocará en una celda de la cuadrícula y tendrá un fondo de color #ddd y un relleno de 10px.

10.¿Qué significa el diseño responsivo en el contexto del desarrollo web?

11.Enumerar al menos tres técnicas o estrategias utilizadas para lograr el diseño responsivo en una página web.

`respuesta 10 y 11`

Es una técnica de diseño web que permite adaptar el sitio web a diferentes resoluciones de pantalla. Esto se logra mediante el uso de diseños flexibles, imágenes flexibles y consultas de medios CSS.

1. Diseño fluido o flexible: Esto implica usar unidades relativas en lugar de unidades absolutas para los anchos de los elementos. Por ejemplo, se utilizan porcentajes en lugar de píxeles para que los elementos se redimensionen en relación con el tamaño de la pantalla.

2. Imágenes flexibles: Las imágenes se redimensionan automáticamente para ajustarse al tamaño de la pantalla. Esto se puede lograr utilizando la propiedad CSS max-width con un valor de 100%.

3. Media Queries de CSS: Las media queries permiten aplicar diferentes estilos a diferentes tamaños de pantalla. Por ejemplo, puedes tener un conjunto de estilos para pantallas pequeñas (como teléfonos móviles) y otro conjunto de estilos para pantallas más grandes (como tablets y escritorios).

```css
@media screen and (max-width: 600px) {
    body {
        background-color: lightblue;
    }
}
```


