# Instrucciones #
1. Instalar el plugin
2. Configurarlo desde Configuración > EC Stars Rating
3. Añadir en tu tema allá donde quieras que se vea (normalmente `single.php`) el siguente pedacito de código:

```php
<?php if(function_exists('ec_stars_rating')) {
		ec_stars_rating();
} ?>
```