# Tarea Evaluable Docker

**CIFP La Laboral - Módulo Despliegue de Aplicaciones Web**

> 👥 **Autores:** Iker y Pelayo Rodríguez                                                                                                                                   📌 **Fecha de entrega y exposición:** Viernes, 21 de febrero de 2025.                                                                                                                                     📂 **Repositorio GitHub:** ‣
> 

# 📑 ÍNDICE

| 📝 | 1. Descripción del Proyecto |
| --- | --- |
| ⚙️ | 2. Instrucciones Generales |
| 👥 | 3. Asignación de tareas |
| 📁 | 4. Estructura del Repositorio |
| 📚 | 5. Ejercicios |
|  | 5.1 Manual de Docker Desktop |
|  | 5.2 Servidor de Base de Datos |
|  | 5.3 Contenedores en Red |
|  | 5.4 Docker Compose |
|  | 5.5 Imagen con Dockerfile - Aplicación Web |

## 📝 Descripción del Proyecto

Este repositorio contiene la resolución de la **Tarea Evaluable Docker**, organizada en cinco ejercicios prácticos relacionados con la gestión de contenedores Docker, redes y despliegue de aplicaciones web.

## ⚙️ Instrucciones Generales

- **👥 Trabajo en equipo:** Grupo compuesto por 2 personas(Pelayo e Iker).
- **📂 Repositorio en GitHub:** Tenemos una persona que creó el repositorio(Pelayo) y otra colaboradora(Iker).
- **🌱 Uso de ramas:** Trabajamos con branches para una correcta organización del código.
- **📌 Registro de contribuciones:** Los commits reflejan las aportaciones de cada miembro del equipo.
- **✅ Asignación de tareas:** Documentación de la distribución de tareas, plazos y porcentaje de cumplimiento en un documento del repositorio.
- **🗃️ Estructura del repositorio:** Contamos con una carpeta para cada ejercicio con la documentación y los archivos necesarios.
- **📑 Entrega final:**  Documento en PDF con nuestros nombres y la URL del repositorio.

## 👥 ASIGNACIÓN DE TAREAS

[ToDo](ToDo%2019851fe9844080a6abddc98573e9407c.csv)

## 📁 ESTRUCTURA DEL REPOSITORIO

```
📂 proyecto-docker/
├── 📁 Ejercicio_1/
│   ├── 📄 manual_docker.md
│   ├── 📸 imagenes/
│   └── 📑 manual_docker.pdf
│
├── 📁 Ejercicio_2/
│   ├── 📄 servidor_base_datos.md
│   ├── 📸 imagenes/
│   └── 📑 servidor_base_datos.pdf
│
├── 📁 Ejercicio_3/
│   ├── 📄 comandos_red.md
│   ├── 📸 imagenes/
│   └── 📑 comandos_red.pdf
│
├── 📁 Ejercicio_4/
│   ├── ⚙️ docker_compose.yaml
│   ├── 📸 imagenes/
│   ├── 📄 docker_compose.md
│   └── 📑 docker_compose.pdf
│
├── 📁 Ejercicio_5/
│   ├── 🐳 Dockerfile
│   ├── 🌐 index.html
│   ├── 🎨 styles.css
│   ├── 🔧 script.php
│   ├── 📸 imagenes/
│   ├── 📝 docker_commands.txt
│   ├── 📄 dockerfile.md
│   └── 📑 dockerfile.pdf
│
└── 📄 README.md
```

## 📖 Ejercicios

### 🖥️ Ejercicio 1: Manual de Docker Desktop

### 💾 Proceso paso a paso de instalación

- **Abrimos el navegador** y accedemos a la página oficial de Docker:

  👉[🔗 Página oficial de Docker Desktop](https://www.docker.com/products/docker-desktop)

- Bajamos un poco pinchamos en Download Docker Desktop y lo descargamos para Windows.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%201.png)

Una vez descargado, pinchamos en el instalador y comenzamos con la descarga:

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%202.png)

![Captura de pantalla 2025-02-14 105846.png](./TareaEvaluableDocker_PelayoIker.assets/Captura_de_pantalla_2025-02-14_105846.png)

Una vez realizada la instalación, accedemos a Docker Desktop:

Nada mas entrar nos pedirá iniciar sesión o registrarnos:

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%203.png)

Una vez hecho, ya accedemos a Docker Desktop y a todas sus funcionalidades: 

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%204.png)

