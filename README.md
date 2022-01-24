Enlace a servidor Firebase:
https://dulce-capricho-chile.web.app


24/01/2022 git commit -m "Entrega de proyecto front-end"

Cambios realizados en este commit:
1) Páginas:
    • index.html: Se incorporan imágenes faltantes en main > section. Se gestiona el responsive de la página.
    • productos.html: Se incorporan imágenes faltantes en main > section. Se gestiona el responsive de la página.
    • servicios.html: Se gestiona el responsive de la página.
    • despachos.html: se asignan fondo bordes y sombras a la página. Se gestiona el responsive de la página.
    • nosotros.html: se le asignan gradienes, bordes, sombras y animaciones a la página. Se gestiona el responsive de la página.

2) Estandarización de saas:
   • Para tener una mejor visión se enumeran las carpetas que conforman scss, siguiendo es modelo 7+1
   • Se crean 3 mixin con parámetros, que corersponden a las propiedades más recurrentes.  
       A continuación se indica el nombre del mixin y propiedades css que se utilizan como parámetros:
     - letra-personalizada (text-align, font-size, color, letter-spacing, text-decoration, font-family,  text-transform, font-weight)
     - display-flex (display, flex-direccion, flex-wrap, justify-content, align-item, gap)
     - divEncabezado  (text-align, width, height, padding, margin, background, border);
   • Boorado de mixin:  
     - mapa $fontNormal --> es reemplazado por mixin "letra-personalizada".
     - flexColumn --> es reemplazado por mixin display-flex.
     - flexRow --> es reemplazado por mixin display-flex.

3) Gestión en componentes de estructura html:
    • Nav: 
      - Logo: Se incorpora el logo del nav, el cual al darle click enlaza al home
      - Cambio en la distribución del menú: hamburguesa + logo (en ese orden) se mueven a la izquierda de la página.
      - Se fija el menú para mantenerlo siempre visible: para ello se incorpora la clase "sticky-top" de bootstrap.
    • Footer: se optimiza el footer incorporando dentro del menú (ul > li) todos los elementos que funcionaban por separado; eliminando así problemas de alineación e incongruencias en el aspecto responsive.

4) Gestión de elaboración de componentes (inpirado en otras páginas): 
    • card-image-duplex: 
      Se trata de una imagen principal que al hacerle hover, se depliega sobre ella una imagen secundadria.
      Utilizada en página index.html > main> secction # 1 > productos destacados. 
    • card-Postal: 
      Tarjeta horizontal tipo esquela.
      Utilizada en página servicios.html > main > section # 1 
    • card-Publicidad:
      Utilizada en página index.html > main> aside > divPublicidad. 

5) Gestión de enlaces: Para los enlaces que se relacionan con páginas que aun no están construidas, se elabora una ventana emergente que indica "Sitio en Construcción". Se trata de una sección dentro de la misma página, la cual es referenciada con enlace interno mediante su #id.


=====================================================================

git commit -m "Aplicación de Sass II"
==========map-get()==========
se declara el mapa $fontNormal y luego se llama a sus key con map-get() en los siguientes partial
scss/componentes/elementos
scss/componentes/footer

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

========================================================================

# tiendaOnline-Bootstrap
Se re-construye desde cero el proyecto TiendaOnline-sandraUlloa , para hacerlo con Bootstrap

notas:
nav de bootstrap, con borde inferior y color personalizado
<nav class="navbar navbar-expand-lg navbar-light border-1 border-bottom border-info"
            style="background-color: #FEEFDD;">
======================================================================
git commit -m "Mejoras para SEO" 
- Se modifica las etiquetas <title> dentro de las páginas, para poner un título descriptivo y personalizado segun la página

- Se incorpora en cada página, la etiqueta <meta name="description"> en ella se incorpora un párrafo descriptivo con respecto a la misión de la página. 

- Se incorpora en cada página, la etiqueta <meta name="keywords">. En el content de esta etiqueta se incorporan las palabras claves que puedan llegar aser utilizadas por los usuarios en los buscadores y meta-buscadores.


