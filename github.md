##Comandos GitHub I
- Añadir repositorio remoto:

 `git remote add origin url`

- Ver repositorios remotos:

 `git remote -v`
- Eliminar repositorio remoto:

 `git remote rm origin`
- Añadir cambios del repositorio local al remoto:

 `git push -u origin master`

- Añadir cambios del repositorio remoto al local:

 `git pull`

##Comandos GitHub II
- Ver branches remotos:

 `git branch -r`

- Ver todos los branches:

 `git branch -a`
- Clonar repositorio remoto:

 `git clone url`

##Dar seguimiento a _branches_ remotos
- **LOCAL → REMOTO:**
1. Cambios en el repositorio local.
2. Commit de los cambios.
3. Añadir cambios a repositorio remoto:

  `git push`
- **REMOTO → LOCAL:**
  - Sincronización y unión:
 ~~~
 git fetch origin
 git merge origin/master
 ~~~
 - En un solo paso:
 `git pull`
 
##Operaciones con _branches_ remotos
 - Creación:
   1. Crear branch local.
   2. Hacer cambios en dicho branch.
   3. Hacer commit.
   4. Copiar el branch al repositorio remoto:

    `git push -u origin branch_remoto`

 - Copia:

  `git checkout -b local remoto`
 - Eliminación:
  `git push origin --delete branch_remoto`