### 🖥️ Navegación por la interfaz principal

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image 5.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%206.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%207.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%208.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%209.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2010.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2011.png)

### 📦 Operaciones básicas con contenedores

***Ver Contenedores Disponibles***

- Abrimos **Docker Desktop**.
- En la barra lateral izquierda, seleccionamos **Containers**.
- Se muestra una lista con los contenedores creados, indicando su estado (corriendo, detenido, etc.).

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2012.png)

***Iniciar un Contenedor Detenido***

- Ubicamos el contenedor en la lista.
- Si el estado es "Exited", hacemos clic en los tres puntos **(⋮)** a la derecha del contenedor.
- Seleccionamos Restart para reiniciarlo.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2013.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2014.png)

***Detener un Contenedor en Ejecución***

- Usamos el contenedor en ejecución.
- Le damos a los tres puntos **(⋮)**.
- Selecciona **Pause** o **Stop** según sea necesario.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2015.png)

***Eliminar un Contenedor***

- Nos aseguramos de que el contenedor está detenido.
- Hacemos clic en los tres puntos **(⋮)** a la derecha del contenedor.
- Seleccionamos el icono de **Eliminar** para eliminarlo.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2016.png)

***Ver Detalles de un Contenedor***

- Hacemos clic en los tres puntos **(⋮)** a la derecha del contenedor.
- Seleccionamos view details.
- Al entrar, podemos ver información como logs, configuración y estadísticas de uso.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2017.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2018.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2019.png)

***Copiar el Comando de Ejecución de un Contenedor***

- Hacemos clic en los tres puntos **(⋮)** junto al contenedor.
- Seleccionamos **Copy docker run** para copiar el comando con el que fue creado.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2020.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2021.png)

***Ver Archivos de un Contenedor***

- Hacemos clic en los tres puntos **(⋮)**.
- Seleccionamos **View files** para explorar los archivos dentro del contenedor.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2022.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2023.png)

## 🏷️ Gestión de imágenes Docker

***Ver las Imágenes Disponibles***

- En la barra lateral izquierda, seleccionamos **Images**.
- Se nos muestra la lista de imágenes descargadas en el sistema.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2024.png)

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

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2025.png)

***Eliminar una Imagen***

1. Encontramos la imagen que queremos borrar en la pestaña **Images**.
2. Hacemos clic en el icono de los tres puntos **(⋮)** a la derecha.
3. Seleccionamos **Delete** para eliminar la imagen.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2026.png)

No se pueden eliminar imágenes que están en uso por un contenedor en ejecución:

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2027.png)

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

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2028.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2029.png)

### 🔌 Configuración de redes y volúmenes

***Ver las redes disponibles***

- En la barra lateral, seleccionamos **Containers**.
- Hacemos clic en un contenedor existente y seleccionamos **View details**.
- En la pestaña **Network**, vemos las redes asociadas al contenedor.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2030.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2031.png)

***Crear una Nueva Red***

Docker Desktop no ofrece una opción nativa para añadir redes directamente desde su interfaz, pero podemos utilizar extensiones de terceros para ampliar su funcionalidad.

- Hacemos clic en la pestaña **Extensions** en la barra lateral izquierda.
- En el Marketplace de Extensiones, buscamos **Portainer**.
- Hacemos clic en **Install** para añadir la extensión.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image 32.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2033.png)

- Configuramos el entorno

Al iniciar Portainer por primera vez, verás la pantalla de "Quick Setup" (como en tu imagen). Aquí puedes:

- **"Get Started"**: Gestionamos el entorno local de Docker donde se ejecuta Portainer.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2034.png)

- **"Add Environments"**: Agregamos otros entornos remotos, como clústeres de Kubernetes o instancias Docker en servidores.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2035.png)

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

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2036.png)

- Una vez instalada, vamos a **"Extensions" > "Disk Usage"**.
- Revisamos el uso de espacio y liberamos lo que no necesitemos.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2037.png)

### **Logs Explorer (Explorador de Logs)**

- Permite ver los logs de todos los contenedores sin usar la terminal.
- Muy útil para detectar errores sin ejecutar `docker logs`.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2038.png)

- Vamos a **"Extensions" > "Logs Explorer"**.
- Seleccionamos el contenedor que queremos analizar y revisamos los logs en la interfaz.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2039.png)

