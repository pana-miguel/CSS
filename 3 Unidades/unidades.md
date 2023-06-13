# Unidades

En CSS tenemos 2 unidades de medida:

* Las relativas .- son medidas que dependen de algo y varian segun algo.

  ```css
  .contac-form-h2{
  	font-size: 2em;
  }
  ```

  La medida `em` por defecto son `16px`.

  Las medidas relativas nos ayuda a nuestro contenido se adapte a la resolucion de nuestra pantalla, permitiendo lo que se conoce como responsive desing.
* Las Fijas .- son medidas establecidas que no varian como los cm, m , km, etc.

  ```css
  .contac-form__h2{
  	font-size: 23px;
  }
  ```

  cuando se trabaja con medidas fijas la caja se quedas con una medida constante, cosa que si pasamos de una resolucion mas pequeña, lacaja seguira midiendo el valor fijo como 2cm, y esto no es bueno por que necitamos que nuestra caja se adapte a nuestra pantalla.
