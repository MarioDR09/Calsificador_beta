# Calsificador_beta

Para construir una Mask R-CNN personalizada, nuevamente se utilizará el  repositorio Matterport Github . El último repositorio de detección de objetos TensorFlow también ofrece la opción de construir una Mask R-CNN. Sin embargo, las nuevas versiones de TensorFlow, detección de objetos, formato para máscara, etc. pueden exigir MUCHA depuración de errores; así que por ahora recomiendo encarecidamente el repositorio Matterport Mask R-CNN para esta versión del calsificador.

# Paso 1: Recolectando datos
En este caso, se usaron 105 imágenes del ines varias (90 entrenamiento y 15 validación). 

# Paso 2: Anotar los datos
Un modelo de máscara R-CNN requiere que el usuario anote las imágenes e identifique la región de interés. La herramienta de anotación que se usó es el Anotador de imágenes VGG - v 1.0.6. La versión html disponible en: http://www.robots.ox.ac.uk/~vgg/software/via/ Con esta herramienta, se puede crear un polígono como máscara.

Una vez que haya creado todas las anotaciones, se procede a descargar la anotación y guardarla en formato json. (No subiré las imágenes ni anotaciones para evitar complicaciones..legaes)

# Paso 3: Entrenando un modelo
Se inicia clonando el repositorio 'Matterport Mask R-CNN':  https://github.com/matterport/Mask_RCNN .

A continuación, cargaremos nuestras imágenes y anotaciones en el archivo custom.py:



