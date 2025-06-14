🎮 Detector de Videojuegos por Imagen
📌 Descripción General
Este proyecto consiste en un programa desarrollado en Python que, mediante el uso de clases y un modelo de aprendizaje automático entrenado en Teachable Machine, permite identificar el nombre de un videojuego a partir de una imagen. Solo es compatible con una lista definida de videojuegos previamente entrenados.

❓ Problema que resuelve
A veces vemos un videojuego en redes sociales, videos o páginas web, pero no sabemos su nombre. Este programa soluciona ese problema: simplemente toma una captura de pantalla o una foto del juego, y el programa te dirá cuál es, siempre que esté entre los juegos reconocidos por el modelo.

🔍 Detalles del funcionamiento
Se utiliza la herramienta Teachable Machine de Google para entrenar un modelo de clasificación de imágenes con ejemplos de videojuegos.

El modelo puede identificar la imagen con una probabilidad y devolver el nombre del juego más probable.

El modelo se exporta y se integra en un entorno de desarrollo en Visual Studio Code, donde se conecta con un programa en Python.

En Python, se procesa la imagen, se pasa al modelo, y se interpreta la respuesta para mostrar el nombre del juego detectado.

🧱 Estructura del proyecto

Videojuego-Detector/
│
├── model/                  # Carpeta con el modelo exportado de Teachable Machine
│   ├── model.json
│   └── weights.bin
│
├── images/                 # Imágenes de prueba para detección
│   ├── ejemplo1.jpg
│   └── ejemplo2.jpg
│
├── src/                    # Código fuente en Python
│   ├── main.py             # Script principal que carga el modelo y ejecuta la predicción
│   └── utils.py            # Funciones auxiliares para procesamiento de imagen
│
├── requirements.txt        # Librerías necesarias para ejecutar el programa
└── README.md               # Este archivo
