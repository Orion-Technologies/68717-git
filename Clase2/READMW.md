# Clase 02

## .gitkeep: darle seguimiento a carpetas vacias
Me permite darle seguimiento a carpetas que debería estar dentro del proyecto a pesar de que no tenen archivos dentro.
Carpetas vacias que deben estar en el proyecto.

## Agregar un archivo
Pasa el arcivo al stage.

```sh
git add # . para agregar todos los archivos
git add <archivo> # agrega el archivo
```
## Commit
Pasa el archivo al repositorio.

```sh
git commit -m <mensaje>
```

## .gitignore: Me permite ignorar los archivos que le indeque
El **.gitignore** regularmente va en la raiz pero puede ir en cualquier lugar.
Se puede tener varios **.gitignore** para evitar rutas largar

> capeta1/carpeta2/carpeta3/...

Para cambiar el editor de git

```sh
git config --global core.editor "nano"
```

Más información en este link

*https://learning.oreilly.com/library/view/gitlab-cookbook/9781783986842/apas07.html#:~:text=The%20first%20is%20via%20the,with%20your%20editor%20of%20choice!*

## Ver todos los commits

```sh
git log
```
dentro de log se puede usar "/" como buscador de palabras claves
