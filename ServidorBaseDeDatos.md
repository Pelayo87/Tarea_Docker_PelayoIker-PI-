# Ejercicio 2

**CIFP La Laboral - Módulo Despliegue de Aplicaciones Web**

> 👥 **Autores:** Pelayo Rodríguez e Iker Pérez                                                                                                                                 📌 **Fecha de entrega y exposición:** Viernes, 21 de febrero de 2025.                                                                                                                                     📂 **Repositorio GitHub:** ‣
> 

# 📑 ÍNDICE

1. Ejercicio 2: Servidor de Base de Datos
    - Descargar la imagen de MariaDB
    - Verificación de la descarga
    - Crear un contenedor con MariaDB
    - Conectarse a la base de datos con DBeaver
    - Crear una nueva base de datos
    - Crear una tabla
    - Detener y eliminar contenedores
    - Verificación del volumen
    - Crear nuevo contenedor con volumen existente
    - Borrado final de recursos

### 🛢️ Ejercicio 2: Servidor de Base de Datos

***Descargar la imagen de MariaDB***

- Buscamos la imagen de **mariadb** y la descargamos
- En el menú de Docker Desktop, seleccionamos la pestaña **"Images"** (Imágenes).
- En la barra de búsqueda, escribimos **"mariadb🦭"**.
- Aparecen varias opciones relacionadas con MariaDB, selccionamos la primera.

![image.png](image.png)

- Identificamos la imagen correcta con el nombre **"mariadb🦭"** y el ícono oficial.
- Verificamos que tiene **más de 1B+ descargas** y **5.9K estrellas** (esto confirma que es la imagen más utilizada y confiable).
- Hacemos clic en la imagen para seleccionarla.

![image.png](image%201.png)

***Verificación que la imagen se descargó correctamente***

- Vamos nuevamente a la pestaña "Images".
- Ahora, la imagen de MariaDB nos aparece en la lista de imágenes disponibles en tu sistema.

![image.png](image%202.png)

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

![image.png](image%203.png)

![image.png](image%204.png)

![image.png](image%205.png)

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

![image.png](image%206.png)

![image.png](image%207.png)

***Probamos la conexión y nos aseguramos de que funciona.***

![image.png](image%208.png)

 ***Crear una nueva base de datos***

- Hacemos clic derecho en la conexión con **MariaDB** y seleccionamos **"Crear Nuevo Database"**.
- Se nos abre una ventana llamada **"Create database"**.
- En **Database name**, escribimos el nombre de la base de datos, en este caso la llamamos `dbPelayoIker.`
- En **Charset**, seleccionamos **utf8mb4** (para compatibilidad con caracteres especiales y emojis).
- Opcionalmente, podiamos configurar **Collation**, pero en este caso lo dejarlo vacío para la opción por defecto.
- Hacemos clic en **"Aceptar"** para crear la base de datos.

![image.png](image%209.png)

![image.png](image%2010.png)

![image.png](image%2011.png)

***Seleccionamos la base de datos y crear una tabla***

- Hacemos clic derecho sobre la base de datos `dbPelayoIker` que acabamos de crear.
- Luego, hacemos clic derecho en **"Tables"** → **"Create New Table"**.
- Asignamos un nombre a la tabla , le ponemos por ejemplo,`ejemplo`.
- Agregamos las columnas necesarias:
    - `id` → **INT**, los marcamos como **Primary Key**, opción **Auto Increment**.
    - `nombre` → **VARCHAR(50)**, lo marcamos como **NOT NULL**.
- Guardamos los cambios y presionamos en **"Aceptar"**.

![image.png](image%2012.png)

![image.png](image%2013.png)

***Verificamos que la tabla se creo correctamente***

- Expandimos la base de datos `dbPelayoIker` en el panel izquierdo y hacemos clic en **"Tables"**.
- Vemos la tabla `ejemplo`, con lo cual se ha creado correctamente.

![image.png](image%2014.png)

***Detener y eliminar los contenedores***

- Abrimos **Docker Desktop**.
- En la pestaña **Containers**, buscamos el contenedores `bbdd`.
- Detenemos cada contenedor presionando el botón **Stop (🟥)**.
- Luego, eliminamos los contenedores con el botón **Delete (🗑️)**.

![image.png](image%2015.png)

***Verificamos que el volumen "datos-mariadb" sigue existiendo***

- En Docker Desktop, vamos a la pestaña **Volumes**.
- Buscamos el volumen `datos-mariadb`.
- Como se ve el volumen sigue ahi, lo que significa que los datos no se han perdido.

![image.png](image%2016.png)

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

![image.png](image%2017.png)

***Comprobamos que los datos siguen en el nuevo contenedor***

- Abrimos **DBeaver** y nos **conectatamos de nuevo a MariaDB** (`localhost:3306`, usuario `daw`).
- Verificamos que `dbPelayoIker` y la tabla `ejemplo` siguen existiendo.
- Como todo está correcto, los datos se han conservado gracias al volumen persistente.

![image.png](image%2018.png)

***Intentar borrar la imagen de MariaDB***

- En Docker Desktop, vamos a la pestaña **Images**.
- Intentamos eliminar la imagen de **MariaDB** (`Delete`).
- **¿Qué sucede?**
    - No podremos eliminar si hay contenedores en ejecución usándola (`bbdd-2`).
    - Tenemos que eliminar `bbdd-2` antes de poder borrar la imagen.

![image.png](image%2019.png)

![image.png](image%2020.png)

***Borrar todo (Volumen, Imagen y Contenedor)***

- Eliminamos los contenedor **`bbdd`** y **`bbdd-2`** desde Docker Desktop.

![image.png](image%2021.png)

- Eliminamos el volumen **`datos-mariadb`** desde la pestaña **Volumes**.

![image.png](image%2022.png)

- Eliminamos la imagen de MariaDB desde la pestaña **Images**.

![image.png](image%2023.png)