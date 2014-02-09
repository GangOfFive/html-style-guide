
# Estándar de HTML para *Gang of Five*

Se utilizará el estándar de HTML5.

Basado en [Google HTML Guide](http://google-styleguide.googlecode.com/svn/trunk/htmlcssguide.xml).

## Codificación
 - Utilizar UTF-8, sin BOM.
 - Especificar la codificación en documentos HTML y *templates*, utilizando `<meta charset="utf-8">`.

## Doctype
 - Utilizar el *doctype* de HTML5.

    ~~~html
    <!DOCTYPE html>
    ~~~
    
## Formato
 - Cerrar todas las etiquetas opcionales por claridad.
 - Utilizar una línea nueva para cada elemento de bloque, lista, o tabla, e indentar cada elemento hijo.
    ~~~html
    <blockquote>
      <p><em>Space</em>, the final frontier.</p>
    </blockquote>
    <ul>
      <li>Moe</li>
      <li>Larry</li>
      <li>Curly</li>
    </ul>
    <table>
      <thead>
        <tr>
          <th scope="col">Income</th>
          <th scope="col">Taxes</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>$ 5.00</td>
          <td>$ 4.50</td>
        </tr>
      </tbody>
    </table>
    ~~~
 
 - No cerrar las etiquetas que se cierran solas.
   Tampoco utilizar: `<tag />`:
    ~~~html
    <!-- No recomendado -->
    <img src="hello.jpg" />
    <!-- No recomendado -->
    <img src="hello.jpg"></img>
    <!-- Recomendado -->
    <img src="hello.jpg" />
    ~~~

 - Utilizar `2` espacios para la indentación:

    ~~~html
    <div class="thumbnail">
      <img src="hello.jpg">
    </div>
    ~~~
 - Utilizar solamente minúsculas para etiquetas y atributos:

    ~~~html
    <!-- No recomendado -->
    <A HREF="/">Home</A>
    <!-- Recomendado -->
    <a href="/">Home</a>
    ~~~

 - Utilizar comillas dobles `""` en vez de simples `''` para los atributos:

    ~~~html
    <!-- No recomendado -->
    <a href='/sign-in' class='button'>Sign in</a>
    <!-- Recomendado -->
    <a href="/sign-in" class="button">Sign in</a>
    ~~~
## Otros
 - No utilizar el atributo `type` para etiquetas `script` y hojas de estilo, ya que HTML5 siempre asume CSS y JavaScript.

    ~~~html
    <!-- No recomendado -->
    <link rel="stylesheet" href="css/style.css" type="text/css">
    <!-- Recomendado -->
    <link rel="stylesheet" href="css/style.css">
    <!-- No recomendado -->
    <script src="js/main.js" type="text/javascript"></script>
    <!-- Recomendado -->
    <script src="js/main.js"></script>
    ~~~
