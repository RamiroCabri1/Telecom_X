# Análisis Exploratorio de Datos de Clientes de Telecomunicaciones 

Este repositorio contiene un análisis exploratorio de datos (EDA) centrado en la comprensión de las características de los clientes de una empresa de telecomunicaciones. El objetivo principal es preparar y explorar el dataset para identificar patrones, detectar anomalías y asegurar la calidad de los datos para futuros análisis o modelos predictivos.

## Contenido del Proyecto

El proyecto se desarrolla en un notebook de Google Colab, estructurado para guiar a través de los siguientes pasos:

1.  **Carga e Inspección Inicial de Datos**: Carga del dataset y una primera revisión de su estructura, tipos de datos y presencia de valores nulos.
2.  **Preprocesamiento y Limpieza de Datos**:
    * Identificación y tratamiento de valores nulos, específicamente en la columna `Charges_Total`, donde los nulos se imputaron con `0` (cero) bajo la hipótesis de que corresponden a clientes recién incorporados sin cargos acumulados.
    * Preparación de variables para visualización.
3.  **Exploración de Outliers en Variables Numéricas**:
    * Utilización de **Boxplots** para visualizar la distribución de las principales variables numéricas (`Charges_Monthly`, `tenure`, `Charges_Total`, `Cuentas_Diarias`) y detectar posibles valores atípicos.
    * Análisis detallado de la distribución de `Charges_Total`, confirmando su concentración en cero debido a la alta proporción de clientes nuevos (`tenure` baja o nula).
4.  **Análisis de Distribuciones**:
    * Creación de un **Histograma** para `Charges_Total` para comprender mejor la naturaleza de su distribución y la frecuencia de los valores cero, complementando la información obtenida del boxplot.

## Tecnologías Utilizadas

* **Python**: Lenguaje de programación principal.
* **Pandas**: Para la manipulación y análisis de datos.
* **Matplotlib**: Para la creación de visualizaciones estáticas.
* **Seaborn**: Basado en Matplotlib, utilizado para crear gráficos estadísticos más atractivos e informativos.
* **NumPy**: Para operaciones numéricas eficientes.
* **Google Colab**: Entorno de desarrollo para la ejecución del notebook.

## Cómo Usar

1.  **Clonar el Repositorio**:
    ```bash
    git clone [https://github.com/TuUsuario/NombreDeTuRepositorio.git](https://github.com/TuUsuario/NombreDeTuRepositorio.git)
    cd NombreDeTuRepositorio
    ```
2.  **Abrir en Google Colab**:
    * Sube el archivo `.ipynb` a tu Google Drive.
    * Ábrelo con Google Colab.
    * Asegúrate de que el dataset (`df_telecomX`) esté disponible y correctamente cargado en el entorno de Colab (ya sea subiéndolo directamente o conectándolo desde Google Drive).
3.  **Ejecutar las Celdas**: Simplemente ejecuta las celdas del notebook en orden para replicar el análisis.

## Resultados y Perspectivas Clave

* Se confirmó la necesidad de tratar los nulos en `Charges_Total`, siendo la imputación con `0` la más adecuada dada la naturaleza de la variable.
* Los boxplots revelaron las distribuciones de `Charges_Monthly` y `tenure` sin *outliers* significativos, mostrando un rango amplio de antigüedad y cargos mensuales.
* La variable `Charges_Total` mostró una particularidad en su distribución, con una gran concentración de valores en cero, lo que fue validado mediante un histograma, sugiriendo una alta proporción de clientes recién llegados.
* Este EDA sienta las bases para futuras fases del proyecto, como la ingeniería de características y el desarrollo de modelos predictivos, considerando las características y particularidades de cada variable.

---

**Autor:** Cabri Ramiro Hernan



---
