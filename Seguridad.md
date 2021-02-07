# Seguridad

## En este apartado vamos a proceder a instalar un certificado para nuestro virtual hosting

### Pasos

### 1.Creamos una carpeta en la cual guardaremos los certificados y procedemos a instalar el 
paquete (openssl ca-certificates)
La frase que nos pide debemos recordarla

![36.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/36.PNG)

### 2.Generamos la clave privada con la que cifraremos el certificado

![37.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/37.PNG)

### 3.Generamos el certificado el cual *todavía no está firmado*
Rellenamos los datos y sobre todo **debemos introducir correctamente el FQDN**

![38.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/38.PNG)

### 4.Firmamos el certificado con la clave que habiamos generado antes
Para ello debemos introducir la frase que nos pidió en el paso 1

![39.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/39.PNG)

### 5.En la carpeta que hemos creado debemos tener los siguientes archivos:

![40.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/40.PNG)

### 6.Configuramos el sitio virtual para que se active la navegación segura:

![41.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/41.PNG)

### 7.Comprobamos la configuración

![18.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/18.PNG)

**Reiniciamos el Sistema**

``` systemctl restart nginx ```

### 8.Comprobaciones

![43.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/43.PNG)

![44.png](https://github.com/Juanrdls/NGINX/blob/main/Capturas/44.PNG)
