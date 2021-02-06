# Vamos a configurar la autentificación mediante las IP
Si accedemos desde la **red externa** pedirá autorización pero la **red interna** no

### Pasos

### 1.Mantenemos la configuración

### 2.Configuramos el sitio virtual de nuevo

![28.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/28.PNG)

### 3.Comprobamos la configuración

![18.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/18.PNG)

### 4.Reiniciamos servicio

``` systemctl restart nginx ```

### 5.Comprobaciones

* Cliente de red externa

![26.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/26.PNG)

* Cliente de red interna

![27.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/27.PNG)
