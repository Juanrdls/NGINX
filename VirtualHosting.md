# Virtual Hosting

## En esta práctica crearemos 2 sitios virtuales con nombre diferentes y vamos a poder acceder
desde un domino local

### 1.Procedemos el directorio de ambos sitios virtuales:

Dicho directorio es donde se va a guardar toda la información:

![5.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/5.PNG)

### 2.Creamos el archivo de configuración de cada sitio virtual de la siguiente forma:
 
Copiamos el archivo default que nos servirá como ejemplo y lo modificamos

![6.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/6.PNG)

### 3.Configuramos los archivos de configuración para que nos quede de la siguiente manera:

* WEB 1:

![7.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/7.PNG)

* WEB 2:

![8.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/8.PNG)

### 4.Comprobamos que la configuración es correcta

![18.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/18.PNG)

### 5.Procedemos a habilitar los sitios virtuales con un enlace duro hacia la siguiente ruta:

![12.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/12.PNG)

### 6.Reiniciamos el servicio para que se aplique la configuración:

``` systemctl restart nginx ```

### 7.Configuramos los DNS locales para poder acceder:

* Cliente de la **Red Interna: (192.168.3.10)**:

![10.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/10.PNG)

* Cliente con **Adaptador Puente**:

![11.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/11.PNG)
