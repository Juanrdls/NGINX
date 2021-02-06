# Autentificación

## Vamos a configurar el sitio virtual de web1 para que cuando accedamos a la ruta /prueba nos pida
una autentificación

La autentificación nos sirve par proteger el contenido de nuestra página

### Pasos:

### 1.Creamos el directorio prueba de nuestra página web
Para ellos nos metemos en el **directorio** y creamos la carpeta

![22.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/22.PNG)

### 2.Instalamos el paquete (apache2-utils)
Este paquete nos sirve para crear usuarios en texto plano pero con contraseña encriptada

![23.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/23.PNG)

### 3.Creamos a los usuarios que van a poder acceder a la ruta
Creamos una carpeta en la que se guradarán el archivo con los usuarios autentificados y luego 
procemos a crearlos

![24.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/24.PNG)

### 4.Configuramos el sitio virtual de Web1 para habilitar la autentificación
Añadimos en el ultimo párrafo donde especificamos que ruta queremos proteger

**auth_Basic:** Mensaje que se muestra cuando nos pida la autentificación

**auth_basic_user_file:** Es el archivo donde se guardan los usuarios que pueden acceder

![25.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/25.PNG)

### 5.Comprobamos la configuración

![18.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/18.PNG)

### 6.Reiniciamos el servicio

``` systemctl restart nginx ```

### 7.Comprobaciones

![26.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/26.PNG)

![27.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/27.PNG)
