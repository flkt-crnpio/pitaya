# Pitaya
La más impresionante librería de CSS, 
jajaja, no.

En [flkt.mx/pitaya](http://flkt.mx/pitaya/index.html) puedes ver cómo funciona la librería.
Si así te gusta, el archivo final esta en dist/pitaya.min.css, puedes copiar y pegar directo en tu proyecto.

## Edición
Instala [SASS](http://sass-lang.com/) si aún no lo tienes.

Si quieres editarle algo, la mayoría de las cosas estan en variables, 
puedes ir a src/_vars.sass y editar los valores de la fuente, el color, el margen, el borde... 

Los archivos de cada componente estan guardados en carpetas iguales a la documentación dentro de la carpeta src/ del proyecto.
Edita lo que necesites en SASS y para ver los cambios ve a la carpeta de docs y abre el html en el navegador... 
(jejeje lo siento, no le puse gulp)
```sh
sass --watch src/pitaya.sass:dosc/css/pitaya.css --style expanded
```

Para obtener el archivo de distribución de la carpeta dist/
```sh
sass src/pitaya.sass:dist/pitaya.min.css --style compressed
```
