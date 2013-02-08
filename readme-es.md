# EC Stars Rating #

El plugin de calificación por estrellas más ligero que podrás encontrar.

## Descripción ##

Un plugin de calificación por estrellas para WordPress **super rápido**, optimizado para el SEO, y con muy poco impacto en el tiempo de carga de la página (sólo usa CSS, un poco de HTML, y el JavaScript estrictamente necesario para su funcionamiento). Ni una sóla imagen!

## Instalación ##

1. Sube el contenido del zip al directorio `/wp-content/plugins/`
2. Activa el plugin desde el menú 'Plugins' en WordPress
3. Configura el plugin según tus necesidades. Si necesitas ayuda o información extra sobre la configuración puedes visitar [http://emiliocobos.net/ec-stars-rating-wordpress-plugin/](la página del plugin)
4. Pon la siguiente línea de código donde quieras que aparezcan las estrellas en tu tema (normalmente en `single.php`, `content-single.php` o `index.php`):

```php
<?php if(function_exists('ec_stars_rating')) {
		ec_stars_rating();
	} ?>
```

## Preguntas frecuentes ##

### ¿Qué formato de marcado debería de usar? ###

Actualmente, microdata es el recomendado por Google, pero con microformats Google detecta las estrellas y las usa en tus búsquedas ([https://www.google.com/search?q=site:emiliocobos.net+ec+stars+rating](ejemplo)).

## Screenshots ##

1. Funcionamiento básico del plugin

## Changelog ##

### 1.0 ###
Primera versión estable, con algunos errores de formato de los números arreglados.