### 🛢️ Ejercicio 2: Servidor de Base de Datos

***Descargar la imagen de MariaDB***

- Buscamos la imagen de **mariadb** y la descargamos
- En el menú de Docker Desktop, seleccionamos la pestaña **"Images"** (Imágenes).
- En la barra de búsqueda, escribimos **"mariadb🦭"**.
- Aparecen varias opciones relacionadas con MariaDB, selccionamos la primera.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2040.png)

- Identificamos la imagen correcta con el nombre **"mariadb🦭"** y el ícono oficial.
- Verificamos que tiene **más de 1B+ descargas** y **5.9K estrellas** (esto confirma que es la imagen más utilizada y confiable).
- Hacemos clic en la imagen para seleccionarla.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2041.png)

***Verificación que la imagen se descargó correctamente***

- Vamos nuevamente a la pestaña "Images".
- Ahora, la imagen de MariaDB nos aparece en la lista de imágenes disponibles en tu sistema.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2042.png)

***Crear un contenedor con MariaDB***

- Vamos a la pestaña **Images** y haz clic en **Run** con la imagen de **MariaDB** que descargamos.
- Configuramos los siguientes parámetros en Optional Settings:
    - **Nombre del contenedor**: `bbdd`
    - **Puerto**: **3306** (nos aseguramos de exponerlo para conexiones externas)
    - **Volumen**: Creamos un volumen llamado `datos-mariadb`.
        - En **Host path**, escribimos el nombre del volumen `datos-mariadb` .
        - En **Container path**, asignamos la ruta donde MariaDB guarda los datos dentro del contenedor  /var/lib/mysql  que es la ruta por defecto donde MariaDB almacena sus datos en el contenedor.
    - **Variables de entorno**:
        - `MYSQL_ROOT_USER=root`
        - `MYSQL_ROOT_PASSWORD=root`
        - `MYSQL_DATABASE=base`
        - `MYSQL_USER=daw`
        - `MYSQL_PASSWORD=daw`
- Guardamos y le damos a Run.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2043.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2044.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2045.png)

***Conectarse a la base de datos con DBeaver***

- Abrimos **DBeaver**
- Creamos una nueva conexión:
    - Configuración general:
        - **Host**: `localhost`
        - **Puerto**: `3306`
    - Credenciales:
        - **Usuario**: `daw`
        - **Contraseña**: `daw`
    - Base de datos:
        - **Base de datos**: `base`

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2046.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2047.png)

***Probamos la conexión y nos aseguramos de que funciona.***

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2048.png)

 ***Crear una nueva base de datos***

- Hacemos clic derecho en la conexión con **MariaDB** y seleccionamos **"Crear Nuevo Database"**.
- Se nos abre una ventana llamada **"Create database"**.
- En **Database name**, escribimos el nombre de la base de datos, en este caso la llamamos `dbPelayoIker.`
- En **Charset**, seleccionamos **utf8mb4** (para compatibilidad con caracteres especiales y emojis).
- Opcionalmente, podiamos configurar **Collation**, pero en este caso lo dejarlo vacío para la opción por defecto.
- Hacemos clic en **"Aceptar"** para crear la base de datos.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2049.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2050.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2051.png)

***Seleccionamos la base de datos y crear una tabla***

- Hacemos clic derecho sobre la base de datos `dbPelayoIker` que acabamos de crear.
- Luego, hacemos clic derecho en **"Tables"** → **"Create New Table"**.
- Asignamos un nombre a la tabla , le ponemos por ejemplo,`ejemplo`.
- Agregamos las columnas necesarias:
    - `id` → **INT**, los marcamos como **Primary Key**, opción **Auto Increment**.
    - `nombre` → **VARCHAR(50)**, lo marcamos como **NOT NULL**.
- Guardamos los cambios y presionamos en **"Aceptar"**.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2052.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2053.png)

***Verificamos que la tabla se creo correctamente***

- Expandimos la base de datos `dbPelayoIker` en el panel izquierdo y hacemos clic en **"Tables"**.
- Vemos la tabla `ejemplo`, con lo cual se ha creado correctamente.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2054.png)

***Detener y eliminar los contenedores***

- Abrimos **Docker Desktop**.
- En la pestaña **Containers**, buscamos el contenedores `bbdd`.
- Detenemos cada contenedor presionando el botón **Stop (🟥)**.
- Luego, eliminamos los contenedores con el botón **Delete (🗑️)**.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2055.png)

