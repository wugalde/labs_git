# Los comando mas usados en git
```shell

1. Crea un nuevo repositorio Git en un directorio vacío o inicializa un repositorio existente.
    git init
    

2. Agrega cambios al área de preparación (staging area) para ser incluidos en el siguiente commit.
    git add .

3. Eliminar los cambios del stage
    git reset .

4. Crea un nuevo commit con los cambios agregados al área de preparación, utilizando un mensaje descriptivo.
    git commit -m "detalle del commit"
    git commit -am "detalle"

5. Deshacer los cambios al ultimo commit.
    git checkout -- .

6. Muestra un registro de commits realizados en el repositorio
    git log

7. Corregir el ultimo commit, SCAPE :wq!
    git commit --amend

8. Crear una rama apartir de la rama donde se encuentra
    git checkout -b <nombre-de-la-nueva-rama>

9. Muestra la lista de ramas en el repositorio. La rama actual está resaltada.
    git branch
    git branch -a

10. Cambia a una rama existente.
    git checkout <nombre-de-rama>

11.  Fusiona una rama específica en la rama actual.
    git merge <nombre-de-rama>

12. Eliminar una rama
    git branch -d <rama-a-borrar>

13. Enviarlo al repo
    git push

14. Asocia un repositorio remoto con tu repositorio local.
    git remote add origin <URL>
    git remote -v

15. Renombrar un branch
    git branch -M main

15. Envía los commits locales al repositorio remoto.
    git push -u origin main

16. Clona un repositorio remoto y crea una copia local en tu máquina.
    git clone <URL>   

17.  Muestra el estado actual del repositorio, incluyendo los archivos modificados, agregados o eliminados.
    git status

18.  Obtiene los últimos cambios del repositorio remoto y los fusiona con tu rama local.
    git pull
 
 19. Muestra las diferencias entre el estado actual y el último commit.
    git diff

20.  Guarda temporalmente los cambios no comprometidos en una pila de cambios (stash) para que puedas cambiar de rama sin perder tu trabajo
    git stash

21. Crea la etiqueta utilizando el siguiente comando, reemplazando <tag_name> con el nombre que desees darle a la etiqueta:
    git tag <tag_name>

22. También puedes agregar un mensaje descriptivo utilizando la opción -a y la opción -m:
    git tag -a <tag_name> -m "Mensaje descriptivo de la etiqueta"

23. Verifica que se haya creado la etiqueta correctamente ejecutando el comando git tag. Ahora, para enviar la etiqueta al repositorio remoto, utiliza el siguiente comando:
    git push origin <tag_name>
    Esto enviará la etiqueta específica que creaste al repositorio remoto llamado "origin".

24. Verifica que la etiqueta se haya enviado correctamente ejecutando el comando 
    git ls-remote --tags.
```