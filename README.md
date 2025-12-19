# Identificando Perfiles de Éxito Académico en Colombia con Machine Learning 📊🧮🔬

## 📖 Descripción  
En este estudio, analicé los resultados de las pruebas Saber Pro (2016-2024) de los estudiantes a nivel nacional y de Matemáticas y Ciencias Naturales por separado. Utilizando técnicas Machine Learning como PCA (Principal Component Analysis), MCA (Multiple Correspondence Analysis) y Clustering (K-Means), donde se identificaron cuatro perfiles estudiantiles distintos, demostrando que el "éxito académico" no es uniforme y está fuertemente influenciado por contextos socioeconómicos, generacionales y de desigualdades estructurales. El objetivo es aportar una visión más detallada para el diseño de políticas educativas en el país.

---

## 🚀 Ejecución Rápida  
Código de las gráficas descriptivas:
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1wauMUdRgnjvel9Hyuc8ClFqEPCK2NRJe?usp=drive_link) *(el código todavía no se encuentra documentado, se subira bien documentado el 20 de Diciembre)*


Puedes visualizar el documento PDF de las gráficas creadas aquí (De los algoritmos de ML solo tiene la gráfica del PCA, el día 20 de Diciembre se actualizará a su versión final con la página web del MCA): 

[![Abrir PDF](https://img.shields.io/badge/Abrir_PDF-4285F4?style=for-the-badge&logo=googledrive&logoColor=white&labelColor=4285F4&color=34A853)](https://drive.google.com/file/d/1N_lYwoT3htiYPBG9J1wVts9eYAcOV5eY/view?usp=drive_link)

- `pandas`, `numpy` para manipulación de datos  
- `scikit-learn` para PCA, K-Means y modelos de regresión  
- `matplotlib`, `seaborn` para visualización  
- `prince`,  para análisis de correspondencias múltiples

---
## 📊 Resultados destacados  

El análisis de 2.2 millones de registros reveló hallazgos clave sobre el desempeño académico a nivel nacional a lo largo de estos últimos nueve años:

- **Cuatro perfiles estudiantiles identificados:**  
  - *Cluster 0*: Estudiantes Promedio (37.6%), rendimiento medio, nivel socioeconómico bajo-medio.  
  - *Cluster 1*: Estudiantes en Desventaja Académica (28.7%), menor rendimiento y estrato bajo.  
  - *Cluster 2*: Estudiantes Adultos (12.9%), mayor edad, bajo índice socioeconómico.  
  - *Cluster 3*: Estudiantes de Alto Rendimiento (20.8%), excelente desempeño, estrato medio-alto.  

- **El 66.3% de los estudiantes** se ubican en clusters de rendimiento medio o bajo, evidenciando desigualdades socioacadémicas significativas.

- **Brecha en inglés de 61.3 puntos** entre los extremos de rendimiento, reflejando disparidades en competencias lingüísticas.

- **Paridad de género en habilidad académica**, aunque persiste segregación en la elección de disciplinas (menor presencia femenina en Física/Matemáticas).

- **Programas aplicados** (Ciencias de la Computación, Ciencia de Datos) superan en rendimiento a Matemáticas puras en pruebas específicas.

- **Disparidades regionales marcadas:** Bogotá y Santander lideran en desempeño, mientras departamentos como Atlántico y Boyacá presentan promedios bajos.

---

## 🧠 Habilidades demostradas  

| Área | Competencias demostradas |
|------|---------------------------|
| **Manipulación de datos** | Limpieza, unión y clasificación de bases con `pandas` y `numpy` |
| **Machine Learning** | Clustering con **K-Means**, análisis multivariado con **MCA** y **PCA** |
| **Visualización** | Gráficos exploratorios con `matplotlib` y `seaborn` |
| **Interpretación estadística** | Identificación de patrones, correlaciones y perfiles latentes |
| **Comunicación científica** | Presentación estructurada de hallazgos en contexto educativo |

---

## 📈 Visualizaciones incluidas   

- Gráficos de componentes principales (PCA) y de correspondencias múltiples (MCA) 
- Distribución de clusters K-Means
- Comparativas de rendimiento por módulo y perfil  
- Mapas de densidad de correlaciones socioacadémicas  
- Diagramas de barras por núcleo de conocimiento 
- Visualizaciones de desempeño regional e institucional  

---

## 📚 Fuentes de datos  

- [**ICFES - DataIcfes (2016–2024)**](https://www.icfes.gov.co/investigaciones/data-icfes/)  
  Datos oficiales de pruebas Saber Pro, incluyendo puntajes genéricos, específicos y variables sociodemográficas.

- **Referencias metodológicas:**  
  - Greenacre, M. *Correspondence Analysis in Practice*  
  - Kroese et al. *Data Science and Machine Learning: Mathematical and Statistical Methods*  
  - Documentación de `pandas`, `numpy`, `scikit-learn`, `seaborn`, `matplotlib`, `prince`, etc...

---

## 👤 Autor

**Juan Pablo Gómez Morales**  


📍 Bogotá, Colombia  
📧 *Contacto: [prxvxjpg@gmail.com]*  

💡 *Proyecto presentado en el XIII Simposio Nororiental de Matemáticas (2025).*

---

## ⭐ Cómo citar  

> Juan Gómez (2025). *Rompiendo el Molde: Identificando los Diversos Perfiles de Éxito Académico en Colombia con Machine Learning*. Universidad Distrital Francisco José de Caldas, Bogotá, Colombia.

