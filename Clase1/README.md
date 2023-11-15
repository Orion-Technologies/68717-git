# Git Desarrollo Markdown

## Clase 01 😎

### Verificar que tengo instalado git

```sh
git --version (snipet)
```

```js
function sumar(a, b) {
    return a + b;
}
```

### Markdown
# h1
## h2
### h3
#### h4
##### h5
###### h6

### Listas ordenadas

1. Primer paso
2. Segundo paso
3. Tercer paso

### Listas desordenadas

* item 1
* item 2
* item 3

---

## GIT

### Inicializo in repositorio de GIt

```sh
git init # crea una carpeta del proyecto. '.git' en el directorio.
```

### GIT STATUS
¿Qué hace? Verifica el estado de los archivos. Los estados pueden ser:

* UNTRACKED: Los archivos aún  no estan en el working directory (WD) y no estan siendo seguidos.

* STAGED: Archivos que estan preparados para commit (snapshot) y preservar los cambios hechos.

* UNMODIFIED: Si el archivo es detectado com osin cambios (sin modificaciones) es porque gir esta verificando que lo que tieneel WD con respecto al RL es lo mismo,

* MODIFIED: Si aparece modifed en el WD esta modificado con respecto a lo que se tiene en el repo(LR).