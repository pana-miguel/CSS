# Metodología BEM

La mtodologia BEM que se encarga de evitar conflictos de especifidad, esta metodologia se basa en el nombre de la clase padre.

Esta metodologia nos ayuda en:

* Evitar conflicto de especificidad.
* Evitar seleccionar muchas clases.
* Nos basamos en el nombre de la clase para poder manejar bien los estilos.
* Añade especificidad: Usa un selector único para cada regla, lo que permite reducirla y hacer menos repeticiones.
* Mejora la herencia múltiple: Se puede cambiar cualquiera de las tres partidas sin afectar a las demás.
* Permite la reutilización: Es posible reciclar ciertas áreas de código desde un proyecto hacia otro, esto debido a la no existencia de dependencias mayores en cuanto a la implementación de cada uno de los bloques estructurados.

```html
<section>
    <article class="noticia--destacada">
        <h1 class="noticia_titulo--uppercase">Titulo de la noticia</h1>
    </article>
</section>
```

```css
.noticia--destacada{
    background: red;
}
 .noticia_titulo-uppercase{
    text-transform: uppercase;
}
```

___

* [Como usar la Metodologia BEM](https://blog.ida.cl/desarrollo/metodologia-bem-desarrollo-front-end/)
