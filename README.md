# Análisis de las pruebas Saber Pro

## 📖 Resumen
\begin{abstract}

\noindent En este proyecto se aplican métodos matemáticos y estadísticos del área de ciencia de datos para analizar el rendimiento de los estudiantes de Matemáticas y Ciencias Naturales que presentaron las pruebas \textbf{Saber Pro} genéricas y específicas entre 2016 y 2024. Con información oficial de DataIcfes \cite{ICFESData}, se estudiará el desempeño en competencias de las 8 áreas de conocimiento y sus 56 núcleos, poniendo especial énfasis en Matemáticas y Ciencias Naturales, nuestro grupo de mayor interés. El objetivo es identificar patrones de rendimiento y realizar comparaciones socioacadémicas con estudiantes de otras áreas, aportando así una visión más clara sobre la formación matemática y científica en el contexto nacional.\\


{\setlength{\parindent}{0pt}
El estudio implementa un flujo de trabajo analítico secuencial que inicia con la caracterización exploratoria de los datos mediante estadísticas descriptivas y visualización, centrándose en la distribución de puntajes por área de conocimiento y las relaciones entre competencias genéricas y específicas, incluyendo tratamiento de valores atípicos, limpieza y estandarización de categorías. Posteriormente, se aplicó Análisis de Correspondencias Múltiples a variables categóricas clave para identificar dimensiones latentes que explican asociaciones socioacadémicas, seguido de clustering sobre las coordenadas factoriales para definir perfiles estudiantiles naturales. En la tercera fase, se implementó Análisis de Componentes Principales sobre los puntajes de competencias, revelando patrones subyacentes de habilidad académica. Estos resultados alimentaron modelos de regresión lineal múltiple que incorporaron los perfiles identificados para cuantificar efectos sobre el desempeño académico, finalizando con la validación robusta mediante métodos de Bootstrap para garantizar la confiabilidad de las inferencias en núcleos de conocimiento con muestras reducidas.

\vspace{10pt} 
Para el desarrollo del proyecto se emplean las siguientes librerías: pandas y numpy para manipulación y limpieza de datos; matplotlib y seaborn para visualizaciones exploratorias; prince para la implementación del Análisis de Correspondencias Múltiples; scikit-learn para la ejecución de PCA, algoritmos de clustering K-Means y métodos de Bootstrap; y statsmodels para la implementación de modelos de regresión lineal múltiple y análisis de inferencia estadística, garantizando así un entorno analítico integral y reproducible.\\



\noindent\textbf{Palabras Clave:} Análisis de Correspondencias Múltiples, Análisis Multivariado, Análisis de Componentes Principales, Regresión lineal múltiple, Modelación Predictiva.\\

Este trabajo ha sido realizado en colaboración con \textbf{Eddy Santiago Vargas Fajardo}, a quien agradecemos su apoyo y contribución en el desarrollo del mismo.


\begin{thebibliography}{9}
\bibitem[1]{ICFESData}
ICFES, “Data ICFES – repositorio de datos de ICFES”, actualizado 26 de junio de 2025, sitiodeweb: \url{https://www.icfes.gov.co/investigaciones/data-icfes/}.
\bibitem[2]{kroese2024} {\sc Dirk P. Kroese, Zdravko I. Botev, Thomas Taimre y Radislav Vaisman}, {\it Data Science and Machine Learning: Mathematical and Statistical Methods}. Chapman and Hall/CRC, \textbf{2024}.
\bibitem[3]{pandasdocs} {\sc The pandas Development Team}, {\it pandas documentation}. \textbf{2024}. Disponible en: https://pandas.pydata.org/docs/
\bibitem[4]{MichaelGreenacre} {\sc Michael Greenacre}, {Correspondence Analysis in Practice. Third Edition}. 
\bibitem[5]{Freund} {\sc Freund}, {Estadística Matemática con Aplicaciones}. 
\bibitem[6]{Mood} {\sc Mood}, {Introduction to the Theory of Statistics}. 

\end{thebibliography}

---
