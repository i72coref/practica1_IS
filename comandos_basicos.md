##Configuracion Básica

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

##Los tres estados de git

![estados de git](https://git-scm.com/figures/18333fig0106-tn.png)

##Comandos básicos I

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