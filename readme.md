# Práctica del curso de git, gitHub y Sourcetree

Respuestas de las preguntas planteadas el primer ejercicio del módulo 1. 

**Alumna:** Beatriz García Jiménez


### ¿Qué comando utilizaste en el paso 11? ¿Por qué?

Para deshacer el commit utilicé ``` git reset --hard HEAD~1``` ya que el uso de **--hard** nos permite eliminar los cambios en el working copy.

### ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué? 

Primero usé el comando ``` git reflog``` para mostrar el listado de todos los commits y encontrar la referencia al que deseamos volver.

Segundo ```git reset --hard 0de11cd``` donde  *75821c1* es el identificador o referencia. Con el uso de --hard vuelvo a modificar mi working copy donde estaba originalmente.

### El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

En este paso se nos pide que styled absorba a master, por lo que situándonos en la rama styled indicamos ```git merge master```. La consola nos devuelve ```Already up to date.```

No se produce conflictos porque la rama styled ya contenía a master.

### El merge del paso 19, ¿Causó algún conflicto? ¿Por qué? 

Cuando styled absorbe a htmlify tenemos un conflicto ````CONFLICT (content): Merge conflict in git-nuestro.md```` porque estamos modificando el mismo archivo en las mismas líneas desde dos ramas diferentes.

### El merge del paso 21, ¿Causó algún conflicto? ¿Por qué? 

El merge de master con Styled No crea conflicto porque es un Fast-forward.

### ¿Qué comando o comandos utilizaste en el paso 25? 

Dibujar el diagrama: 
```git log --graph --decorate --pretty=oneline```

--graph: muestra el gráfico

--decorate: muestra los punteros

--pretty=oneline: muestra cada commit resumido 

### El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

Sí, podría haber sido un fast forward porque compartían el mismo nodo de inicio.

### ¿Qué comando o comandos utilizaste en el paso 27?
Deshacer el merge (sin perder los cambios del working copy):

```git reset HEAD~1```

### ¿Qué comando o comandos utilizaste en el paso 28?

Como los cambios permanecen en mi working copy, para descartarlos reseteo a HEAD con --hard:

```git reset --hard HEAD```

### ¿Qué comando o comandos utilizaste en el paso 29?

Para eliminar la rama “title”:

``` git branch -D title```

### ¿Qué comando o comandos utilizaste en el paso 30?
Rehacemos el merge que hemos deshecho:

1. busco la referencia con ```git reflog```
2. reseteo a ese commit con ```git reset --hard e032f22```

### ¿Qué comando o comandos usaste en el paso 32?
1. busco la referencia con: ```git log --graph --decorate --pretty=oneline ```

2. ```git reset --hard bd40cda77884d10b05b470048a52fd49f7b4ebc4```

### ¿Qué comando o comandos usaste en el punto 33?

1. busco la referencia con ```git reflog```

2. me muevo al commit donde el título fue absorvido por master: 
```git reset --hard e032f22 ```






