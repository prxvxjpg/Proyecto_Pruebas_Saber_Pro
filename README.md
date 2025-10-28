# Análisis de las pruebas Saber Pro

## 📖 Resumen
En este proyecto se aplican m´etodos matem´aticos y estad´ısticos del ´area de ciencia de
datos para analizar el rendimiento de los estudiantes de Matem´aticas y Ciencias Naturales
que presentaron las pruebas Saber Pro gen´ericas y espec´ıficas entre 2016 y 2024.
Con informaci´on oficial de DataIcfes [1], se estudiar´a el desempe˜no en competencias de
las 8 ´areas de conocimiento y sus 56 n´ucleos, poniendo especial ´enfasis en Matem´aticas
y Ciencias Naturales, nuestro grupo de mayor inter´es. El objetivo es identificar patrones
de rendimiento y realizar comparaciones socioacad´emicas con estudiantes de otras
´areas, aportando as´ı una visi´on m´as clara sobre la formaci´on matem´atica y cient´ıfica
en el contexto nacional.
El estudio implementa un flujo de trabajo anal´ıtico secuencial que inicia con la caracterizaci
´on exploratoria de los datos mediante estad´ısticas descriptivas y visualizaci´on,
centr´andose en la distribuci´on de puntajes por ´area de conocimiento y las relaciones
entre competencias gen´ericas y espec´ıficas, incluyendo tratamiento de valores at´ıpicos,
limpieza y estandarizaci´on de categor´ıas. Posteriormente, se aplic´o An´alisis de Correspondencias
M´ultiples a variables categ´oricas clave para identificar dimensiones latentes
que explican asociaciones socioacad´emicas, seguido de clustering sobre las coordenadas
factoriales para definir perfiles estudiantiles naturales. En la tercera fase, se implement´o
An´alisis de Componentes Principales sobre los puntajes de competencias, revelando
patrones subyacentes de habilidad acad´emica. Estos resultados alimentaron modelos
de regresi´on lineal m´ultiple que incorporaron los perfiles identificados para cuantificar
efectos sobre el desempe˜no acad´emico, finalizando con la validaci´on robusta mediante
m´etodos de Bootstrap para garantizar la confiabilidad de las inferencias en n´ucleos de
conocimiento con muestras reducidas.
Para el desarrollo del proyecto se emplean las siguientes librer´ıas: pandas y numpy
para manipulaci´on y limpieza de datos; matplotlib y seaborn para visualizaciones exploratorias;
prince para la implementaci´on del An´alisis de Correspondencias M´ultiples;
scikit-learn para la ejecuci´on de PCA, algoritmos de clustering K-Means y m´etodos de
Bootstrap; y statsmodels para la implementaci´on de modelos de regresi´on lineal m´ultiple
y an´alisis de inferencia estad´ıstica, garantizando as´ı un entorno anal´ıtico integral y
reproducible.
Palabras Clave: An´alisis de Correspondencias M´ultiples, An´alisisMultivariado, An´alisis
de Componentes Principales, Regresi´on lineal m´ultiple, Modelaci´on Predictiva.

---
