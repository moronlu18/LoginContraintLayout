# Uso de Barrier, Guías y Cadenas en ConstraintLayout
En este ejemplo se usa dos guías para añadir un margen a los componentes.

## Guías
Las guías y las barreras tienen varias similituddes ya que son dos elementos que no son visibles al usuario y los componentes se posicionan respecto
a ellos pero las Guías son fijas, se establece en base a una de las siguientes
restricciones:
- Una distancia fija desde la izquierda o la parte superior de un diseño
- Una distancia fija desde la derecha o la parte inferior de un diseño
- Especificar un porcentaje del ancho o alto de un diseño


## Barreras
Las barreras son útiles cuando colocamos una vista a la derecha de otras vistas que están a la izquierda y que tienen diferentes tamaños. En el gif animado hay tres vistas de texto que se establecen dinámicamente
o que muestran contenido generado por el usuario cuyo tamaño no se puede predecir.

<br />

![Barreras](/img/barrier.gif)

En el ejemplo Login, los campos `EditText` se tienen que ajustar cuando se cambia el idioma.
Las cadenas de texto o `TextView`cambian de tamaño ya que en inglés se muestra "**user**" y en español "**nombre de usuario**" de forma que los `EditText` de la derecha se tiene que ajustar según la cadena de texto que se muestre.

![Login en inglés](/img/login_en.png)
![Login en español](/img/login_es.png)
## Cadenas
Cuando se crea una cadena horizontal se añade el atributo `layout_constraintHorizontal_chainStyle` en el primer widget, en nuestro ejemplo es el primer botón de la cadena.
Si fuera una cadena vertical el atributo se coloca en el widget más alto.Por defecto el comportamiento de la cadena cambiará de acuerdo con el estilo especificado cuyo valor predeterminado es `spread` pero en el ejemplo es `packed`.
Puedes ver el funcionamiento de las cadenas en el siguiente gift animado:
<br />
![Cadenas](/img/chain_style.gif)
