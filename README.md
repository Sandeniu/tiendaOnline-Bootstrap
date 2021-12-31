# tiendaOnline-Bootstrap
Se re-construye desde cero el proyecto TiendaOnline-sandraUlloa , para hacerlo con Bootstrap

notas:
nav de bootstrap, con borde inferio y color personalizado
<nav class="navbar navbar-expand-lg navbar-light border-1 border-bottom border-info"
            style="background-color: #FEEFDD;">

git commit -m "Aplicación de Sass II"
==========map-get()==========
se declara el mapa $fontNormal y luego se llama a sus key con map-get() en los siguientes partial
scss/componentes/elementos
scss/componentes/footer

==========extends==========
de la clase madre divCard, se extienden las clases .divCardProductoDestacado y 
.divCardProductoNormal, estas clase son incluidas en el siguiente partial:
scss/proveedores/bootstrap/card-productos

==========mixin==========
*Se crea e incorpora la función @mixin_flexColumn en los siguientes parciales:
scss/componentes/main;
scss/proveedores/bootstrap/card-productos;
scss/proveedores/bootstrap/bs-form;
scss/componentes/footer;
scss/vistas/productos/productos-aside;
scss/responsive/1.xs;
scss/responsive/2.sm;

*Se crea e incorpora la función @mixin _flexRow en los siguientes parciales:
scss/vistas/index/index-section1;
scss/proveedores/bootstrap/card-text-white; 
scss/componentes/footer;
scss/vistas/productos/productos-section1;
scss/responsive/1.xs;
scss/responsive/2.sm;
scss/responsive/3.md;

*Se crea e incorpora la función @mixin _font-h en los siguientes parciales:
scss/componentes/elementos

*Se crea e incorpora la función @mixin _animation-scale en los siguientes parciales:
scss/componentes/nav";
scss/proveedores/bootstrap/card-productos;

*Se crea e incorpora la función @mixin _animation-rotate en los siguientes parciales:
scss/vistas/productos/productos-aside

// Fin aplicación de Sass II
