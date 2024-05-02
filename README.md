# Alternativa a Xampp para trabajar con PHP

Para aquellos que tengan problemas para trabajar con PHP usando Xampp, os propongo una alternativa más sencilla, rápida y "libre", ya que no estaréis sujetos a las versiones de PHP, Apache y MySQL que vienen con la última versión de Xampp.

**Nota**: Estos pasos son válidos para Linux, Mac y Windows (en este último caso, si estáis usando WSL2).

## Pasos

### 1. Eliminar Xampp
Elimina cualquier rastro de Xampp en tu equipo.

**Importante**: No necesitas hacer nada especial con tus proyectos de PHP. Si los eliminas, tus archivos y proyectos existentes no se perderán. Podrás seguir corriéndolos donde estén, simplemente tendrás que correr el comando para lanzar el servidor PHP desde la raíz del directorio usando la terminal de VSCode, por ejemplo.

### 2. Instalar PHP
Para Linux, usa los repositorios disponibles. En distribuciones basadas en Debian/Ubuntu, ejecuta:


    apt install php

Para Mac, usa Homebrew, que es como un repositorio de Linux pero para macOS. Instala PHP con:

    brew install php


Ahora ya tienes PHP en tu equipo y un servidor rápido con el que trabajar. Puedes iniciar proyectos de PHP en cualquier lugar de tu disco duro. Solo abre una terminal en la raíz del proyecto y ejecuta:

    php -S localhost:8000

Como escribir eso da palo, lo mejor es que creéis un alias en vuestro intérprete de comandos, normalmente bashen Linux y zsh en Mac. El comando para crear un alias una vez que estáis en el perfil de bashrc o zsh con un editor de texto sería este:

    alias ps="php -S localhost:8000"

### 3. Instalar MySQL

Para instalar MySQL en Linux, ejecuta:

`apt install mysql-server`

Para Mac, usa:

`brew install mysql`

## ¡Listo!

Con esto, ya puedes usar cualquier programa para visualizar bases de datos o trabajar directamente desde Visual Studio Code con uno de los muchos complementos disponibles.
