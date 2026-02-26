# Escenario Procedural 3D: Animación y Geometría en Blender

## 📝 Descripción del Proyecto

Este proyecto consiste en la generación procedural de un escenario 3D automatizado mediante Python y la API de Blender (`bpy`). Como parte de la materia de **Graficación** (4to Semestre de Ingeniería en Sistemas), se implementó un sistema que construye un pasillo con tramos rectos y curvos, aplicando transformaciones lineales y modelos de iluminación dinámica.

El objetivo principal es demostrar la importancia de la gestión de objetos en memoria y la automatización de procesos geométricos.

---

## 🛠️ Fundamentos de Graficación Aplicados

### 1. Modelos de Color (Tema 1.4)

Se utilizó el **modelo RGB** para la definición de materiales. A través de una función orientada a objetos, se crearon materiales dinámicos para los polígonos del escenario:

* 
**Material Base**: Un tono gris oscuro para elementos estructurales.


* 
**Material de Acento**: Un color neón (naranja rojizo) para resaltar detalles visuales y la alternancia de patrones.



### 2. Transformaciones Tridimensionales (Tema 3.3)

La construcción del escenario se basa en el cálculo de matrices de transformación aplicadas mediante scripting:

* 
**Traslación (3.3.1)**: Ubicación precisa de cubos en los ejes X, Y y Z para formar el pasillo lineal.


* 
**Escalamiento (3.3.2)**: Modificación de las dimensiones de los bloques para generar variedad visual y definir la superficie del suelo.


* 
**Rotación**: Implementada en el tramo curvo para que los objetos se orienten de forma tangencial a la trayectoria.



### 3. Geometría Procedural y Trigonometría

A diferencia de un modelado manual, el tramo curvo se generó utilizando algoritmos matemáticos:

* **Funciones Trigonométricas**: Uso de Seno ($sin$) y Coseno ($cos$) para determinar la posición de los bloques en un arco circular.
* 
**Ciclos de Iteración**: Automatización de la geometría para optimizar el código y evitar la repetición manual de tareas.



---

## 🎥 Animación y Recorrido Virtual

El proyecto incluye un recorrido de cámara animado de **250 fotogramas** configurado directamente desde el script:

* **Trayectoria Híbrida**: Transición fluida entre un movimiento rectilíneo y uno circular.
* **Interpolación Lineal**: Se forzó la interpolación de los "Keyframes" a tipo **Linear** para evitar tirones y asegurar un movimiento constante.
* **Simulación Humana**: Altura de cámara fijada en $Z=1.5$ para simular la perspectiva de un personaje en primera persona.

---

## 🚀 Cómo Ejecutar el Proyecto

1. Descarga el archivo `Import.py` de este repositorio.
2. Abre **Blender** (Versión 3.0 o superior).
3. Dirígete al espacio de trabajo de **Scripting**.
4. Haz clic en `Open` y selecciona el archivo `.py`.
5. Pulsa el botón **Run Script**.

### Renderizado de Video

El script ya viene configurado para exportar un video en formato **MP4 (H.264)**. Para generarlo:

* Presiona `Ctrl + F12`.
* El video se guardará automáticamente en la carpeta de tu proyecto con el nombre `escenario_final.mp4`.

---

## 📂 Estructura del Repositorio

* `/scripts`: Código fuente en Python (`.py`).
* `/renders`: Video de demostración y capturas de pantalla.
* `/docs`: Documentación adicional y PDF de la práctica.

---

## 👨‍💻 Autor

**Plascencia Mora David Emiliano**
*Materia: Graficación, 4to Semestre.*
---
## 🖼️ Resultado Visual
<img width="562" height="341" alt="image" src="https://github.com/user-attachments/assets/4a419115-2cce-49c3-9304-10a2912ff4cf" />
