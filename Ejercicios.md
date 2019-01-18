
1. Tienes que modificar la escena 5 de Hamlet en el fichero scene-5.txt. En dicha escena Hamlet encuentra al fantasma de su padre. Añade este texto al fichero:
> Ghost: 
> My hour is almost come,
> When I to sulphurous and tormenting flames
> Must render up myself.

Edito el fichero con el comando nano scene-5.txt y añado la linea al final

2. Añade scene-5.txt al área de preparación.

Añado el fichero al área de preparacion con git add scene-5.txt

3. Haz un commit con los cambios con un buen mensaje de commit.

git commit -m "añadiendo cambios a scene-5.txt"

4. Modifica las palabras del fantasma. Aquí tienes una sugerencia divertida:
> Ghost: 
> My hour is almost come,
> When I to sulphurous and tormenting balloons
> Must render up myself.

Edito con nano scene-5.txt

5. Devuelve el fichero al estado del último commit.

Utilizo el comando git reset --hard

6. Cambia el nombre de LARRY por LAERTES en los ficheros scene-3.txt y scene-7.txt.

Edito los ficheros con nano scene-3.txt y nano scene-7.txt

7. Añade los ficheros al área de preparación usando un único comando git.

Utilizo el comando git add .

8. Vamos a cometer un error a propósito. Borra cualquier línea del fichero scene-2.txt.

Edito con nano scene-2.txt

9. Añade scene-2.txt al área de preparación.

Utilizo git add scene-2.txt

10. Comprueba el estado del repositorio. 

Utilizo git status

11. Devuelve scene-2.txt al directorio de trabajo.

git rm --cached scene-2.txt

12. Haz un commit para guardar los cambios realizados en el nombre de Larry por Laertes.

git commit -m "ejercicio 12"

13. Busca el primer commit que has hecho y vuelve a dicho commit. Indica como has buscado el commit anterior y como has vuelto a él.

Utilizo el comando git log para ver el historial de commits
git reset --hard 24330a9113ce68509cfb78a62780c3c3e0a16a86

14. Crea una nueva rama llamada **reinventando_hamlet**

git branch reinventando_hamlet

15. Cámbiate a dicha rama

git checkout reinventando_hamlet

16. Mejora la escena 2 como creas conveniente.

Edito con nano scene-2.txt

17. Haz un commit con los cambios con un mensaje adecuado.

git add .
git commit -m "ejercicio17"

18. Vuelve a la rama master.

git checkout master

19. Elimina la rama **reinventando_halet**

Usamos el comando  el comando 'git branch -D reinventando_hamlet'

20. Crea una nueva rama, modifica algo en la rama master, haz commit y llévate los cambios a la rama que has creado.

Creamos la nueva rama con 'git branch ejercicio20'
Modificamos un archivo con 'nano scene-5.txt'
Añadimos al área de preparación con 'git add .'
Hacemos commit 'git commit -m "ejercicio200"'
Usamos 'git merge ejercicio20'

21. Provoca un conflicto entre la rama master y la rama que has creado (indica lo que has hecho). Une la rama a la rama master resolviendo el conflicto.

Creamos un archivo prueba en Ejercicio20 - nano Ejercicio20.txt
Hacemos git add .
Hcemos git commit -m "21"
Nos movemos a master - git checkout master
Creamos y editamos otro archivo con el mismo nombre y con contenido distinto con nano Ejercicio20
Hacemos git add .
Hcemos git commit -m "21"
Hacemos un merge - git merge conflict
Nos da un conficto, abrimos el archivo y solucionmos - nano Ejercicio20.txt
Hacemos git add .
Hcemos git commit -m "Conflicto resuelto"

