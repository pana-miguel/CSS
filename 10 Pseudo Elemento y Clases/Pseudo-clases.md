# Pseudo Clases

las pseudo-clases se usan para definir un estado especial de un elemento.

Por ejemplo aplicar estilos cuando el usuario de click a un elemento o cuando pase el cursos por encima de un elemento.

## Sintaxis

```css
selector:pseudo-class{
	propiedad: valor;
}
```

---

* :hover
  La pseudo-clase hover se utiliza cuando el usuario pasa el cursos  por encima del elemento, pero no nesesariamente activandolo.

  ```css
  a:hover{
  	color: orange;
  }
  ```
* :link
  La pseudo-clase link se usa cuando un elemento que aun no fue visitado. esta pseudo clase es usada por defecto en las etiquetas `<a>`, `<area>` y `<link>`.

  ```css
  a:link {
  	color: red;
  }
  ```
* :visited
  La pseudo-clase visited , representa enlaces que ya fueron visitados por el usuario. Por motivos de privacidad, lo estilos que se pueden modificar son muy limitados.

  ```css
  a:visited{
  	color:green;
  }
  ```
* :active
  La pseudo-clase activate representa cuando un usuario a activo un elemento, por lo general se trata de un boton. La activacion comienza cuando el usuario da un click en el elemento, recordar que los estilos se aplican mientras se de click, cuando se suelte volvera con los estilos predefinidos.

  ```css
  a:active{
  	color: blue;
  }
  ```
* :focus la pseudo-clase focus representa un elemento que
* :lang
