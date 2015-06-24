title: css3-box-sizing
tags:
---
El box-sizing se utiliza para decirle al navegador si se deben de incluir o no los bordes y el padding en las propiedades de tamaño como el width y el height. Por default el borde y el padding no son incluidos **box-sizing: border-content** por lo que sí defines un elemento con un width de 200px y le pones un borde 10px el elemeno final quedaría de 220px de ancho, para solventar este inconveniente se puede usar **box-sizing: border-box** que incluye los bordes y paddings en el tamaño final.

**border-box**
{<1>}![border-box](http://i.imgur.com/vtue6aX.png)
**border-content**
{<2>}![border-content](http://i.imgur.com/1NO5FNL.png)

Puedes probar como estos dos valores funcionan en el siguiente codepen

<p data-height="400" data-theme-id="0" data-slug-hash="VYxGQE" data-default-tab="result" data-user="Elyager" class='codepen'>See the Pen <a href='http://codepen.io/Elyager/pen/VYxGQE/'>Box Model</a> by Erik Ochoa (<a href='http://codepen.io/Elyager'>@Elyager</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

Yo utilizo mucho esta propiedad para cuando estoy maquetando aplicandola a todos los elementos por medio del selector * ya que acostumbro ponerle bordes a los contenedores para visualizarlos de mejor manera.
...language-css
  * {
  -webkit-box-sizing: border-box; /* Safari/Chrome, other WebKit */
  -moz-box-sizing: border-box; /* Firefox, other Gecko */
  box-sizing: border-box; /* Opera/IE 8+ */
  }    
...