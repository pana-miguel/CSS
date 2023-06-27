# Position

la propiedad position que se utiliza para saber la posicion de una caja, exiten 5 valores para este propiedad que son :

* static
  Los elementos html por defecto traen la propiedad position static, los elementos estaticos no se ven afectados por las propiedades de top, bottom, left y right.
  Los elementos que posen este valor no estan posicionados de ninguna manera especial; se posicionan de acuerdo con el flujo normal del DOM.

  ```css
  mi-box{
  	position: static;
  }
  ```
* relative

  Los elementos que se posicionan con relacion a su posicion normal, esta valor permite incluir las propiedades de top, bottom, left, right.

  Esta propiedad conserva todas las propiedades de la caja como medidas, border,etc;

  ![1686870821589](image/position/1686870821589.png)

  Como vemos el segundo div se quedo en su lugar como si el primer div ocupara su espacio, esto es lo que relative nos da, modificar su posicion sin afectar el espacio ocupado.
* fixed

  El valor fixed proporciona a la caja una posicion en la relacion a la ventana grafica, lo que significa que siempre para en el mismo lugar; tambien se pueden usar las propieddes top, bottom, left y right.
  La propiedad fixed eliminar la el espacio que ocupaba, dandole el paso a otro elemento en el flujo del DOM.

  ![1686872825810](image/position/1686872825810.png)
* absolute:

  El valor absolute se coloca en relacion a la anterior caja, el elemento es removido del flujo del DOM; es como un relative fucionado con fixed; en resume la caja dejara de ocupar su espacio y pasara a quedar fijo en un lugar con las propiedades top, right, bottom, y left.

  ```css
  mi-elemento{
  	position: absolute;
  	top: 40px;
  	left: 50px;
  	background: red;
  }
  ```
* sticky: (experimental, se espera que en un futuro cambie)

  Esta propiedad nos da una conbinacion entre 'relative' y 'fixed', que solo desplaza como un 'fixed' en su caja contenedora, de ahi se comporta como un 'relative'.

  ```css
  mi-element{
  	position: sticky;
  	top: 0;
  	background-color: green;
  }
  ```

  ![1686890345270](image/position/1686890345270.png)

## Z INDEX

El 'z-index' nos sirve para poder ordenar elementos superposicionados uno detras de otros, esta propiedad nos ayudara a darle un orden segun el valor que le dasmos.

```html
<!DOCTYPE html>
<html>
<body>
	<h1>This is a heading</h1>
	<img src="img_tree.png">
	<p>Because the image has a z-index of -1, it will be placed behind the text.</p>
</body>
</html>

```

```css
img {
	position: absolute;
	left: 0px;
	top: 0px;
 	z-index: -1;
}
```

![1686891666625](image/position/1686891666625.png)
