# Reto : Kitten

## Objetivo 
Crea una página web donde se muestre un paisaje y un gatito diferente a medida que la ventana del navegador se haga más pequeña. Las vistas se deben ver de la siguiente manera.

![Con titulo](docs/kitten-dawn.png "titulo")
![Con titulo](docs/kitten-night.png "titulo")
![Con titulo](docs/kitten-sunnyday.png "titulo")


## Recursos brindados
Se brindo las 3 imágenes de los escenarios y las 3 imágenes de gatos en diferentes posiciones.

## Desarrollo del Reto

Para el desarrollo de este reto se ha necesitado de la investigación de una nueva etiqueta en html  `<picture>`, ya que se necesitaba cambiar la imagen de acuerdo a la resolución de la pantalla.
Se aplico de la siguiente manera.

```html 
<picture>
        <source media="(min-width: 992px)" srcset="assets/images/kitten-large.png">
        <source media="(min-width: 768px)" srcset="assets/images/kitten-small.png">
        <img src="assets/images/kitten-medium.png" alt="kitten" style="width:auto;">
    </picture>
```
Dentro de la etiqueta   `<source media=''>` he colocado la resolución de los dispositivos que se va tener en cuenta para cambiar las imágenes.
Esta información la obtuve gracias al siguiente link : [W3schools](https://www.w3schools.com/tags/tag_picture.asp "titulo").

Asimismo, con esta etiqueta `<picture>` se han establecido el orden de las imágenes de los gatos, pero el fondo de cada uno se estableció en la hoja de estilos CSS utilizando Media Queries.
