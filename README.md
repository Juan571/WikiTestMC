# WiketsMC

Modulo Manejador de Clientes - PHP - MYSQL 
> Para WIkets

## Instalación



### Para Windows : 

Es Necesario instalar

```
PHP 5.4+
Mysql(stable)
```

>Se recomienta Instalar   [XAMPP](https://www.apachefriends.org/es/index.html).


##### Una vez instalado XAMPP 

Crear una Base de datos llamada `wiketsMC`, y exportar la estructura a partir del archivo: `wiketsMC.sql`

>Se recomienda usar Phpmyadmin.. (ya deberia estar previamente instalado)

Luego procedemos a configurar los parametros de conexion del proyecto en 

>Wikest_Test1/Funciones/parametros_bd/parametros_bd.php


```
<?php

    #MOTOR DE BASE DE DATOS 'DRIVER' DEBE IR EN MINÚSCULA
    define('MOTOR_BD', 'mysql');

    # IP SERVIDOR USADO PARA ACCEDER A LA BD
    define("SERVIDOR_BD","localhost");

    # PUERTO DEL SERVIDOR USADO PARA ACCEDER A LA BD
    define('PUERTO_BD', '3306');

    # NOMBRE DE USUARIO PARA ACCEDER A LA BD
    define('USUARIO_BD', 'USUARIO');

    # PASSWORD DEL USUARIO
    define('CLAVE_BD', 'CLAVE');

    # EL NOMBRE DE LA BASE DE DATOS
    define("NOMBRE_BD","wiketsMC");

    #CHARSET
    define("CHARSET","UTF8");
?>


```
Modificando los parametros necesarios con datos del servidor y según la instalacion previa del XAMPP
Los a modificar serian : 

```php
USUARIO_BD -> root (usuario por defecto para mysql con todos los privilegios)
CLAVE_BD -> por defecto seria ''.
```

Luego copiar la carpeta Wikets_Test1 en : 
>C:\XAMPP/Htdocs/

Una vez copiada la carpeta abrir un navegador web y acceder a http://localhost/Wikets_Test1/




