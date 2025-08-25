# ✔ Proyecto AWS ✔

<img width="472" height="350" alt="image" src="https://github.com/user-attachments/assets/b6bbfe59-c9cf-4aa7-9004-7e018a05b36e" />

![Versión](https://img.shields.io/badge/versión-1.0-red)  
![Estado](https://img.shields.io/badge/estado-en%20prototipo-yellow)  
![Licencia](https://img.shields.io/badge/licencia-MIT-green)

> El proyecto busca desarrollar un sistema de basura inteligente que, mediante inteligencia artificial y cámaras, clasifique automáticamente los residuos en reutilizables,
> orgánicos y desechables. Su objetivo es mejorar la separación de desechos en la comunidad escolar de la ETITC, aumentando las oportunidades de reciclaje y reduciendo la
> contaminación ambiental.

> Se evaluará la precisión del sistema con la meta de alcanzar al menos un 30% de efectividad en tres meses, aplicando mejoras al algoritmo según los resultados.
> Este proyecto fomenta la conciencia ambiental y la participación de estudiantes y docentes en el cuidado del planeta.

---

## 🎯 Objetivo del Proyecto

Explica brevemente el propósito general: Desarrollar un sistema de basura inteligente que utilice inteligencia artificial y cámaras para clasificar automáticamente 
los desechos en 3 categorías: papel, orgánicos y plastico, con el propósito de mejorar la gestión de residuos y fomentar la cultura del reciclaje en el 
entorno escolar.

---

## 🧪 Prototipo

🔗 **[Ver prototipo funcional](https://tuprototipo.netlify.app)**  
📁 **[Ver prototipo en Figma](https://www.figma.com/file/...)**

### 📸 Registro fotografico 

| Diseño guia | Primer diseño de proyecto | Diseño final |
|--------------------|------------------|-------------|
|<img width="248" height="545" alt="image" src="https://github.com/user-attachments/assets/3596bbaa-7069-4da0-a7b5-26698745bf38" />| <img width="276" height="490" alt="image" src="https://github.com/user-attachments/assets/787625d2-3538-4829-b492-1ef7ce6efd3e" />| <img width="437" height="476" alt="image" src="https://github.com/user-attachments/assets/07e9cae7-7005-4398-880d-233b72bf073b" /> |

---

## 🧰 ¿Cómo funciona?

El proyecto combina software (IA con Teachable Machine y Python) con hardware (Arduino y servomotores):

Captura de imagen

Una cámara web toma una foto del objeto que el usuario quiere desechar.


Clasificación con IA

El modelo entrenado en Teachable Machine analiza la imagen.

Detecta si el residuo es plástico, vidrio, papel, orgánico, etc.



Comunicación con Arduino

Python interpreta la predicción del modelo.

Envía un comando al Arduino por el puerto serie (COM5 en este caso).


<img width="300" height="600" alt="image" src="https://github.com/user-attachments/assets/128feb0f-3301-42d3-8044-0266034c977b" />

Movimiento mecánico (los servos)

Servo 1: mueve un tubo o conducto para direccionar la basura al contenedor adecuado.

Servo 2: abre una compuerta para permitir que el residuo caiga en el lugar correcto.

Al terminar, el sistema regresa a la posición inicial, listo para el próximo objeto.


🛠️ Componentes principales

Software:

Teachable Machine (Google) → para entrenar el modelo de clasificación de imágenes.

Python (con TensorFlow y OpenCV) → para ejecutar el modelo en tiempo real.

Comunicación Serial → conecta Python con Arduino.

Hardware:

Arduino UNO (o compatible).

2 servomotores (uno para el tubo direccionador, otro para la compuerta).

Cámara web.

### Pasos
