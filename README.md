# Práctica 3
## Paso 1
Para empezar se tiene que crear la carpeta para el repositorio local y ejecutar el comando para que git se inicie en esa carpeta.
![Iniciar repositorio](/capturas/1.png)

## Paso 2
Depués creamos un archivo de python con una función básica de sumar para hacer pruebas con el mismo.
![Crear calculadora.py](/capturas/2.png)

## Paso 3
Añadimos el archivo al Staging Area donde luego aplicaremos los cambios con un mensaje de commit.
![Primer commit](/capturas/3.png)

## Paso 4
Modificamos el archivo y añadimos una nueva función para restar y aplicamos los cambios.
![Segundo commit](/capturas/4.png)

## Paso 5
Le damos una etiqueta al último commit realizado y los comparamos los dos commits con diff para ver las diferencias que tienen. <br>
![Comparacion diff](/capturas/7.png)

## Paso 6
Realizamos un cambio erroneo a forma de prueba y vemos con git status que el archivo tiene un cambio sin aplicar, pero como es un cambio erroneo, lo cancelamos con restore y revertimos los cambios.
![Uso del restore](/capturas/8.png)

## Paso 7
Realizamos otro cambio erroneo y esta vez lo añadimos al Staging Area y para eliminarlo utilizamos el restore pero con el parametro --staged para solo eliminarlo del Staging Area.
![Segundo uso del restore](/capturas/9.png)

## Paso 8
Esta vez si aplicamos los cambios con un error para probar el revert, que lo que realiza es hacer un nuevo commit con los cambios que tenia anterior al commit de el commit del error, es decir el commit C2.
![Uso del revert](/capturas/10.png)

## Paso 9
A partir del commit anterior donde utilizamos el revert, hacemos cambios del archivo de forma correcta y le hacemos un commit modificando el último commit, es decir el del revert.
![Modificar el commit del revert](/capturas/11.png)

### 3. Ejercicios de Autoevaluación
Responda a estas preguntas basándose en su trabajo en la terminal: <br>
Identificación de Versiones: ¿Cuál es el hash abreviado del commit donde solo existía la función sumar (C1)? <br>
662afe7 <br>
Referencia a un Ancestro: Escriba el comando exacto para hacer un viaje en el tiempo (switch o checkout) en modo desacoplado al commit inmediatamente anterior a la etiqueta v1.0-estable, usando la notación de ancestro (~ o ^). <br>
git switch –detach v1.0-estable^ <br>
Seguridad y Borrado: Si usted hubiera usado git reset --hard <HASH_C2> en lugar de git revert HEAD en el punto 3.4, ¿cuál habría sido la principal implicación si este repositorio estuviera compartido en GitHub con otros compañeros? <br>
Habría borrado los cambios hechos en el archivo para todos los integrantes y habría vuelto al primer commit ya que es el último guardado. <br>
Propósito de HEAD: Tras finalizar el punto 3.5, ¿a qué está apuntando HEAD en su repositorio? ¿A un commit específico (Detached HEAD) o a la rama principal (main)? <br>
Está apuntando a la rama principal ya que en ese punto se modifica el último commit realizado y automáticamente se pone el HEAD en ese mismo. 
