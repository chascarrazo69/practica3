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
