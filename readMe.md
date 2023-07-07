# Los comando mas usados en git

## init
* Crea un nuevo repositorio Git en un directorio vacío o inicializa un repositorio existente.
```shell
    git init
```


## status
* Muestra el estado actual del repositorio, incluyendo los archivos modificados, agregados o eliminados.
```shell
    git status
```




 ## add   
* Agrega cambios al área de preparación (staging area) para ser incluidos en el siguiente commit.
```shell
    git add .
```    



## Reset
* Eliminar los cambios del stage
```shell
    git reset .
``` 



## Commit
* Crea un nuevo commit con los cambios agregados al área de preparación, utilizando un mensaje descriptivo.
```shell
    git commit -m "detalle del commit"
    git commit -am "detalle"
```

* Corregir el ultimo commit, SCAPE :wq!
```shell
    git commit --amend
``` 



## checkout
* Crear una rama apartir de la rama donde se encuentra
```shell
    git checkout -b <nombre-de-la-nueva-rama>
```
* Deshacer los cambios al ultimo commit.
```shell
    git checkout -- .
```
* Cambia a una rama existente.
```shell
    git checkout <nombre-de-rama>
```



## log
* Muestra un registro de commits realizados en el repositorio
```shell
    git log
```


## branch
* Eliminar una rama
```shell
    git branch -d <rama-a-borrar>
```
* Muestra la lista de ramas en el repositorio. La rama actual está resaltada.
```shell
    git branch
    git branch -a
```
* Renombrar un branch
```shell
    git branch -M main
```


## merge
* Fusiona una rama específica en la rama actual.
```shell
    git merge <nombre-de-rama>
```



## push
* Enviarlo al repo
```shell
    git push
```
* Envía los commits locales al repositorio remoto.
```shell
    git push -u origin main
```
* Verifica que se haya creado la etiqueta correctamente ejecutando el comando git tag. Ahora, para enviar la etiqueta al repositorio remoto, utiliza el siguiente comando:
*   Esto enviará la etiqueta específica que creaste al repositorio remoto llamado "origin".
```shell
    git push origin <tag_name>
```


## remote
* Asocia un repositorio remoto con tu repositorio local.
```shell
    git remote add origin <URL>
    git remote -v
```
* Verifica que la etiqueta se haya enviado correctamente ejecutando el comando 
```shell
    git ls-remote --tags.
 ```   


## clone
* Clona un repositorio remoto y crea una copia local en tu máquina.
```shell
    git clone <URL>   
```


## pull 
* Obtiene los últimos cambios del repositorio remoto y los fusiona con tu rama local.
```shell
    git pull
 ```
 
 ## diff
 * Muestra las diferencias entre el estado actual y el último commit.
```shell
    git diff
```

## stash
* Guarda temporalmente los cambios no comprometidos en una pila de cambios (stash) para que puedas cambiar de rama sin perder tu trabajo
```shell
    git stash
```


## tag 
* Crea la etiqueta utilizando el siguiente comando, reemplazando <tag_name> con el nombre que desees darle a la etiqueta:
```shell
    git tag <tag_name>
```

* También puedes agregar un mensaje descriptivo utilizando la opción -a y la opción -m:
```shell
    git tag -a <tag_name> -m "Mensaje descriptivo de la etiqueta"
```



  


