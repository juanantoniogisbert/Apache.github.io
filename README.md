## Práctica Apache

Primeramente instalaremos Apache, esto es un servidor web `http` existe para todas las plataformas actualmente, se usa principalmente para enviar páginas web estáticas y dinámicas en www.

Para instalar Apache realizaremos los siguientes comandos.

```markdown
$ sudo apt-get update
$ sudo apt-get install apache2
```

### SITIO 1

Ahora vamos a realizar la siguiente configuración para nuestro sitio.

- Estar publicada en el puerto 82.
  Una vez instalado el Apache deberemos de hacer los siguientes comandos:
  ```markdown
  Acceder a la siguiente carperta.
  $ cd /etc/apache2/sites-available

  En esta carpeta crearemos el fichero sitio1.conf
  $ sudo touch sitio1.conf
  ```
  ![Alt text](images/cap1.png?raw=true "Title")

  Ahora editamos el fichero:
  ![Alt text](images/cap2.png?raw=true "Title")

- Directorio en /var/www/sitioPhp

  Primeramente no dirigimos al directorio /var/www
  ![Alt text](images/cap3.png?raw=true "Title")

  Crearemos la carperta y luego crearemos el index dentro de la misma.
  ```markdown
  $ sudo mkdir sitioPhp
  $ cd sitioPhp
  $ sudo touch index.php
  ```
  ![Alt text](images/cap4.png?raw=true "Title")

  Detro del index.php pondremos lo siguiente.
  ![Alt text](images/cap5.png?raw=true "Title")

  Ahora crearemos el directorio de nuestros logs en:
  ![Alt text](images/cap6.png?raw=true "Title")

  Creamos el fichero "log_personalizado.log" y añadimos la siguiente linea
  ```markdown
  LogFormat "%t %h %m %>s" PhpLogFormat
  ```
  Para poder acceder a nuestro sitio web tenemos que hacer tenemos que hacer que escuche nuestro puerto en el siguiente fichero de configuracion.
  ![Alt text](images/cap7.png?raw=true "Title")

  Despues tenemos que habilitar nuestro fichero .conf con el siguiente comando.
  ```markdown
  $ sudo a2ensite sitio1
  ```
  
  Ahora comprobamos que todo funciona y hacemos la prueba de error.
  ![Alt text](images/cap8.png?raw=true "Title")
  ![Alt text](images/cap9.png?raw=true "Title")



### SITIO 2

Ahora vamos ha crear el segundo sitio, tendremos que seguir algunos de los pasos que hemos utilizado en el sitio anterior
pare ello realizaremos los siguientes comandos.


Primeramente no dirigimos al directorio /var/www

Crearemos la carpeta
```markdown
$ sudo mkdir sitioNode
```
![Alt text](images/cap10.png?raw=true "Title")

También crearemos la carpeta de logs en /etc/logs
```markdown
$ sudo mkdir sitioNode
```
![Alt text](images/cap11.png?raw=true "Title")