***Verificamos que el volumen "datos-mariadb" sigue existiendo***

- En Docker Desktop, vamos a la pestaña **Volumes**.
- Buscamos el volumen `datos-mariadb`.
- Como se ve el volumen sigue ahi, lo que significa que los datos no se han perdido.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2056.png)

***Creamos otro contenedor con el mismo volumen***

- En Docker Desktop, vamos a **Images** y buscamos **MariaDB**.
- Hacemos clic en **Run** para desplegar un nuevo contenedor.
- Configuramos:
    - **Container name**: `bbdd-2`
    - **Port**: `3306`
    - **Volume**: `datos-mariadb`
    - **Environment variables** (como antes):
        - `MYSQL_ROOT_USER=root`
        - `MYSQL_ROOT_PASSWORD=root`
        - `MARIADB_DATABASE=base`
        - `MARIADB_USER=daw`
        - `MARIADB_PASSWORD=daw`
- Hacemos clic en **Run**.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2057.png)

***Comprobamos que los datos siguen en el nuevo contenedor***

- Abrimos **DBeaver** y nos **conectatamos de nuevo a MariaDB** (`localhost:3306`, usuario `daw`).
- Verificamos que `dbPelayoIker` y la tabla `ejemplo` siguen existiendo.
- Como todo está correcto, los datos se han conservado gracias al volumen persistente.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2058.png)

***Intentar borrar la imagen de MariaDB***

- En Docker Desktop, vamos a la pestaña **Images**.
- Intentamos eliminar la imagen de **MariaDB** (`Delete`).
- **¿Qué sucede?**
    - No podremos eliminar si hay contenedores en ejecución usándola (`bbdd-2`).
    - Tenemos que eliminar `bbdd-2` antes de poder borrar la imagen.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2059.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2060.png)

***Borrar todo (Volumen, Imagen y Contenedor)***

- Eliminamos los contenedor **`bbdd`** y **`bbdd-2`** desde Docker Desktop.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2061.png)

- Eliminamos el volumen **`datos-mariadb`** desde la pestaña **Volumes**.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2062.png)

- Eliminamos la imagen de MariaDB desde la pestaña **Images**.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2063.png)

### 🌐 Ejercicio 3: Contenedores en Red

### 🛠️ Crear una red bridge (redbd)

En **Docker Desktop**, no hay una sección visual para redes en la interfaz, pero podemos verlas y administrarlas con comandos Docker.

Primero listamos las redes, luego, creamos la red bridge pedida y por ultimo vemos los detalles de esa red y comprobamos que se ha creado correctamente:

```bash
 $docker network ls
 $docker network create redbd
 $docker network inspect redbd
```

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2064.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2065.png)

### 🐬 Crear el contenedor de MariaDB con comandos

Ejecutamos en la terminal:

```bash
$docker run -d --name mariadb-container \
  --network redbd \
  -e MYSQL_ROOT_PASSWORD=root \
  -e MYSQL_DATABASE=base \
  -e MYSQL_USER=daw \
  -e MYSQL_PASSWORD=daw \
  -p 3306:3306 \
  -v mariadb_data:/var/lib/mysql \
  mariadb:latest
```

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2066.png)

### 🐬 Crear el contenedor de MariaDB con Docker Desktop

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2067.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2068.png)

Podemos ver en los logs que el contenedor de MariaDB se ha iniciado correctamente. El sistema nos muestra una secuencia de mensajes de inicialización que confirman que la base de datos está lista para aceptar conexiones y que todos los componentes necesarios se han cargado correctamente.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2069.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2070.png)

### 🌐 Crear el contenedor con Adminer o phpMyAdmin con comandos

```bash
$docker run -d --name adminer-container \
  --network redbd \
  -p 8080:8080 \
  adminer
```

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2071.png)

### 🌐 Crear el contenedor con Adminer o phpMyAdmin con Docker Desktop

- Vamos a la pestaña **"Images"** y hacemos clic en **"Run"** con la imagen de Adminer.
- En **"Advanced settings"**:
    - Nombre: `adminer-container`.
    - Host Port: `8080`.
- Hacemos clic en **"Run"**.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2072.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image 73.png)

### 💻 Acceder a la base de datos desde la interfaz gráfica

Abrimos el navegador y vamos a `http://localhost:8080`.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2074.png)

