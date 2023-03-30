## Conectarse al contenedor. el comando exec(ejecutar), el nombre de servicio, y le ejecutamos una terminall tipo bash. De esa manera nos conectamos a un servicio que estemos corriendo en docker. esto me ingresaria en la terminal al contenedor (estan basados en unix)

``` sh
docker-compose exec mongodb bash
```

## Contectarse con mongosh.Si ya entramos y ese contenedor tiene mongo corriendo con mongo sh, debemos coencetarnos. Debemos colocar la URL conexion de mongo (en Atlas)

```sh
mongosh "mongodb://luism:luis123@localhost:27017/?authMechanism=DEFAULT&tls=false" ## local mongo compass
mongo "mongodb+srv://luisadmin:Orestico21.@mongodb101.gc47tbc.mongodb.net/test" ## en la nube mongo atlas
 
```

## Comando para ver las bases de datos de esa base de datos

```sh
show dbs ## para ver databases
show collections ## para ver colecciones
```

## conectarse a una base de datos especifica.

```sh
use("nombre_bd") ##para ingresar a la bd
db.nombre_coleccion.find() ##me mostraria los elementos o documentos existentes en una coleccion
```
 
