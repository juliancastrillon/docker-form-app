# Docker Form App

Este proyecto es una aplicación simple de formulario de registro de usuario que se ejecuta en un contenedor Docker utilizando Nginx.

## Requisitos previos

Antes de comenzar, asegúrate de tener instalado lo siguiente en tu sistema:

- [Git](https://git-scm.com/)
- [Docker](https://www.docker.com/)

## Pasos para ejecutar el proyecto

Sigue estos pasos para clonar el proyecto y levantarlo con Docker:

### 1. Clonar el repositorio

Abre una terminal y ejecuta el siguiente comando para clonar el repositorio:

```bash
git clone https://github.com/tu-usuario/docker-form-app.git
```

Luego, navega al directorio del proyecto:

```bash
cd docker-form-app
```

### 2. Construir la imagen de Docker

Ejecuta el siguiente comando para construir la imagen de Docker:

```bash
docker build -t docker-form-app .
```

### 3. Ejecutar el contenedor

Inicia un contenedor basado en la imagen que acabas de construir:

```bash
docker run -d -p 8080:80 --name form-app-container docker-form-app
```

### 4. Acceder a la aplicación

Abre tu navegador web y accede a la aplicación en la siguiente URL:

```
http://localhost:8080
```

### 5. Detener y eliminar el contenedor

Para detener el contenedor, ejecuta:

```bash
docker stop form-app-container
```

Para eliminar el contenedor, ejecuta:

```bash
docker rm form-app-container
```

## Estructura del proyecto

```
docker-form-app/
├── index.html
├── dockerfile
└── README.md
```

- **index.html**: Archivo HTML de la aplicación.
- **dockerfile**: Archivo Docker para construir la imagen.
- **README.md**: Instrucciones para ejecutar el proyecto.

## Contribuciones

Si deseas contribuir a este proyecto, por favor crea un fork del repositorio, realiza tus cambios y envía un pull request.

## Licencia

Este proyecto está bajo la licencia MIT. Consulta el archivo `LICENSE` para más detalles.