# Practica git y github

## ¿Qué comando utilizaste en el paso 11? ¿Por qué?

Utilice el comando *git reset --hard HEAD~1* porque es el comando para deshacer el último commit y el working copy. Con este comando el staging área queda vacío.

## ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

Utilice el comando *git reflog show* para ver el historial de los logs de referencia del repositorio. Luego utilice *git reset <hash>*.

## El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

No causó ningún conflicto, porque hice el merge desde la rama styled. Ejecutando el comando *git merge main* de esta manera styled absorbe a main.
 
## El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

Causó un conflicto, el merge fallo porque el archivo de git-nuestro.md en la rama styled es diferente al archivo git-nuestro.md en la rama htmlify. Pide que arregle los conflictos y luego se haga el commit. Abrí el archivo, me quedé solo con el contenido de la rama styled -> guardado -> commit. 

## El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

No me causó ningún conflicto. Se hizo el merge correctamente, con Fast-forward, 1 cambio en el archivo de git-nuestro.md con 9 inserciones y 9 eliminaciones.

## ¿Qué comando o comandos utilizaste en el paso 25?

Para visualizar el log graph utilice el comando: *git log --all --decorate --oneline --graph*

## El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

Hice el merge con *git merge --no-ff <branch>* como indicaba en el paso 26. Sin embargo, el merge se podría hacer con fast-forward, ya que en ningún caso, ni haciendo *git merge <branch>* ni con la opción *(--no-ff)* se verá afectado el código, solo cambia la forma en la que visualizamos el histórico del repositorio. 

## ¿Qué comando o comandos utilizaste en el paso 27?

Utilice el comando *git reset HEAD~1* 

## ¿Qué comando o comandos utilizaste en el paso 28?

Utilice el comando *git status* -> nano git-nuestro.md -> para descartar el título.

## ¿Qué comando o comandos utilizaste en el paso 29?

Para eliminar una rama utilice el comando *git branch -D <rama>* 

## ¿Qué comando o comandos utilizaste en el paso 30?

Utilice el comando *git reflog* -> para buscar la referencia del hash de donde se había hecho el merge de title en main -> *git merge <hash>* -> para hacer el merge del commit en la rama main.

## ¿Qué comando o comandos usaste en el paso 32?

Utilice el comando *git log* -> para encontrar el commit inicial donde se creó el poema - > luego *git checkout <hash>*, con eso voy al commit donde se creó el poema.

## ¿Qué comando o comandos usaste en el punto 33?

Para volver al estado final, cuando pusimos título al poema utilice el comando *git switch main* vuelve a la rama donde estaba antes.
