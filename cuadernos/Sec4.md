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
