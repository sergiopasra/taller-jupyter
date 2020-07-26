# Taller de Jupyter

<!--- This is an HTML comment in Markdown -->

Jupyter es una aplicación web que permite generar
documentos (cuadernos) que contienen código, texto,
ecuaciones y visualizaciones.

## Instalación

Para la instalación podemos visitar http://www.jupyter.org

En la sección **The Jupyter Notebook**, tenemos dos opciones:
 **Try in in your browser** e **Install the Notebook**

De nuevo tenemos opciones para instalar varios programas. 
Buscamos la sección **Getting started with the classic Jupyter Notebook**,
donde tenemos instrucciones para instalar utilizando *conda* o *pip*.

Jupyter es una aplicación Python, así que require un entorno de Python.
Tanto en Linux como en Mac, Python viene instalado por defecto. Sin embargo,
es preferible trabajar en un entorno aislado del Python del sistema para
evitar problemas de compatibilidad.

Las dos maneras más habituales de trabajar con un entorno aislado Python
son *pip* y *conda*. *Pip* es el instalador nativo de Python y *conda* es sistema alternativo que permite instalar no solo paquetes de Python sino programas (como por ejemplo R).


En caso de no tener experiencia previa, creo que lo más sencillo es instalar 
Jupyter con *pip* en Linux y con *conda* en Mac.

### Pip

El primer paso es crear un *entorno virtual*. De esa manera usaremos un Python aislado del Python del sistema, donde podremos instalar y desintalar paquetes sin permisos de administrador.

En una terminal, escribimos:

```
$ python3 -m venv taller
```

Este comando nos creará un directorio `taller` con toda la estructura
de directorios de Python. A continuación hay que activar el entorno, lo 
que hará que, en esa terminal en particular, el comando `python` invoque
el ejecutable en `taller/bin/python`.

La activación se realiza con:
```
$ source taller/bin/activate
```

A continuación , el *prompt* cambia para indicar que estamos dentro del
entorno:

```
(taller) $
```

Para salir del entorno, basta escribir `deactivate` (o cerrar la terminal).

La instalación de Jupyter es simplemente:

```
(taller) $ pip install notebook
```

para ejecutar el cuaderno, en la terminal podemos:


```
(taller) $ jupyter notebook
```

### Conda

La instalación de conda está detallada en 
https://docs.anaconda.com/anaconda/install/

Una vez instalado conda, creamos un entorno con:

```
$ conda create --name taller
```

Activamos el entorno con:
```
$ conda activate taller
```

E instalamos con:

```
(taller) $ conda install -c conda-forge notebook
```

### Kernel R para Jupyter
Jupyter se compone de una aplicación web que muestra los cuadernos y un **kernel** que ejecuta las intrucciones. El kernel de Python viene por defecto, pero
para ejecutar instrucciones en otros lenguajes hay que tener instalado el kernel correspondiente.

[Lista de kernels disponibles](https://github.com/jupyter/jupyter/wiki/Jupyter-kernels)

Para instalar el kernel R, si estamos utilizando conda basta con hacer:

```
(taller) $ conda install -c conda-forge r-irkernel
```

En Linux, se puede instalar el paquete precompilado:

En Fedora:
```
$ dnf install R-IRkernel
```

En Ubuntu:
```
$ apt-get install r-cran-irkernel
```

para más información, esta es la página del kernel R: https://irkernel.github.io/

### Widgets
Los controles interactivos se pueden instarlar tanto con `pip` como con `conda`.

Con pip:

```
pip install ipywidgets
jupyter nbextension enable --py widgetsnbextension --sys-prefix
```
La opción `--sys-prefix` es necesaria en entornos virtuales.

Con conda:
```
conda install -c conda-forge ipywidgets
```


