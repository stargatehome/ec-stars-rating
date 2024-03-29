=== EC Stars Rating ===
Contributors: ecoal95
Donate link: http://emiliocobos.net/donar/
Tags: stars, rating, posts rating
Requires at least: 3.0
Tested up to: 3.5.1
Stable tag: 1.0
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

El plugin de calificación por estrellas más ligero que podrás encontrar en el directorio

== Description ==

Un plugin de calificación por estrellas para WordPress **super rápido**, optimizado para el SEO, y con muy poco impacto en el tiempo de carga de la página (sólo usa CSS, un poco de HTML, y el JavaScript estrictamente necesario para su funcionamiento). Ni una sóla imagen!

== Installation ==

1. Sube el contenido del zip al directorio `/wp-content/plugins/`
2. Activa el plugin desde el menú 'Plugins' en WordPress
3. Configura el plugin según tus necesidades. Si necesitas ayuda o información extra sobre la configuración puedes visitar [la página del plugin](http://emiliocobos.net/ec-stars-rating-wordpress-plugin/)
4. Pon la siguiente línea de código donde quieras que aparezcan las estrellas en tu tema (normalmente en `single.php`, `content-single.php` o `index.php`):

	<?php if(function_exists('ec_stars_rating')) {
		ec_stars_rating();
	} ?>

5. Adicionalmente, si sólo quieres mostrar las estrellas en un post en particular, puedes usar el siguiente shortcode:
	
	[ec_stars_rating]

== Frequently asked questions ==

= ¿Qué formato de marcado debería de usar? =

Actualmente, microdata es el recomendado por Google, pero con microformats Google detecta las estrellas y las usa en tus búsquedas ([ejemplo](https://www.google.com/search?q=site:emiliocobos.net+ec+stars+rating)).

== Screenshots ==

1. Funcionamiento básico del plugin

== Changelog ==

= 1.0.4 =
Añadido el shortcode y el widget (beta)

= 1.0.3 =
Pequeño fix del sistema de votos, y internacionalización mejorada otra vez

= 1.0.2.1 =
Incluye archivos de lenguaje

= 1.0.2 =
Internacionalización

= 1.0.1 =
Pequeña mejora en el rendimiento, accesibilidad y más documentación

= 1.0 =
Primera versión estable, con algunos errores de formato de los números arreglados.

== Upgrade notice ==
= 1.0.3 =
ACTUALIZA URGENTEMENTE PARA GARANTIZAR LA INTEGRIDAD DE TUS VOTOS

= 1.0.2 =
Internacionalización

= 1.0.1 =
Actualiza para una pequeña mejora en el rendimiento

= 1.0 =
Si usas una versión antigua, actualiza lo más pronto posible

== Cómo funciona ==

Básicamente creamos una nueva tabla llamada `(prefijo)ec_stars_votes`, donde guardamos los votos de la gente (para prevenir votos duplicados).

El número de votos y la suma de todos los votos son guardados en la tabla `(prefijo)options` en forma de campos meta personalizados: Uno para el número de votos, otro para la suma de todos los valores de los votos. Ambos se actualizan cuando alguien vota.