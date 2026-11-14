# VISION LAB — Actividad de Visión Computacional (SENATI)

Proyecto con **un único cuaderno Jupyter documentado** y **una actividad web interactiva**.

- [Abrir el cuaderno Jupyter](CUADERNO_PROYECTO_VISION_COMPUTACIONAL.ipynb)
- [Ver código de la actividad web](index.html)

## Contenido
El cuaderno presenta objetivos, lectura y dimensiones de una imagen, color BGR, escala de grises, filtro Gauss 5×5, Canny 50/150 y 100/200, rotaciones 15° y 30°, redimensionado, retos por módulos, seis imágenes procesadas y preguntas de reflexión respondidas.

La página web ofrece un laboratorio que permite subir una imagen, aplicar filtros en el navegador y guardar PNG, junto con una evaluación de **20 preguntas de opción múltiple** con calificación y explicaciones.

**Nota técnica:** el laboratorio web usa Canvas (detección de bordes aproximada); el cuaderno utiliza OpenCV y el algoritmo Canny real.

## Ejecutar Jupyter
```bash
pip install opencv-python numpy matplotlib pillow
jupyter notebook CUADERNO_PROYECTO_VISION_COMPUTACIONAL.ipynb
```
Coloca `imagen_practica.png` en la carpeta `recursos` si quieres usar la imagen del material docente; el cuaderno también crea una imagen ilustrativa si falta el archivo.

## Desplegar la web en Render
Servicio web de Python, rama `main`. Comando de compilación: `echo ready`. Comando de arranque: `python -m http.server $PORT --bind 0.0.0.0`.
La aplicación web es estática y no necesita instalar OpenCV en el servidor.