- Rellenamos los datos de conexión:
    - **Servidor**: `mariadb-container` (nombre del contenedor).
    - **Usuario**: `daw`.
    - **Contraseña**: `daw`.
    - **Base de datos**: `base`.
- Hacemos clic en **"Login"**.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2075.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2076.png)

***Crear una Tabla en la Base de Datos***

- Entramos en la base de datos `base` y elegimos **"Crear tabla"**.
- Definimos una tabla de ejemplo:
  
  
    | Campo | Tipo | Clave primaria |
    | --- | --- | --- |
    | id | INT | ✅ (Auto-incremental) |
    | nombre | VARCHAR(50) | ❌ |
- Guardamos los cambios.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2077.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2078.png)

### 🧹 Borrar los contenedores, la red y los volúmenes utilizados con comandos

```bash
$docker stop mariadb-container adminer
$docker rm mariadb-container adminer
$docker network rm my_network
$docker volume prune -f
```

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2079.png)

### 🧹 Borrar los contenedores, la red y los volúmenes utilizados con Docker Desktop

Primero paramos los contenedores, haciendo click en Stop.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2080.png)

Y luego los borramos:

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2081.png)

Una vez borrados podemos borrar sus imagenes:

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2082.png)

### 🏗️ Ejercicio 4: Docker Compose

***Crear el archivo `docker-compose.yaml` con comandos***

Abrimos una terminal y creamos una nueva carpeta para el proyecto, dentro de esta carpeta, creamos el archivo `docker-compose.yaml`. Para esto, usamos bloc de notas(o cualquier otro editor de texto):

```bash
$mkdir htop-docker && cd htop-docker
$notepad docker-compose.yaml
```

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2083.png)

Pegamos el siguiente contenido en el archivo y luego lo guardamos y cerramos el bloc de notas:

```yaml
services:
  htop:
    image: terencewestphal/htop
    container_name: htop_container
    stdin_open: true
    tty: true
    command: htop
```

***Crear el archivo `docker-compose.yaml` sin comandos***

- Abrimos el **Explorador de archivos**.
- Creamos una carpeta llamada **htop-docker** en la misma ubicacion que lo estabamos haciendo con los comandos.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2084.png)

Abrimos **Visual Studio Code**, **Bloc de notas**, o cualquier editor de texto y escribimos:

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2085.png)

***Iniciar el contenedor con Docker Compose***
Ejecutamos el siguiente comando para iniciar **htop** en un contenedor y verificamos que el contenedor está corriendo:

```bash
$docker-compose up -d
$docker ps
```

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2086.png)

```bash
$docker exec -it htop_container htop
```

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2087.png)

***Detener y eliminar el contenedor***

Primero, paramos la imagen y la borramos:

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2088.png)

Y luego una vez paradas/borradas podemos borrar el conte

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2089.png)

### 🏗️ Ejercicio 5: Imagen con Dockerfile - Aplicación Web

***Creación inicial del contenedor***

Descargamos la imagen base y creamos una carpeta para los archivos del sitio web con comandos:

```bash
$docker pull php:7.4-apache
$mkdir -p web_desplieguePelayoIker
$cd web_desplieguePelayoIker
```

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2090.png)

Descargamos la imagen base y creamos una carpeta para los archivos del sitio web sin comandos:

- En Docker Hub buscamos `php:7.4-apache` y descargamos la primera.
- Una vez descargada, en la pestaña **"Images"** (Imágenes), buscamos `php:7.4-apache`.
- Por último, creamos la carpeta manualmente y la llamamos `web_desplieguePelayoIker` .

![Captura de pantalla 2025-02-13 182336.png](./TareaEvaluableDocker_PelayoIker.assets/Captura_de_pantalla_2025-02-13_182336.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2091.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2092.png)

Una vez creada la carpeta, creamos los archivos del sitio.

Abrimos VS Code y creamos los archivos index.html  ,  styles.css  y  info.php.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2093.png)

📄 **Archivo `index.html`**

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sitio Web Pelayo e Iker</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Bienvenidos al Sitio Web de Pelayo e Iker</h1>
    <p>Esta es nuestra página principal.</p>
    <p>Consulta la información del servidor <a href="info.php">aquí</a></p>
</body>
</html>

