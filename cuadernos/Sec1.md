
# Anatomía de Jupyter

## Frontend / Backend
Jupyter es una aplicación que se separa en dos partes la ejecución de código.
El *frontend* es el navegador y se encarga de mostrar texto que acompaña 
al código, el código en sí mismo, así como el resultado de los 
cálculos. Estos pueden ser numéricos o gráficos. 

El texto y el código se organizan en *celdas*. Cada celda puede ejecutarse por 
separado y potencialemente en cualquier orden.

El contenido de las celdas, así como los resultados, se almacenan en ficheros
con extensión `.ipynb`, denominados **cuadernos**. Internamente, los cuadernos
son ficheros [JSON](https://en.wikipedia.org/wiki/JSON) y utilizan *base64*
para almacenar resultdos como imágenes o videos. (Los cuadernos incrementan
su tamaño al ejecutarlos).

El *backend* o kernel se encarga de realizar los cálculos. Diferentes
kernels trabajan en diferentes lenguajes. Nosotros veremos ejemplos
con el kernel Python y el kernel R.

[Lista de kernels disponibles](https://github.com/jupyter/jupyter/wiki/Jupyter-kernels)


## Barras y menús

Cuando arrancamos Jupyter con el comando:

```
(taller) $ jupyter notebook
```

automáticamente arranca un navegador con el tablero (**dashboard**).
Aquí veremos los ficheros en el directorio donde hayamos arrancado (*Files*),
información sobre los cuadernos y terminales que tengamos arrancados (*Running*)e información sobre ejecuciones en paralelo (*Clusters*).

La solapa *Files* permite borrar o renombrar ficheros.

En la parte superior derecha (*New*) podemos arrancar terminales y cuadernos
de diferentes tipos.

## Celdas

## Markdown

Markdown es un lenguage de texto plano que puede convertirse en estructurado
(HTML). Existen versiones ligeramente diferentes del lenguaje. La que
utiliza Jupyter es la versión de Github

[En la ayuda de Jupyter](https://jupyter-notebook.readthedocs.io/en/stable/examples/Notebook/Working%20With%20Markdown%20Cells.html)

[Guía de Github](https://guides.github.com/features/mastering-markdown/)


# Conversión de cuadernos

# Cuadernos interactivos

# Ejecución remota de cuadernos

