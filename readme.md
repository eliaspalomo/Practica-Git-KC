# Practica 1

* ¿Qué comando utilizaste en el paso 11? ¿Por qué?
  * git reset --hard HEAD~1
    * Porque git reset HEAD~1, solo deshace el ultimo commit y con --hard deshace tambien lo que tenemos en la working copy

* ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
  * git reflog
    * para buscar el commit anterior 
  * git reset 876da37
    * posicionar el HEAD en el commit anterior
  * git add git-nuestro.md
    * añadir el archivo a la staging area
  * git commit -m "Rehacer el commit anterior"
    * añadir el archivo al repositorio

* El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
  * git branch
    * Para comprobar en la rama en la que me encuentro
  * git merge master
    * Ningun conflicto, porque master esta en un commit anterior al que se encuentra styled

* El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
  * git checkout styled
    * para movernos a la rama styled, nos da error porque perderiamos los cambios de git-nuestro.md
  * git add git-nuestro.md
    * añadir el archivo a la staging area
  * git commit -m "Commit para guardar los datos"
    * añadir el archivo al repositorio
  * git checkout styled
    * para movernos a la rama styled, con los cambios guardados
  * git merge htmlify
    * nos da un conflicto que debemos resolver para finalizar el merge

* El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
  * git checkout master
    * me cambio a master
  * git merge styled
    * No causo ningun conflicto porque master estaba en un commit anterior a styled

* ¿Qué comando o comandos utilizaste en el paso 25?
  * git log --graph
    * para dibujar el diagrama 

* El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
  * git merge --no-ff title
    * Si que podria hacerse fast forward, porque el commit en el que esta master es anterior al que esta title

* ¿Qué comando o comandos utilizaste en el paso 27?
   * git reset HEAD~1
     * deshace los cambios dejando  los cambios realizado en la working copy

* ¿Qué comando o comandos utilizaste en el paso 28?
  * git checkout -- git-nuestro.md
    * utilizo una version antigua, y como estan los cambios en la working copy, los quito

* ¿Qué comando o comandos utilizaste en el paso 29?
  * git branch -D title
    * elimina la rama de title

* ¿Qué comando o comandos utilizaste en el paso 30?
  * git reflog
    * para buscar el commit anterior 
 * git reset --hard 460d0eb
    * posicionar el HEAD en el commit anterior
  * git add git-nuestro.md
    * añadir el archivo a la staging area
  * git commit -m "Rehacer el commit anterior"
    * añadir el archivo al repositorio
  * git merge --no-ff title
    * hacer el merge anterior

* ¿Qué comando o comandos usaste en el paso 32?
  * git reflog
    * para buscar el commit 
  * git reset --hard 3a04672
    * para posicionarme en el primer commit
  
* ¿Qué comando o comandos usaste en el punto 33?
  * git reflog
    * para buscar el commit 
  * git reset --hard 0b4f6a4 
    * para posicionarme en el ultimo commit