# DOCKER

---
## Comandos

### Verificar version de python en terminal 

```bash 
python -V 
```

### Verificar si docker está instalado

```bash
docker
```

###  Probar que **Docker** está bien instalado. 

Descarga y ejecuta una imagen mínima de prueba que solo imprime un mensaje de bienvenida y se cierra.
```bash
docker run hello-world
```


###  Descargar ejecutar un contenedor con una imagen de **Ubuntu**
Descarga y ejecuta un contenedor con una imagen de **Ubuntu**. Pero tiene un detalle importante, parece que no hace nada, lo que pasa por dentro:

1. Descarga la imagen de **ubuntu* desde Docker Hub (si no la tenía).
2. Crea un contenedor **ubuntu**
3. Como **no se le dio ningún comando que ejecutar**, el contenedor arranca, no tiene nada que hacer, y se cierra de inmediato.



```bash
docker run ubuntu
```

### Entrar a una terminal dentro del contenedor

Entra a una terminal dentro del contenedor, aunque no le escribiste bash al final. La razón: la imagen de Ubuntu ya trae configurado bash como su comando por defecto, así que se ejecuta solo.

```bash
docker run -it ubuntu
#          │  │
#          │  └── imagen de Ubuntu
#          └── -i (interactivo) + -t (terminal). Juntos: -it
````

Para salir de esta terminal es con el comando:

```bash
exit
```