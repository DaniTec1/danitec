# git init
Iniciar Repositorio de Git

# git status -s
Muestra los archivos que hay en el proyecto que no 
han sido agregados o modificados en el repositorio

# git add (nombre archivo o un ".")
Añade uno o varios archivos al repositorio local

# git commit -m "(Comentario)"
Añadira una version de nuestro proyecto a nuestro
repositorio local

# git log --oneline
Muestra los Commits(Versiones) de nuestro proyecto

# git reset --hard ##id##
Colocara nuestro proyecto en una verison disponible
(Haras que tu proyecto viaje en el tiempo)

# git pull
compara los archivos de github con los locales y 
descarga los archivos faltantes

# git fetch
detecta cambios locales y los sube a github

# git tag "nombre" -m "descripcion"
Sirve para hacer versiones en local

# git push --tags
Sube tu version al repositorio remoto

# git branch "NombreRama"
Crea una rama del repositorio

# git branch
Muestra las ramas y nos dice en la que nos encontramos ubicados

# git checkout "NombreRama"
Se usa para movernos a la rama que vallamos a trabajar

# git merge "NombreRamaAUnir"
Se utiliza para unir la rama creada y modificada a la rama principal
*NOTA: Es necesario estar ubicados en la rama raiz(master)

# git branch -d "NombreRama"
Se emplea para Eliminar una rama
