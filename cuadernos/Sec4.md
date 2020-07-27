# Conversión de cuadernos

Los cuadernos son ficheros en formato JSON que la
aplicación Jupyter es capaz de mostrar. Si queremos
poder ver los cuadernos sin utilizar Jupyter, tenemos que
convertirlos a otro formato.

Los cuadernos pueden convertirse a diferentes formatos, utilizando
el menu `File->Download as` de la aplicación web o el comando `nbconvert`
en la consola. Este último es más versátil ya que permite pasar opciones
que pueden modificar la conversión.

Utilizaremos como ejemplo el cuaderno de R [prac\_estat.ipynb](prac_estat.ipynb)

## HTML

Basta con seleccionar `File->Download as->HTML` para generar una versión
estática del cuaderno

## PDF
Para generar el PDF, se convierte el cuaderno a latex. Esta conversión suele
requerir tener una instalación extensa de latex, con un buen montón de
módulos (es difícil que funcione bien a la primera).

## Slides
Este es un formato de presentación basado en HTML con Javascript (https://revealjs.com/).

Para establecer el la jerarquía de las celdas, utilizamos un menú especial:
`View->Cell Toolbar->SlideShow`. Sobre cada celda aparece un menú desplegable
que indica el orden en el que se distribuyen las celdas.

* *Slide* es un transparencia, cada una parece a la *derecha* de la anterior
* *Sub-Slide* es una transparencia que aparece *debajo*
* *Fragment* aparece *dentro* de la anterior transparencia
* *Skip* se ignora
* *Notas* aparece solo para el presentador



