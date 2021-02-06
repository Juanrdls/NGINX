# Autentificación

El cliente de la **red interna** podrá acceder a ambas páginas, pero el cliente externo solo podrá 
acceder a una de ellas:

### Pasos:

### 1.Mantenemos la configuración del fichero /etc/hosts

### 2.Modificamos el sitio virtual:

* WEB 1:
A esta página solo podrá acceder las IP que provengan de la red 1.0 y 3.0 **La opción "Deny all" es
opcional**:

![16.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/16.PNG)

* WEB 2:
A esta página solo podrá acceder las ip que vengan de la red 3.0 y deniega las demás conexiones

![17.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/17.PNG)

### 3.Comprobamos que la configuración está bien:

![18.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/18.PNG)

### 4.Riniciamos el sistema:

``` systemctl restart nginx ```

### 5.Comprobaciones:

* **Cliente de la red externa:** --> Podrá acceder a la web1.org pero **NO** a la web2.org

![20.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/20.PNG)

![19.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/19.PNG)

* **Cliente de red interna:** --> Podrá acceder a **ambas** páginas

![21.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/20.PNG)

![15.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/15.PNG)