```

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2094.png)

🎨 **Archivo `styles.css`**

```css
body {
    font-family: 'Arial', sans-serif;
    margin: 0;
    padding: 0;
    background: linear-gradient(to right, #2c3e50, #4ca1af);
    color: #fff;
    text-align: center;
}

.container {
    width: 80%;
    margin: 50px auto;
    background: rgba(255, 255, 255, 0.1);
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.2);
}

h1 {
    font-size: 2.5em;
    margin-bottom: 10px;
    color: #f1c40f;
}

p {
    font-size: 1.2em;
    line-height: 1.6;
}

@media (max-width: 768px) {
    .container {
        width: 90%;
    }

    h1 {
        font-size: 2em;
    }

    p {
        font-size: 1em;
    }
}
```

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2095.png)

🖥 **Archivo `info.php`**

```php
<?php
setlocale(LC_TIME, "es_ES.UTF-8");
$mes_actual = strftime("%B");
$fecha_actual = date("d/m/Y");
$hora_actual = date("H:i:s");

echo "<h1>Información</h1>";
echo "<p>Hoy es $fecha_actual</p>";
echo "<p>El mes es: <strong>$mes_actual</strong></p>";
echo "<p>Hora: $hora_actual</p>";
?>
```

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2096.png)

Ahora arrancamos el contenedor al que llamamos web y que sea accesible desde un navegador en el puerto 8000.

Con comados :

- `d`: Corre el contenedor en modo "detached" (en segundo plano).
- `-name web`: Nombre del contenedor.
- `p 8000:80`: Mapea el puerto 8000 del host al puerto 80 del contenedor.
- `v "$(pwd)":/var/www/html`: Monta la carpeta actual en `/var/www/html` dentro del contenedor.

```bash
$docker run -d --name web -p 8000:80 -v C:\Users\usuario\Documents\web_desplieguePelayoIker:/var/www/html php:7.4-apache 
```

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2097.png)

Desde docker desktop:

- Vamos a **“Images”** y clicamos Run en la imagen de `php:7.4-apache.`
- En optional settings, lo rellenamos con los siguientes datos:
    - Contianer Name: web.
    - Ports: Host Port: `8000`.
    - En Volumes: **Host Path"**, seleccionamos la carpeta donde guardamos nuestro sitio web(web_desplieguePelayoIker) y en Container Path(/var/www/html).
- Por último pinchamos en Run, para arrancar el contenedor.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2098.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%2099.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%20100.png)

Vemos la salida del script y de la página index en el navegador:

- Abrimos el navegador y entramos a [http://localhost:8000](http://localhost:8000/).
- Para ver el info PHP, pinchamos en aquí o metemos este enlace [http://localhost:8000/info.php](http://localhost:8000/info.php).

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%20101.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%20102.png)

***Detenemos y eliminamos el contenedor con comandos***

```bash
$docker stop web
$docker rm web
```

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%20103.png)

***Detenemos y eliminamos el contenedor desde Docker Desktop***

![Captura de pantalla 2025-02-13 194602.png](./TareaEvaluableDocker_PelayoIker.assets/Captura_de_pantalla_2025-02-13_194602.png)

***Automatización de estas operaciones creando un fichero Dockerfile***
Creamos un `Dockerfile` en desde VS Code para construir la imagen automáticamente.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%20104.png)

***Construcción de la imagen***

- Ejecutamos el siguiente comando en la carpeta donde está el `Dockerfile.`
- Verificamos la nueva imagen.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%20105.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%20106.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%20107.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%20108.png)

***Subimos la imagen a Docker Hub***

- Nos dirigimos a **“Images”** y buscamos la imagen que subimos.
- Para subirla a Docker Hub, hacemos clic en el icono de los tres puntos **(⋮)** y seleccionamos Push to Docker Hub.

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%20109.png)

![image.png](./TareaEvaluableDocker_PelayoIker.assets/image%20110.png)

***Desplegar la imagen en otro equipo***

- Buscamos la imagen llamada ikerpc123/apache2.
- Descargamos la imagen desde Docker Hub en el otro equipo, haciendo click en **“Pull”.**

![Captura de pantalla 2025-02-14 101043.png](./TareaEvaluableDocker_PelayoIker.assets/Captura_de_pantalla_2025-02-14_101043.png)

- Comprobamos que esta entre nuestras imagenes.

![Captura de pantalla 2025-02-14 101319.png](./TareaEvaluableDocker_PelayoIker.assets/5b99d486-62c3-4ebc-aca8-1c5aa40d3a72.png)