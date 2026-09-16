**Explicación de pseudo clases y identificadores.**


En la página, aparecen dos recursos de CSS que a veces se confunden pero son cosas distintas: uno marca "qué es" un elemento, el otro marca "cómo está" en un momento dado.

**Los ids** son nombres únicos que se le ponen a una etiqueta HTML, tipo `<section id="podcast">`. Desde el CSS se agarran con `#`, entonces `#podcast { padding: 2em; }` le da estilo solo a esa sección. La otra función fuerte que tienen es la navegación interna: un `<a href="#podcast">` salta directo a la sección con ese id. En la página se usaron varios: `inicio`, `podcast`, `premisa`, `causas`, `geopolitica`, `propuestas`, uno por cada bloque de contenido. Un truco aparte es `scroll-margin-top`, que se le pone al id para que al saltar con el link la sección no quede tapada arriba.

**Las pseudoclases** en cambio no nombran nada, describen un estado del elemento en ese instante. Se escriben con `:` después del selector. La que más se ve es `:hover`, que cambia el estilo mientras el cursor está encima, como en `nav a:hover` para los links del menú. También está `:visited` para links ya clickeados y `:focus`, que le pone un contorno al elemento cuando se selecciona con teclado (pensado para accesibilidad). De ejemplo propio se puso `.galeria img:hover { opacity: 0.8; }`, que baja un poco la opacidad de las fotos al pasar el mouse, sin necesitar JavaScript.

La diferencia de fondo: el id apunta a un elemento concreto, la pseudoclase describe una situación temporal de ese elemento.
