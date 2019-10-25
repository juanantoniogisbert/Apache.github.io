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




Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/juanantoniogisbert/Apache.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
