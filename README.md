# RetoDotCSV2080Super

Concurso del canal DotCSV gana una Nvidia 2080 Súper

## Objetivo:
Dar uso de las redes condicionales adversarias en el algoritmo pix2pix para obtener a partir de una imagen en blanco y negro al estilo Comic una imagen con características humanas. 

## Desarrollo:

Para afrontar este proyecto, se necesita un dataset con imágenes de personas y su equivalente en caricatura. Las fotos se obtuvieron de un dataset de rostros humanos (https://sites.google.com/view/sof-dataset) las cuales se seleccionaron sólo 50 y otras 50 de un sitio de fotos selfies (http://selfiecity.net/selfiexploratory/).

Al momento se disponía de 100 imagenes.

El dataset se preparó de la siguiente manera:

1-	Utilización del software XnConvert para trabajar las imágenes en lotes y renombrarlas a “sample__xx.jpg”

2-	Se utilizó una App para Android llamada “Comica”, la cual realiza la conversión a estilo cómic. Se convierte imagen por imagen a través de mi teleléfono celular.

3-	Se normalizan los tamaños de las imagenes tanto de input como de target.

4-  Se cuadriplicó el tamaño del dataset inviertiendo las imagenes en efecto espejo, con más brillo y con menos brillo.

5-	Se suben a google drive las imágenes normales a la carpeta ‘Target’ y las convertidas a cómic a la carpeta ‘Input’

# Se realizan pruebas con 3 escenarios:

a) Entrenamiento con 100 imágenes originales

b) Entrenamiento con 200 imágenes ( originales + imágenes espejadas)

c) Entrenamiento con 400 imágenes ( originales + imágenes espejadas + más brillo + menos brillo)

# Conclusiones

Las imágenes son muy escasas para predecir un rostro humano, pero al menos el sistema aprende en algunas imágenes a colorear el rostro y del color correcto.

La ampliación del dataset de la forma mencionada no parece ser efectiva, el resultado que más me convenció es las pruebas (a)

Más descripción y detalles del proyecto en youtube:

[Ver video explicativo](https://youtu.be/GQxsDHkLrZ8)



### Sobre mi:

Me llamo Bruno Diaz vivo en Mendoza, Argentina. Soy Ingeniero en Electrónica pero me encanta programar y estoy comenzando en el mundo del Machine Learning

