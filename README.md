# FacialRecognition

Reconocimiento de Emociones

Este proyecto reconoce emociones usando la cámara de la computadora.
Funciona en tres pasos que son la captura, entrenamiento y reconocimiento.

1. Captura de datos
Este paso toma fotos del rostro para crear la base de datos.

¿Qué hace el programa?
Enciende la cámara.
Detecta tu rostro con Haar Cascade.
Recorta solo la cara.
Guarda muchas imágenes dentro de una carpeta con el nombre de la emoción (Felicidad, Tristeza, Enojo, Sorpresa).

2. Entrenamiento del modelo
Esta parte enseña al programa a reconocer emociones usando las fotos guardadas.

¿Qué hace?
Lee todas las imágenes de cada emoción.
Les asigna una etiqueta (0, 1, 2, 3).
Entrena tres modelos:
EigenFaces
FisherFaces
LBPH
Guarda los modelos entrenados en archivos XML.

3. Reconocimiento en tiempo real
Donde se muestra el reconocimiento.

¿Qué hace?
Activa la cámara.
Detecta tu rostro.
Lo compara con lo aprendido en el entrenamiento.
Muestra en pantalla qué emoción reconoce, por ejemplo:
Feliz, Triste, Enojado, Sorprendido.

Ejemplo:












![Image](https://github.com/user-attachments/assets/96465881-8796-4bf5-95e0-fad61aba70b9)

Instalaciones necesarias:
pip install opencv-contrib-python numpy imutils

