# comandos-basicos-docker
Listado de comandos más usados en Docker.
En Mayúsuca valores a ingresar u opciones de Docker.


Mostrar información de Docker:
```
docker info
```

Descargar imagen (hub.docker.com):
```
docker pull NOMBRE_IMAGEN
```

Mostrar imágenes descargadas:
```
docker images
```

Mostrar contenedores activos:
```
docker ps
```

Mostrar contenedores inactivos:
```
docker ps -a
```

Mostrar contenedor con filtro: exited, etc:
```
docker ps --filter="FILTRO=VALOR"
```

Correr contenedor (Crea nueva instancia):
```
docker run NOMBRE_IMAGEN echo COMENTARIO
```

Correr contenedor interactivo (ejemplo bash):
```
docker run -it NOMBRE_IMAGEN COMANDO
```

Correr contenedor con nombre:
```
docker run --name NOMBRE NOMBRE_IMAGEN COMANDO
```

Entrar a contenedor activo:
```
docker attach CONTENEDOR_ID
```

Levantar contenedor apagado:
```
docker start NOMBRE_CONTENEDOR
```

Salir cde contenedor sin matarlo:
```
ctrl + p + q
```

Borrar contenedor:
```
docker rm NOMBRE_CONTENEDOR
```

Ping 10 veces a Google:
```
docker run NOMBRE_CONTENEDOR  ping -c 10 google.com
```

Ejecutar contenedor como daemon:
```
docker run -ps NOMBRE_CONTENEDOR
```

Ejecutar contenedor y exponer puerto:
```
docker run -P 80:80 NOMBRE_CONTENEDOR
```

Mostrar Log de contenedor activo:
```
docker logs ID_CONTENEDOR
```

Mostrar log de contenedor activo en tiempo real:
```
docker logs -f ID_CONTENEDOR
```

Ingresar a contenedor activo:
```
docker exec -ti ID_CONTENEDOR COMANDO
```

Mostrar IP de la máquina Docker:
```
docker-machine ls
```

Parar un contenedor:
```
docker stop ID_CONTENEDOR
docker kill ID_CONTENEDOR
```

Pausar un contenedor:
```
docker pause ID_CONTENEDOR
```

Despausar un contenedor:
```
docker unpause ID_CONTENEDOR
```

Inspeccionar un contenedor:
```
docker inspect ID_CONTENEDOR
```
