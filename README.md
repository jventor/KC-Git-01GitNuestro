## CUESTIONARIO
### 1.- ¿Qué comando utilizaste en el paso 11? ¿Por qué?

```
git reset --hard HEAD~1
```

Porque con el reset HEAD~1 nos movemos al commit padre y con la opción *—-hard* sustituimos el WC por el del commit a donde nos movemos deshaciendo los cambios

### 2.- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

```
git reflog
git reset --hard 55214ac
```

Usamos el *git reflog* para obtener el historial de movimientos del HEAD donde buscamos el hash-id del commit anterior, y con el *reset —hard* volcamos el contenido de ese comió al WC descartando los cambios

### 3.- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué? 

No, porque indica que *“Already up-to-date”*. Es decir, que todos los cambios de la rama que deseas mergear ya están incluidos en la rama destino. Más concretamente, porque master es padre de styles. En definitiva, no hace nada 

### 4.- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

Si, se originó un conflicto porque ambas ramas habían modificado el archivo en las mismas lineas.

### 5.- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué? 

No porque se hace merge fastforward porque los nodos de commit forman una lista, así que no se crea un nuevo commit, simplemente se mueve el HEAD y master a la posición donde está la rama styled

### 6.- ¿Qué comando o comandos utilizaste en el paso 25?

```
git log --graph --abbrev-commit --pretty=oneline
```

Porque el comando git log  con la opción *-—graph* dibuja un grado simple. Con las otras opciones conseguimos que los commits se muestren compactos (mensaje en una sola linea y la version corta del hash)

### 7.- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

Si, porque forman una lista. HEAD y master simplemente se movería hasta el punto donde apunta title

### 8.- ¿Qué comando o comandos utilizaste en el paso 27? 

```
git reset HEAD~1
```

### 9.- ¿Qué comando o comandos utilizaste en el paso 28?

```
git checkout -- git-nuestro.md
```

### 10.- ¿Qué comando o comandos utilizaste en el paso 29?

```
git branch -D title
```

### 11.- ¿Qué comando o comandos utilizaste en el paso 30?

```
git reflog 
git reset --hard 223a34
```


### 12.- ¿Qué comando o comandos usaste en el paso 32? 
 
 ```
 git log
 git reset —hard 83ec3359371c7a58329a80a3a8609c06751fd622
 ```
Buscamos en el log el commit con el mensaje inicial copiamos el hash y después movemos HEAD 

### 13.- ¿Qué comando o comandos usaste en el punto 33? 

```
git reflog 		
git reset --hard HEAD@{1}
```
