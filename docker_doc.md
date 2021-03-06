# DOCKER

_>Apuntes de comandos basicos de docker_

## Pruebas posterior a la instalaci贸n ubuntu 20.04 馃殌


### Primeros comandos 馃搵

_>listar contenedores_

```
docker ps -a
```
_>detalles de un contenedor (no se considera las " ")_

```
docker inspect "container_name"
```

_>crear contenedor con nombre_

```
docker run --name "hello_geek" hello-world
```

_>cambiar nombre de contenedor_

```
docker rename "hello_geek" "hello_new_name"
```
_>borrar contenedor_

```
docker rm "hello_geek"
```
_>borrar todos los contenedores_

```
docker container prune
```

### Levantar contenedores
_>Levantar contenedor con ubuntu, al no colar ningun parametro previo el contenedor levanta y se apaga sin realizar ninguna acci贸n_

```
docker run ubuntu
```
_>Levantando contenedor de ubuntu en modo interactivo: Esto nos permite acceder a modo terminal bash en el contenedor_

```
docker run -it ubuntu
```
### Ciclo de vida de un contedor

_>Levantar contenedor enviando un comando de ejecuci贸n_

```
docker run --name alwaysup -d tail -f /etc/null
```
_El contenedor permanece activo y podemos intereactuar con el mediante:_

```
docker exec -it alwaysup bash
```
_>Matar proceso de contenedor. Extraemos el proceso en la PC ejecutando:_

```
docker inspect --format {{.State.Pid}} alwaysup 

```
_Esto nos devolver谩 el PID del proceso para eliminarlo_

### Instalaci贸n 馃敡

_Una serie de ejemplos paso a paso que te dice lo que debes ejecutar para tener un entorno de desarrollo ejecutandose_

_D铆 c贸mo ser谩 ese paso_

```
Da un ejemplo
```

_Y repite_

```
hasta finalizar
```

_Finaliza con un ejemplo de c贸mo obtener datos del sistema o como usarlos para una peque帽a demo_

## Ejecutando las pruebas 鈿欙笍

_Explica como ejecutar las pruebas automatizadas para este sistema_

### Analice las pruebas end-to-end 馃敥

_Explica que verifican estas pruebas y por qu茅_

```
Da un ejemplo
```

### Y las pruebas de estilo de codificaci贸n 鈱笍

_Explica que verifican estas pruebas y por qu茅_

```
Da un ejemplo
```

## Despliegue 馃摝

_Agrega notas adicionales sobre como hacer deploy_

## Construido con 馃洜锔?

_Menciona las herramientas que utilizaste para crear tu proyecto_

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - El framework web usado
* [Maven](https://maven.apache.org/) - Manejador de dependencias
* [ROME](https://rometools.github.io/rome/) - Usado para generar RSS

## Contribuyendo 馃枃锔?

Por favor lee el [CONTRIBUTING.md](https://gist.github.com/villanuevand/xxxxxx) para detalles de nuestro c贸digo de conducta, y el proceso para enviarnos pull requests.

## Wiki 馃摉

Puedes encontrar mucho m谩s de c贸mo utilizar este proyecto en nuestra [Wiki](https://github.com/tu/proyecto/wiki)

## Versionado 馃搶

Usamos [SemVer](http://semver.org/) para el versionado. Para todas las versiones disponibles, mira los [tags en este repositorio](https://github.com/tu/proyecto/tags).

## Autores 鉁掞笍

_Menciona a todos aquellos que ayudaron a levantar el proyecto desde sus inicios_

* **Andr茅s Villanueva** - *Trabajo Inicial* - [villanuevand](https://github.com/villanuevand)
* **Fulanito Detal** - *Documentaci贸n* - [fulanitodetal](#fulanito-de-tal)

Tambi茅n puedes mirar la lista de todos los [contribuyentes](https://github.com/your/project/contributors) qu铆enes han participado en este proyecto.

## Licencia 馃搫

Este proyecto est谩 bajo la Licencia (Tu Licencia) - mira el archivo [LICENSE.md](LICENSE.md) para detalles

## Expresiones de Gratitud 馃巵

* Comenta a otros sobre este proyecto 馃摙
* Invita una cerveza 馃嵑 o un caf茅 鈽? a alguien del equipo.
* Da las gracias p煤blicamente 馃.
* etc.



---
鈱笍 con 鉂わ笍 por [Villanuevand](https://github.com/Villanuevand) 馃槉
