# Ejercicio 1

**CIFP La Laboral - Módulo Despliegue de Aplicaciones Web**

> 👥 **Autores:** Pelayo Rodríguez e Iker Pérez                                                                                                                                   📌 **Fecha de entrega y exposición:** Viernes, 21 de febrero de 2025.                                                                                                                                     📂 **Repositorio GitHub:** ‣
> 

# 📑 ÍNDICE

### 🖥️ Ejercicio 1: Manual de Docker Desktop

### 💾 Proceso paso a paso de instalación

- **Abrimos el navegador** y accedemos a la página oficial de Docker:

  👉[🔗 Página oficial de Docker Desktop](https://www.docker.com/products/docker-desktop)

- Bajamos un poco pinchamos en Download Docker Desktop y lo descargamos para Windows.

![image.png](./imagenes/image.png)

![image.png](./imagenes/image 1.png)

Una vez descargado, pinchamos en el instalador y comenzamos con la descarga:

![image.png](./imagenes/image 2.png)

![Captura de pantalla 2025-02-14 105846.png](./imagenes/Captura_de_pantalla_2025-02-14_105846.png)

Una vez realizada la instalación, accedemos a Docker Desktop:

Nada mas entrar nos pedirá iniciar sesión o registrarnos:

![image.png](./imagenes/image 3.png)

Una vez hecho, ya accedemos a Docker Desktop y a todas sus funcionalidades: 

![image.png](./imagenes/image 4.png)

### 🖥️ Navegación por la interfaz principal

![image.png](./imagenes/image 5.png)

![image.png](./imagenes/image 6.png)

![image.png](./imagenes/image 7.png)

![image.png](./imagenes/image 8.png)

![image.png](./imagenes/image 9.png)

![image.png](./imagenes/image 10.png)

![image.png](./imagenes/image 11.png)

### 📦 Operaciones básicas con contenedores

***Ver Contenedores Disponibles***

- Abrimos **Docker Desktop**.
- En la barra lateral izquierda, seleccionamos **Containers**.
- Se muestra una lista con los contenedores creados, indicando su estado (corriendo, detenido, etc.).

![image.png](./imagenes/image 12.png)

***Iniciar un Contenedor Detenido***

- Ubicamos el contenedor en la lista.
- Si el estado es "Exited", hacemos clic en los tres puntos **(⋮)** a la derecha del contenedor.
- Seleccionamos Restart para reiniciarlo.

![image.png](./imagenes/image%2013.png)

![image.png](./imagenes/image%2014.png)

***Detener un Contenedor en Ejecución***

- Usamos el contenedor en ejecución.
- Le damos a los tres puntos **(⋮)**.
- Selecciona **Pause** o **Stop** según sea necesario.

![image.png](./imagenes/image 15.png)

***Eliminar un Contenedor***

- Nos aseguramos de que el contenedor está detenido.
- Hacemos clic en los tres puntos **(⋮)** a la derecha del contenedor.
- Seleccionamos el icono de **Eliminar** para eliminarlo.

![image.png](./imagenes/image 16.png)

***Ver Detalles de un Contenedor***

- Hacemos clic en los tres puntos **(⋮)** a la derecha del contenedor.
- Seleccionamos view details.
- Al entrar, podemos ver información como logs, configuración y estadísticas de uso.

![image.png](./imagenes/image 17.png)

![image.png](./imagenes/image 18.png)

![image.png](./imagenes/image 19.png)

***Copiar el Comando de Ejecución de un Contenedor***

- Hacemos clic en los tres puntos **(⋮)** junto al contenedor.
- Seleccionamos **Copy docker run** para copiar el comando con el que fue creado.

![image.png](./imagenes/image 20.png)

![image.png](./imagenes/image 21.png)

***Ver Archivos de un Contenedor***

- Hacemos clic en los tres puntos **(⋮)**.
- Seleccionamos **View files** para explorar los archivos dentro del contenedor.

![image.png](./imagenes/image 22.png)

![image.png](./imagenes/image 23.png)

## 🏷️ Gestión de imágenes Docker

***Ver las Imágenes Disponibles***

- En la barra lateral izquierda, seleccionamos **Images**.
- Se nos muestra la lista de imágenes descargadas en el sistema.

![image.png](./imagenes/image 24.png)

***Descargar una Imagen desde Docker Hub***

- Descargamos la imagen manualmente con:

```bash
$docker pull nginx:latest
```

- Vamos a la pestaña **Images**.
- Hacemos clic en el botón **Pull** (Descargar).
- Escribimos el nombre de la imagen y su versión, por ejemplo:

```bash
$nginx:latest
```

- Haz clic en **Pull** para descargar la imagen.

![image.png](./imagenes/image 25.png)

***Eliminar una Imagen***

1. Encontramos la imagen que queremos borrar en la pestaña **Images**.
2. Hacemos clic en el icono de los tres puntos **(⋮)** a la derecha.
3. Seleccionamos **Delete** para eliminar la imagen.

![image.png](./imagenes/image 26.png)

No se pueden eliminar imágenes que están en uso por un contenedor en ejecución:

![image.png](./imagenes/image 27.png)

***Crear una Imagen Personalizada***

- Escribimos un **Dockerfile** con la configuración de la imagen.
- Usamos el siguiente comando en la terminal:
  
    ```bash
    $docker build -t mi-imagen .
    ```
    
- Posteriormente, la imagen nos aparece en la pestaña **Images**.

***Ejecutar un Contenedor desde una Imagen***

- Encontramos la imagen que queremos ejecutar.
- Hacemos clic en **Run**.
- Configuramos los puertos y volúmenes si es necesario y hacemos clic en Run.

![image.png](./imagenes/image 28.png)

![image.png](./imagenes/image 29.png)

### 🔌 Configuración de redes y volúmenes

***Ver las redes disponibles***

- En la barra lateral, seleccionamos **Containers**.
- Hacemos clic en un contenedor existente y seleccionamos **View details**.
- En la pestaña **Network**, vemos las redes asociadas al contenedor.

![image.png](./imagenes/image 30.png)

![image.png](./imagenes/image 31.png)

***Crear una Nueva Red***

Docker Desktop no ofrece una opción nativa para añadir redes directamente desde su interfaz, pero podemos utilizar extensiones de terceros para ampliar su funcionalidad.

- Hacemos clic en la pestaña **Extensions** en la barra lateral izquierda.
- En el Marketplace de Extensiones, buscamos **Portainer**.
- Hacemos clic en **Install** para añadir la extensión.

![image.png](./imagenes/image 32.png)

![image.png](./imagenes/image 33.png)

- Configuramos el entorno

Al iniciar Portainer por primera vez, verás la pantalla de "Quick Setup" (como en tu imagen). Aquí puedes:

- **"Get Started"**: Gestionamos el entorno local de Docker donde se ejecuta Portainer.

![image.png](./imagenes/image 34.png)

- **"Add Environments"**: Agregamos otros entornos remotos, como clústeres de Kubernetes o instancias Docker en servidores.

![image.png](./imagenes/image 35.png)

- Administramos contenedores

Desde el panel de control de Portainer, puedes:

- Crear, iniciar, detener y eliminar contenedores.
- Ver logs y estadísticas de rendimiento.
- Gestionar imágenes y volúmenes de Docker.
- Configurar redes y stacks con Docker Compose.

### 🔧 Herramientas de diagnóstico

### **Disk Usage (Uso de Disco)**

- Muestra cuánto espacio ocupan las imágenes, contenedores y volúmenes.
- Ideal si Docker usa demasiado espacio en disco.

![image.png](./imagenes/image 36.png)

- Una vez instalada, vamos a **"Extensions" > "Disk Usage"**.
- Revisamos el uso de espacio y liberamos lo que no necesitemos.

![image.png](./imagenes/image 37.png)

### **Logs Explorer (Explorador de Logs)**

- Permite ver los logs de todos los contenedores sin usar la terminal.
- Muy útil para detectar errores sin ejecutar `docker logs`.

![image.png](./imagenes/image 38.png)

- Vamos a **"Extensions" > "Logs Explorer"**.
- Seleccionamos el contenedor que queremos analizar y revisamos los logs en la interfaz.

![image.png](./imagenes/image%2039.png)