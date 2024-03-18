# Análisis de Pulsos MPPC y PMT a partir de Datos de Osciloscopio Tektronix MSO44

Este repositorio contiene scripts en Python para el análisis de señales capturadas con el osciloscopio Tektronix MSO44, específicamente diseñados para trabajar con datos de detectores MPPC (Multi-Pixel Photon Counter) y PMT (Photomultiplier Tube). Los datos de entrada se esperan en formato CSV, donde la primera columna representa el tiempo y las columnas subsiguientes representan los canales del osciloscopio, con cada fila indicando un valor de voltaje.

## Contexto del Análisis

Los scripts implementan una serie de pasos para procesar y analizar los datos del osciloscopio, buscando identificar patrones, evaluar la relación entre las señales de diferentes canales, y cuantificar características fundamentales de los pulsos detectados. Este proceso incluye:

1. **Extracción y Visualización de Datos**: Lectura de archivos CSV y visualización inicial de los pulsos.
2. **Filtrado y Procesamiento de Señales**: Aplicación de umbrales y otras técnicas de filtrado para seleccionar pulsos de interés.
3. **Análisis Cuantitativo**: Cálculo de integrales de los pulsos para estimar energías y otras propiedades.
4. **Modelado y Sustracción de Fondo**: Ajuste de curvas para eliminar el ruido de fondo y mejorar la detección de señales.
5. **Comparación y Correlación**: Evaluación de la relación entre señales de MPPC y PMT y otros análisis comparativos.

## Estructura del Repositorio

- `src/`: Scripts de Python para el análisis.
- `data/`: Datos en formato CSV generados por el osciloscopio Tektronix MSO44.
- `docs/`: Documentación adicional y notas metodológicas.
- `results/`: Gráficas y datos resultantes del análisis.

## Requisitos

Este análisis requiere Python 3.X y las siguientes librerías:

- Numpy
- Matplotlib
- SciPy
- Uproot (opcional, para manejo de archivos ROOT en análisis relacionados)



