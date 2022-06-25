README PRACTICA 001_GIT -Manuel Ruiz Farrouh

¿Qué comando utilizas te en el paso 11?

   Utilizo el comando *git reset --hard HEAD~1*, porque elimina todos los cambios realizados en el working copy, dejando
   el staging area vacío.

¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

   Uso el comando *git reflog* para averiguar el hash SHA del commit anterior al reset, y, a continuación uso *git reset --hard* + SHA 
del commit que necesito para recuperar los cambios en el working copy.

El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

   No, es un merge fast-forward, realizado en la misma bifurcación de la rama, y no generó conflictos.

El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

   Si, fusionar la rama htmlify en styled provocó conflictos ya que las ramas se encontraban en diferentes bifurcaciones y eran dos
   versiones diferentes del mismo archivo, por lo qué había que gestionar esas diferencias.

El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

   No, es un merge fast-forward, por lo que git actualizo el archivo sin conflictos en le misma bifuración.

¿Qué comando o comandos utilizaste en el paso 25?

   Para visualizar el graph en git utilizo el alias personalizado *git graph* del comando *git log --graph --decorate --pretty=online*

El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

   Si, podría ser un merge fast forward, puesto que se encuentran en la misma bifurcación del grafo y no necessitaría crear un nuevo commit.

¿Qué comando o comandos utilizaste en el paso 27?

   Uso *git reset* mas el SHA del commit anterior al merge (donde añadí el título). El working copy no se ve afectado.

¿Qué comando o comandos utilizaste en el paso 28?

   En el staging area no hay cambios puesto que el paso anterior no hizo ninguna modificación en el working copy, salvo deshacer el merge.

¿Qué comando o comandos utilizaste en el paso 29?

   Utilizo el comando *git branch -d title*.

¿Qué comando o comandos utilizaste en el paso 30?

   Uso el comando *git reflog* para encontrar el SHA del merge no fast forward anterior y el comando *git reset --hard* + SHA del merge para
   recuperar y dejar en el working copy todo como estaba hasta ese momento.

¿Qué comando o comandos usaste en el paso 32?

   Utilizo el comando *git reset* mas SHA del primer commit donde creé el archivo git-nuestro.md.

¿Qué comando o comandos usaste en el punto 33?

   Uso *git reset* + SHA del comit donde añadí el título personalizado al archivo git-nuestro.md.


---------------------------------------------------------------------------------------------------------------------------------------------

ANEXO

En la última petición del paso 34 (añadir el tag title en la modificación del paso 30), dicho paso 34 era "rehacer el merge que hemos deshecho"
por lo que ha sido justo ahí donde he puesto el tag solicitado.


