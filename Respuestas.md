# PracticaGit - Respuestas


**1. ¿Qué comando utilizaste en el paso 11? ¿Por qué?**

`git reset --hard HEAD~1`

Porque el comando reset permite desplazarse a otros commits, indicando --hard, se elimina el contenido del working station
y con HEAD hacemos que el head se desplace el numero de 
pasos que indiquemos en "~1".

--

**2. ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**

`git reflog`  y `git reset --hard bf45afd"
siendo bf45afd la referencia del commit al que había que retroceder

Con git reflog se puede ver cada paso realizado y la referencia de su correspondiente commit. copiando esta referencia e incluyendola en el comando "git reset --hard ", se puede acceder a ese paso.

--

**3. El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?**

No sucedió nada, debido a que ambas están en línea y la rama master no contenia nungún cambio nuevo que añadir a styled, siendo esta la última rama donde se realizaron cambios.

--

**4. El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?**

Sí. se habían creado dos modificaciones diferentes de don-quijote. Una en styled y otra en htmlify. Al hacer merge, git no puede decidir que información es la que se quedará en la version definitiva. Por eso muestra un conflicto. Junta en el archivo ambos cambios y solicita al usuario que lo modifique ocn la versión final, para poder hacer correctamente el merge una vez se realice un nuevo commit.

--

**5. El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?**


No, porque el merge realizado era un fast forward, y en merge no se habían realizado más cambios desde que se creó styled. De esta manera, al hacer merge para absorber styled en master. Lo que sucede es que master pasa a adquirir el mismo estado que styled, con los mismos cambios.

--

**6. ¿Qué comando o comandos utilizaste en el paso 25?**

`git graph` 

Con este comando se dibuja en el terminal un pequeño esquema que muestra los commits, ramas y merges realizados en el tiempo, así como la ubicación del head y las referencias de los commits.

--

**7.El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?**


Sí. Las dos ramas están en línea. Es decir, en master, despues de crear title no se realizó ningún cambio.
Para que fuese un no fast forward, debería de realizarse primero algún cambio en master, y despues realizar el merge.

--

**8. ¿Qué comando o comandos utilizaste en el paso 27?**

`git reset HEAD~1` 

Así se retrocede al commit anterior con HEAD, pero al no indicar *--hard*, no se pierde lo que hay en el working station.

--

**9. ¿Qué comando o comandos utilizaste en el paso 28?**

`git checkout don-quijote.md ` 

Este comando retira del working station el archivo mencionado. En este caso don-quijote.md

--

**10. ¿Qué comando o comandos utilizaste en el paso 29?**

`git branch -d title` y después `git branch -D title` para confirmar la acción

Primero, se indica que se desea eliminar la rama con el nombre *title*, y después se confirma la acción.

--

**11. ¿Qué comando o comandos utilizaste en el paso 30?**

`git reflog`´y después,`git reset --hard 2456aa0` 

Primero se busca la referencia del commit donde se realizó el merge. Con *reflog* y despues se retrocede, cambiando tambien el working station, con *git reset --hard*, indicando la referencia a la que se quiere acceder.



--

**12. ¿Qué comando o comandos usaste en el paso 32?**

`git reflog`´y después,`git reset --hard caf8375` 

Primero se busca la referencia del commit donde se realizó el merge. Con *reflog* y despues se retrocede, cambiando tambien el working station, con *git reset --hard*, indicando la referencia a la que se quiere acceder.

--

**13. ¿Qué comando o comandos usaste en el punto 33?**

`git reflog` y despues `git reset --hard 2456aa0` 

Primero se busca la referencia del commit donde se realizó el merge. Con *reflog* y despues se retrocede, cambiando tambien el working station, con *git reset --hard*, indicando la referencia a la que se quiere acceder.

--
