##Ramas o *Branches*

* Es la forma para separar la línea actual de desarrollo con respecto a la principal. Normalmente representa versiones del software que poeteriormente son integradas a la línea principal.

![](https://uialberto.files.wordpress.com/2016/11/gitflowui.png?w=616&h=381)

##Comandos Ramas I
* Ver listado de ramas:

 `git branch`

* Crear una rama:

 `git branch nombre_rama`

* Cambiarnos a una rama:

 `git checkout nombre_rama`

* Crear una rama y moverse en un paso:
 `git checkout -b nombre_rama`

##Comandos Ramas II

* Ver ramas idénticas a la actual

 `git branch --merged`

* Renombrar ramas:

 `git branch -m nombre_antiguo nombre_nuevo`

* Eliminar ramas:

~~~
git branch -d nombre_rama
git branch -D nombre_rama
~~~

* Integrar ramas a la actual:

 `git merge nombre_rama`

* Resolver conflictos (se suele hacer manualmente)

 `git merge --abort`

##Comandos Ramas III

* Almacenar cambios temporales:

 `git stash save "Mensaje"`


* Listar cambios:

 `git stash list`


* Ver contenido de un cambio temporal:

 `git stash show -p nombre_stash`


* Eliminar un cambio temporal:

 `git stash drop nombre_stash `

* Aplicar cambios del stash:

~~~
git stash apply nombre_stash
git stash pop nombre_stash
~~~
