# Análisis de las pruebas Saber Pro

## 🚀 Link de ejecución rápida para el código base de limpieza y preparación de los datos por año documentado:
https://colab.research.google.com/drive/1AIe4LdyoFVHYP9tte5asQlRz2xHsQcRn?usp=sharing
 *(para visualizar y ejecutar los códigos)*

- `Filtracion_Pruebas_Saber_Pro.ipynb` archivo .ipynb del proyecto

Importante descargar los datos `areasynucleos_sirveparafiltrar` que se encuentran en la carpeta `Data_Preparation`, también debe descargar los datos de las pruebas específicas y genéricas que se encuentran en la siguiente carpeta de Drive:

https://drive.google.com/drive/folders/1kRGfHPoHS0XW2EgKuTLKB8im2Rb9yXnE?usp=sharing

Los archivos se utilizan en el código de filtración.


## 📖 Resumen
En este proyecto se aplican métodos matemáticos y estadísticos del área de ciencia de datos para analizar el rendimiento de los estudiantes de Matemáticas y Ciencias Naturales que presentaron las pruebas Saber Pro genéricas y específicas entre 2016 y 2024. Con información oficial de DataIcfes ICFESData, se estudiará el desempeño en competencias de las 8 áreas de conocimiento y sus 56 núcleos, poniendo especial énfasis en Matemáticas y Ciencias Naturales, nuestro grupo de mayor interés. El objetivo es identificar patrones de rendimiento y realizar comparaciones socioacadémicas con estudiantes de otras áreas, aportando así una visión más clara sobre la formación matemática y científica en el contexto nacional.


El estudio implementa un flujo de trabajo analítico secuencial que inicia con la caracterización exploratoria de los datos mediante estadísticas descriptivas y visualización, centrándose en la distribución de puntajes por área de conocimiento y las relaciones entre competencias genéricas y específicas, incluyendo tratamiento de valores atípicos, limpieza y estandarización de categorías. Posteriormente, se aplicó Análisis de Correspondencias Múltiples a variables categóricas clave para identificar dimensiones latentes que explican asociaciones socioacadémicas, seguido de clustering sobre las coordenadas factoriales para definir perfiles estudiantiles naturales. En la tercera fase, se implementó Análisis de Componentes Principales sobre los puntajes de competencias, revelando patrones subyacentes de habilidad académica. Estos resultados alimentaron modelos de regresión lineal múltiple que incorporaron los perfiles identificados para cuantificar efectos sobre el desempeño académico, finalizando con la validación robusta mediante métodos de Bootstrap para garantizar la confiabilidad de las inferencias en núcleos de conocimiento con muestras reducidas.

Para el desarrollo del proyecto se emplean las siguientes librerías: pandas y numpy para manipulación y limpieza de datos; matplotlib y seaborn para visualizaciones exploratorias; prince para la implementación del Análisis de Correspondencias Múltiples; scikit-learn para la ejecución de PCA, algoritmos de clustering K-Means y métodos de Bootstrap; y statsmodels para la implementación de modelos de regresión lineal múltiple y análisis de inferencia estadística, garantizando así un entorno analítico integral y reproducible.



Palabras Clave: Análisis de Correspondencias Múltiples, Análisis Multivariado, Análisis de Componentes Principales, Regresión lineal múltiple, Modelación Predictiva.

---




