# Git Desarrollo Markdown

## Clase 01

### Verificar que tengo instaldo git

```sh
git --version
```

---

### Markdown
Me permite documentar y tomar apuntes... Es un lenguaje de marcas, pariente del html

#### Títulos

# h1
## h2
### h3
#### h4
##### h5
###### h6

#### Listas ordenadas

1. Primer paso
2. Segundo paso
3. Tercer paso

#### Lista desordenada

* Item
* Item
* Item

---

## GIT

### Configuración inicial


> Agrego el usuario

```sh
git config --global user.name "Maximiliano Principe" # Global (Para todos los repos que se creen en este equipo)

git config --local user.name "Maximiliano Principe" # Local (Para este único repos) Este comando se tiene que ejecutar luego de haber creado un repositorio
```

> Agrego un correo

```sh
git config --global user.email "mlapeducacionit@gmail.com" # Global (Para todos los repos que se creen en este equipo)

git config --local user.email "mlapeducacionit@gmail.com" # Local (Para este único repos) Este comando se tiene que ejecutar luego de haber creado un repositorio
```

> Verificar las configuraciones hechas

```
git config --global --get-regexp user
```

**Nota**: Si por algun motivo ingresan el comando anterior y les abre un editor. Para salir. Ingresar en la consola :q => quit

### Inicializo un repositorio de GIT

```sh
git init # Va a crear en la carpeta del proyecto una carpeta  '.git' en el directorio (carpeta)
```

**IMPORTANTE**: No hay que borrar la carpeta .git, ni hay que modificar archivos dentro de ella. Solo trabaja git sobre esa carpeta, no nosotros

## Limpiar consola

```sh
clear
```

### GIT STATUS
¿Qué hace? Verifica el estado de los archivos. Porque los archivos pueden estar en varios estados

* UNTRACKED: Que los archivos aún estan en el working directory (WD) y no están siendo seguidos (controlados) por GIT.

* STAGED: Archivos que están preparando para crear el commit (Sacar la foto) el snapshot y preservar los cambios hechos de mi código fuente.

* UNMODIFIED: Si el archivo es detectado como sin cambios (sin modificaciones) es porque git está verificando que lo que tiene el WD con respecto al RL es lo mismo.

* MODIFIED: Si me aparece *modified* el archivo en el WD esta modificado con respecto a lo que tengo en el repositorio local (RL)
