# Clase 3

## RAMAS (Branches)

### Crear una rama

```sh
git branch <nombre-rama>
git branch reature/ramas
```
### Listar las ramas disponibles en mi repo

```sh
git branch
```

### Para moverme entre ramas

```sh
git switch <nombre-rama>
git switch feature/ramas
```

### Quiero crear una rama y al mismo tiempo moverme a esa rama

```sh
git switch -c feature/demo
```
### Quiero switchear entre las 2 ultimas ramas

```sh
git switch -
```

### Borrar una rama

```sh
git branch -d <nombre-rama>
git branch -d reature-rama
```
> Forfaz el borrado

```sh
git branch -D <nombre-rama>
git -D feature/sinmerge
```

# MERGE
Combina los cambios de la rama actual y la rama especificada.

## Tipos de merge (fusiones)

* Fast-Forward (No hay conflictos. Lo hace de forma automatica) [No agrega un commit]
* Recursivo (No hay conflictos. No se requiere ayuda de nosotros) [Agrega un commit al hacer la fusión]
* Manual (Si hay conflicto. Nosotros tenemos que resolver el conflicto y avisarle al git que lo solucionamos)

## Abortar la fusión

Si no tengo a la persona que me puede ayudar por ejemplo. Tendría que detener el proceso de merge

```sh
git merge --abort
```

## ¿Cuándo puede ocurrir que tenga un conflicto?
En ramas diferentes se modifica el mismo archivo en la misma ubicación. Osea en la misma linea de código.

```sh
git push <remoto> <rama-a-subir>
git push origin dev 
```

## ¿Cómo actualizar la metadata de nuestro repo local con la info del remoto?

```sh
git fetch
```

## ¿Cómo listar las ramas locales?

```sh
git branch -av # a:all -> todas | v:verbose -> más información
```

# STASH
El stash trabaja con una estructura de datos tipo pila. El primero que entra sale ultimo.

**Importante** Los stash no se puede subir al remoto

## Creo un stash 

```sh
git stash
```
## Listo los stash

```sh
git stash list
```

## Recupero o aplico el ultimo stash

```sh
git stash pop # se borra despues de aplicarse. Si entra en conflicto no se borra
```

