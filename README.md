# Predicción de Peso de peces y Tamaño de Plantas en Acuaponía mediante Inteligencia Artificial

Este proyecto es un estudio comparativo que aplica y evalúa diferentes modelos de inteligencia artificial para predecir el crecimiento de peces (peso) y plantas (tamaño) en sistemas acuapónicos. El objetivo es analizar el rendimiento de cada modelo utilizando datos de sensores de calidad del agua y variables de cultivo.

## 📜 Descripción

La motivación principal de este proyecto es explorar cómo la Inteligencia Artificial puede ser aplicada a la agricultura sostenible para optimizar la producción de alimentos. Al predecir con precisión la biomasa, es posible mejorar la gestión de recursos, anticipar cosechas y aumentar la eficiencia general de los sistemas acuapónicos.

**Dataset Principal:** El análisis inicial se basa en el dataset público [Sensor-Based Aquaponics Fish Pond Datasets](https://www.kaggle.com/datasets/ogbuokiriblessing/sensor-based-aquaponics-fish-pond-datasets), que monitorea el crecimiento de Bagre (Catfish). A futuro, se planea incorporar otros datasets para enriquecer el estudio.

---

## 🛠️ Estructura del Proyecto

El repositorio está organizado para separar la lógica, los datos y los resultados, promoviendo la reutilización de código y la claridad.

* **/data:** Contiene los datasets limpios y combinados, listos para ser usados por los modelos.
* **/results:** Almacena las gráficas (curvas de aprendizaje, comparativas, etc.) y métricas generadas por cada experimento.
* **/src:** Contiene todo el código fuente de Python, modularizado para su fácil mantenimiento.
    * `data_processing.py`: Scripts para la limpieza y preparación de datos.
    * `models.py`: Definiciones de las arquitecturas de los diferentes modelos.
    * `evaluation.py`: Funciones para evaluar los modelos y generar visualizaciones.
    * `train.py`: Script principal para orquestar el entrenamiento y la evaluación.

---

## 🚀 Cómo Empezar

Sigue estos pasos para ejecutar el proyecto en tu máquina local.

### Prerrequisitos

* Python 3.9 o superior
* Git

### Instalación

1.  **Clona el repositorio:**
    ```bash
    git clone https://github.com/FredyZarate11/ACUAPONIA_IA
    cd ACUAPONIA_IA
    ```

2.  **Crea y activa un entorno virtual:**
    ```bash
    # Crear el entorno
    python -m venv .venv

    # Activar en Windows
    .\.venv\Scripts\activate

    # Activar en macOS/Linux
    source .venv/bin/activate
    ```

3.  **Instala las dependencias:**
    ```bash
    pip install -r requirements.txt
    ```

### Uso

Para entrenar los modelos definidos y ver los resultados, ejecuta el script principal desde la carpeta raíz del proyecto:

```bash
python src/train.py
```

El script cargará los datos, entrenará los modelos y generará las métricas de rendimiento y las gráficas de evaluación.

-----

## 📊 Resultados y Experimentos

A continuación se resumen los resultados de los diferentes modelos probados. El objetivo era minimizar el error de predicción del peso de los peces.

| Modelo Probado | RMSE (g) | MAE (g) | $$R^{2}$$ | Error Relativo (%) | Observaciones y Detalles |
| :--- | :---: | :---: | :---: | :---: | :--- |
| **ANN (Red Neuronal Artificial)** | 26.3791 | 19.4693 | 0.9589 | 10.0333 | El crecimiento no es lineal, por lo que no es bueno para predecir.
| **DNN (Red Neuronal Profunda)** | ** | ** | ** | ** | 
| **KNN (K-Nearest Neighbors)** |  ** | ** | ** | ** |
| **RNN (Red Neuronal Recurrente)**|  ** |  ** | ** | ** |
| **ANFIS** |  ** | ** | ** | ** |
| **SVR (Support Vector Regression)**| ** | ** | ** | ** |
| **K-MEANS** |  ** | ** | ** | ** |

### Conclusiones del Estudio

*[Esta sección se llenará una vez que los experimentos hayan concluido. Aquí se analizará qué modelos funcionaron mejor y bajo qué condiciones, proporcionando una recomendación final sobre el enfoque más adecuado para esta problemática.]*

-----

## 👤 Autor

  * **Fredy Alejandro Zárate Abril**
  * **Email:** ing.fredyzarate@outlook.com
  * **GitHub:** [@ThissFredy](https://github.com/ThissFredy) ---

## 📄 Licencia

Este proyecto está bajo la Licencia MIT.

