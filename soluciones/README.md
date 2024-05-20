# Ejercicio semanal

## Apartado 1

Para la realización del ejercicio se han hecho dos deployments, uno para la base de datos MySQL y otro para la aplicación de laravel. Para ello se han utilizado las imágenes oficiales en sus últimas versiones. Éstas han sido: 
- ``mysql`` (https://hub.docker.com/_/mysql)
- ``bitnami:laravel`` (https://hub.docker.com/r/bitnami/laravel)

Se ha hecho un seguimiento de la documentación para configurar las variables de entorno.

### Creación del deployment y servicio de MySQL

Se crea un deployment para la base de datos. Se ha hecho uso de ConfigMap para las variables de entorno y se han utilizado secretos para el usuario y contraseña.

Una vez el pod se encuentra en estado ``running`` se crea un servicio de tipo ClusterIP.

Se comprueba a través de los logs que la base de datos funciona de manera correcta.

![]()


### Creación del deployment y servicio de Laravel

Se crean tanto el depoyment como el servicio de Laravel, en este caso de tipo NodePort.

Se comprueba a través de los logs del contenedor que funciona correctamente.

![]()


