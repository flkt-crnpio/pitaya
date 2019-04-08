# Pitaya #
La más impresionante librería de CSS, jajaja, no.


## Uso ##
Puedes utilizar directamente los archivos de distrubución para usar tal cual la librería como está. Los puedes descargar desde el index de la documentación [github.io/pitaya](http://flkt-crnpio.github.io/pitaya/) o bajar el proyecto de github y buscar los archivos de css

#### Archivos ####
```text
mol.colors/
├── dist/
    ├── pitaya.min.css
    └── pitaya.min.css.map
├── docs/
    ├── css/
        ├── pitaya.css
        └── pitaya.css.map
    ├── dist/
        ├── pitaya.min.css
        └── pitaya.min.css.map
    ├── img/
        ├── gallery/
        ├── profile/
     	└── GitHub-Mark-Light-32px.png
    ├── auxiliares.html
    ├── componentes.html
    ├── composicion.html
    ├── cuadricula.html
    ├── index.html
    ├── navegacion.html
    └── nucleo.html
└── scss/
    ├── components/
    	├── badge.sass
	├── breadcrumb.sass
	├── card.sass
	├── collapsable.sass
	├── divider.sass
	├── tab.sass
	└── tag.sass
    ├── core/
	├── button.sass
	├── form.sass
	├── link.sass
	├── list.sass
	├── table.sass
	└── typography.sass
    ├── helper/
    	├── align.sass
	└── colors.sass
    ├── layout/
    	├── col.sass
    	├── flex.sass
    	├── layout.sass
    	├── pin.sass
	└── row.sass
    ├── navigation/
    	├── navbar.sass
	├── navmenu.sass
	└── sidenavbar.sass
    ├── _mixings.sass
    ├── _normalize.sass
    ├── _vars.sass
    └── pitaya.sass
```

#### Edición ####
Únicamente necesitas tener instalado [SASS](http://sass-lang.com/) y el proyecto descargado.


Todos los archivos de la librería se encuentran dentro de la carpeta `src/`


#### Variables ####
Algunas propiedades están en variables que puedes editar desde el archivo de `src/_vars.sass`
```text
// media queries
$phone:     20rem
$phone-l:   30rem
$tablet:    48rem
$laptop:    64rem
$MDPI:      75rem
$HiDPI:     90rem
$HD:        120rem

// texto
@import url(https://fonts.googleapis.com/css?family=Roboto:400,300,700,100)
@import url(https://fonts.googleapis.com/css?family=Arvo)
$font-family:       'Roboto', Arial, Helvetica, sans-serif
$font-line:         1.6em
$font-size:         16px
$font-weight:       300
$code-font:         monospace
$title-font:        'Arvo', Georgia, serif
$title-line:        1em
$title-weight:      400

// color
$main-background:   #191828
$main-color:        #efedef
$color-primary:     #fd264f
$color-accent:      #0de084
$color-white:       #dddddd
$color-black:       #333333

// bordes
$border-radius:     1px
$border-width:      1px

// espacio entre elementos
$layout-space:      2rem

// espacio de la cuadrícula
$grid-space:        2vw
$grid-space-inside: 2vw

// ancho de contenedores
$width-phone:       90%
$width-tablet:      90%
$width-laptop:      80%
$width-HD:          80%
$width-max:         auto

// alto del menú
$navbar-height:     60px

```

#### Visualizacion ####
Para poder ver los cambios que hiciste, corre en la terminar el comando de abajo y abre los archivos de html dentro de la carpeta `docs/`
```sh
sass --watch src/pitaya.sass:dosc/css/pitaya.css --style expanded
```


#### Usar mi propio archivo ####
Para obtener el archivo de minificado, corre en la terminar el comando de abajo y utiliza en tu proyecto los archivos de css que estan dentro de la carpeta `dist/`
```sh
sass src/pitaya.sass:dist/pitaya.min.css --style compressed
```
