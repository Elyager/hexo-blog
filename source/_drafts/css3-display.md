title: css3-display
tags:
---
La propiedad display en CSS nos sirve para determinar cómo se comportará un elemento en el html imaginemos que cada elemento en nuestro sitio es una caja y el display nos determina como se comporta esa caja en el flujo del html y respecto a las demás cajas. 


Por default los tags en html ya tienen definida su propiedad display como los elementos h1,h2,h3 etc. son del tipo block y los elementos tipo a o span por ejemplo son del tipo inline. Para ver más sobre este tema vean [Valores default lo que nadie te dijo](www.google.com)

Acostumbro poner bordes a los contenederes cuandoy estoy maquetando sólo hay que tener cuidad de que estos borde no afecten el flujo los elementos html para eso pueden ver este post de [box-sizing](https://blogdelyager.herokuapp.com/propiedad-box-sizing-css3/) .

Los valores más comunmente usados son:

- block
- inline
- inline-block

    

***block***

Los elementos con esta propiedad se despliegan como bloques tomando todo el ancho disponible y agregando un salto de linea al incio y al final.

***inline***

Los elementos inline se despliegan en linea con los demas elementos elementos como el spam, em y b son del tipo inline. Estos elementos aceptan margin y padding  desplazando elementos horizontalmente **pero no verticalmente**. No se les puede establecer un width y height.


***inline-block***

Los elementos inline-block muy similar a los inline con la única diferencia de que respetan el width y el height a su vez desplazando elementos tanto horizontal como verticalmente.

Ejemplo:

<p data-height="268" data-theme-id="0" data-slug-hash="zxjLeB" data-default-tab="result" data-user="Elyager" class='codepen'>See the Pen <a href='http://codepen.io/Elyager/pen/zxjLeB/'>Displays block, inline, inline-block</a> by Erik Ochoa (<a href='http://codepen.io/Elyager'>@Elyager</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>
