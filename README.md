# Configuración Git

Lo primero que deberás hacer es establecer tu nombre de usuario y dirección de correo electrónico. Esto es importante porque los **"commits"** de Git usan esta información y también puedes cambiarlas en cualquier momento volviendo a ejecutar los comandos correspondientes:

`$ git config --global user.name "Su nombre"`

`$ git config --global user.email "sucorreo@ejemplo.com"`

Para ver las configuraciones realizadas use el comando:

`$ git config --list`

Para mostrar el origen o ruta de los archivos de configuracion utilize el comando:

`$ git config --list --show-origin`


# Comandos basicos en Git

Para crear un repositorio nuevo.

`$ git init`

Este comando creara un respositorio Git, basicamente una carpeta oculta con el nombre `.git` y subcarpetas. Pero eso no es todo, tambien es creado un archivo inical llamado **HEAD** que hace referencia a la **rama master**.

Se crea tambien una área en memoria ram llamada **Staging "área de preparación"**

Para agregar un archivo al área de preparacion **"stating"** se utiliza el comando:

`$ git add nombre-archivo`

El archivo que estaba sin seguimiento **"untracked"**, pasa a ser un archivo en seguimiento **"tracked"**. Pasa a vivir en el área **staging** recuerda que es una area de preparacion.

Para que un archivo pase de la área **staging** al **repositorio** se utiliza el comando.

`$ git commit -m "Mi primer cambio"`

Cada vez que realizes un **commit** estas creando una nueva version de tu archivo.

Para mostrar los archivos en que **estado** se encuentran utiliza el comando.

`$ git status`

Mostrara el estado de los archivos **en seguimiento "tracked"** o **sin seguimiento "untracked"**.

Para ver los registros de los commits realizado utiliza el comando.

`$ git log`