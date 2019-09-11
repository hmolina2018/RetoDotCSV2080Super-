# RetoDotCSV2080Super

Concurso del canal DotCSV gana una Nvidia 2080 Súper

##Objetivo:
Dar uso de las redes condicionales adversarias en el algoritmo pix2pix para obtener a partir de una imagen en blanco y negro al estilo Comic una imagen con características humanas. 

##Desarrollo:

Para afrontar este proyecto, se necesita un dataset con imágenes de personas y su equivalente en caricatura. Las fotos se obtuvieron de un dataset de rostros humanos (https://sites.google.com/view/sof-dataset) las cuales se seleccionaron sólo 50 y otras 50 de un sitio de fotos selfies (http://selfiecity.net/selfiexploratory/).

Al momento se disponía de 100 imagenes.

El dataset se preparó de la siguiente manera:
1-	Utilización del software XnConvert para trabajar las imágenes en lotes y renombrarlas a “sample__xx.jpg”
2-	Se utilizó una App para Android llamada “Comica”, la cual realiza la conversión a estilo cómic. Se convierte imagen por imagen a través de mi teleléfono celular.
3-	Se normalizan los tamaños de las imagenes para que tanto input como target tengan la misma cantidad de datos.
4-  Se cuadriplicó el tamaño del dataset inviertiendo las imagenes en espejo, con más brillo y con menos brillo.
5-	Se suben a google drive las imágenes normales a la carpeta ‘Target’ y las convertidas a cómic a la carpeta ‘Input’

Se entrena el sistema con 200 épocas y se obtienen resultados bastante acertados.

Más descripción de la realización del proyecto en 

