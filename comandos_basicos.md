# Práctica 1. Ingeniería del Software **(UCO)**

## Configuración Básica

- Nombre del administrador:

 `git config --global user.name "Antonio M. Durán Rosal"`

- Correo electronico:

 `git config --global user.email aduran@uco.es`

- Editor de texto:

 `git config --global core.editor "gedit"`

- Color de la interfaz

 `git config --global color.ui true`

- Listado de Configuración

 `git config list`

## Los tres estados de git

![estados de git](https://git-scm.com/figures/18333fig0106-tn.png)

## Comandos básicos I

- Iniciar repositorio en un repositorio

 `git init`

- Agregar cambios al area de staging:

 `git add`

- Validar cambios en el repositorio:

 ´git commit -m "Mensaje"

- Hacer los dos pasos anteriores en uno:

 `git commit -am "Mensaje"`

- Historial de commits
 
 `git log`

## Comandos básicos II

- Ayuda del listado anterior

 `git help log`

- Listar los 5 commits más recientes

 `git log -n 5`

- Listar los commits desde una fecha

 `git log --since=2018-09-18`

- Listar los commits por autor
 
 `git log --author="Antonio"`

- Ver cambios en el directorio

 `git estatus`

## Comandos Básicos III

- Ver diferencia entre ficheros en el directorio y el repositorio de git:

 `git diff`

- Ver diferencia entre ficheros en el *staging* y  el repositorio:

 `git diff staged`

- Eliminar archivos:

~~~
git rm archivo
git commit -m "Mensaje"
~~~

- Mover o renombrar archibos:

~~~
git mv antiguo nuevo
~~~

## Comandos Básicos IV

- Deshacer cambios con git:

 `git checkout -- nombre_fichero`

- Retirar archivos de staging

 `git reset HEAD nombre_fichero`

- Completar último commit:

 `git commit --amend -m "Mensaje"`

- Recuperar version de un fichero de commit antiguo:

 `git checkout <id_commit> -- nombre_archivo`

- Revertir un commit:

 `git revert <id_commit>`

## Comandos Básicos V

- Deshacer multiples cambios con el repositorio:

~~~
 git reset --soft <id_commit>
 git reset --mixed <id_commit>
 git reset --hard <id_commit>
~~~

- Listar archivos que git no controla:

 `git clean -n`

-Eliminar archivos que git no controla:

 `git clean -f`

- Ignorar archivos en el repositorio: .gitignore

## Comandos Básicos VI

- Listar el contenido del repositorio de git:

~~~
 git ls-tree master
 git ls-tree master^^^
 git ls-tree master~3
~~~

- Log en una linea:

 `git log --oneline`

- Log con los tres últimos commits en una linea

 `git log --oneline -3`

## Comandos Básicos VII

- Examinar el contenido de un commit:

 `git show <id>`

- Comparar un commit con el actual:

 `git diff <id> nombre_archivo`

- Comparar dos commits:

 `git diff id..id nombre_archivo`