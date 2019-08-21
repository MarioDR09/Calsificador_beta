# Calsificador_beta

Para construir una Mask R-CNN personalizada, nuevamente se utilizará el  repositorio Matterport Github . El último repositorio de detección de objetos TensorFlow también ofrece la opción de construir una Mask R-CNN. Sin embargo, las nuevas versiones de TensorFlow, detección de objetos, formato para máscara, etc. pueden exigir MUCHA depuración de errores; así que por ahora recomiendo encarecidamente el repositorio Matterport Mask R-CNN para esta versión del calsificador.

# Paso 1: Recolectando datos
En este caso, se udasron 105 imágenes del ines varias (90 entrenamiento y 15 validación). 

# Paso 2: Anotar los datos
Un modelo de máscara R-CNN requiere que el usuario anote las imágenes e identifique la región del daño. La herramienta de anotación que utilicé es el Anotador de imágenes VGG - v 1.0.6. Puede usar la versión html disponible en este  enlace . Con esta herramienta, puede crear una máscara de polígono como se muestra a continuación:

Una vez que haya creado todas las anotaciones, puede descargar la anotación y guardarla en formato json . Puede ver mis imágenes y anotaciones en mi repositorio aquí .

# Paso 3: Entrenando un modelo
Se inicia clonando el repositorio 'Matterport Mask R-CNN':  https://github.com/matterport/Mask_RCNN .

A continuación, cargaremos nuestras imágenes y anotaciones.
