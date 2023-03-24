# masteruah
-- Clonar del repositorio de git a local

git clone https://github.com/inmatapias/masteruah

-- Acceder al directorio masteruah

cd masteruah/

-- Añadir a masteruah un readme

git add README.md

-- hacer commit inicial

git commit -m "commit inicial"

-- hacer push inicial

git push

-- crear fichero 1

captura || git add "fichero_1.txt"

-- commit del fichero 1

git commit -m "añadir fichero 1.txt"

-- crear tag v0.1

git tag v0.1

-- subir tags

git push --tags

-- crear rama v0.2

git branch v0.2

-- cambiar a rama v0.2

git checkout v0.2

-- crear fichero 2 en rama 2

echo "Contenido del fichero 2" > 2.txt || git add 2.txt || 

git commit -m "Añadir fichero 2.txt a la rama v0.2"

-- Subir los cambios hechos

git push -u origin origin v0.2

-- Posicionarse en la rama main

git checkout main

-- Hacer un merge de la rama v0.2

git merge v0.2

-- Escribir "hola" en el fichero 1 txt 

git add "fichero 1.txt" || git commit -m "Agregado Hola en fichero 1.txt en la rama main"

-- posicionarse en la rama v0.2

git checkout v0.2


-- Escribir adios en el fichero 1 txt

echo "Adios" > "fichero_1.txt" || git add "fichero_1.txt"

-- Commit de lo anterior

git commit -m "Agregado Adios en fichero_1.txt en la rama v0.2"


-- Volver a la rama main para hacer el merge con conflicto

git checkout main || git merge v0.2


-- Listar ramas con merge || sin merge

git branch --merge || git branch --no-merge

-- corregir cambios de ficheros y guardar

vim "fichero_1.txt" || para guardar, shift+: y wq || git add "fichero_1.txt"

-- commit de lo anterior

git commit -m "Resuelto conflicto en fichero 1.txt"

-- crear tag v0.2

git tag v0.2

-- Borrar rama v0.2

git branch -D v0.2

-- listar todos los cambios hechos

git log --oneline --decorate --all

-- cambiar ajustes de usuario en git

pulsar en icono del usuario -> settings

-- poner el doble factor de autentificación

settings -> password and authentication

-- Generar key ssh

entrar a cmd -> ssh-keygen -> nombre: github 

entrar otra vez al cmd git -> cd ~/.ssh -> ssh-keygen -> cat ~/.ssh/github

copiar el texto y pegarlo en la pagina de git, ponerle nombre y guardar.
