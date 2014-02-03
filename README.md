# HTML Style Guide for *Gang of Five*

We will be using the HTML5 standard.

Based on the [Google HTML Guide](http://google-styleguide.googlecode.com/svn/trunk/htmlcssguide.xml).

# Encoding
 - Use UTF-8, no BOM.
 - Specify the encoding in HTML templates and documents via `<meta charset="utf-8">`.

# Doctype
 - Use the HTML5 doctype

    ~~~html
    <!DOCTYPE html>
    ~~~
    
# Formatting
 - Close all the optionally-closed tags for clarity.
 - Use a new line for every block, list, or table element, and indent every such child element.
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
 
 - Don't close self-closing tags. Also, do not use their old HTML-4 style: `<tag />`.
    ~~~html
    <!-- bad -->
    <img src="hello.jpg" />
    <!-- good -->
    <img src="hello.jpg" />
    ~~~

 - Use 2 spaces for indentation

    ~~~html
    <div class="thumbnail">
      <img src="hello.jpg">
    </div>
    ~~~
 - Use only lowercase for tags and attributes
    ~~~html
    <!-- Bad -->
    <A HREF="/">Home</A>
    <!-- Good -->
    <a href="/">Home</a>
    ~~~
 - Use double ("") rather than single quotation marks ('') around attribute values.

    ~~~html
    <!-- Bad -->
    <a href='/sign-in' class='button'>Sign in</a>
    <!-- Good -->
    <a href="/sign-in" class="button">Sign in</a>
    ~~~
# Misc
 - Do not use type attributes on script tags and stylesheets, since HTML5 always assumes CSS and JavaScript.

    ~~~html
    <!-- Bad -->
    <link rel="stylesheet" href="css/style.css" type="text/css">
    <!-- Good -->
    <link rel="stylesheet" href="css/style.css">
    <!-- Bad -->
    <script src="js/main.js" type="text/javascript"></script>
    <!-- Good -->
    <script src="js/main.js"></script>
    ~~~
