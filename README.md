# Identificando Perfiles de Éxito Académico en Colombia con Machine Learning 📊🔬

## 📖 Descripción  
En este estudio, analicé los resultados de las pruebas Saber Pro (2016-2024) de los estudiantes a nivel nacional y de Matemáticas y Ciencias Naturales por separado. Utilizando técnicas Machine Learning como PCA (Principal Component Analysis), MCA (Multiple Correspondence Analysis) y Clustering (K-Means), donde se identificaron cuatro perfiles estudiantiles distintos, demostrando que el "éxito académico" no es uniforme y está fuertemente influenciado por contextos socioeconómicos, generacionales y de desigualdades estructurales. El objetivo es aportar una visión más detallada para el diseño de políticas educativas en el país.

---

## 🚀 Ejecución Rápida  
Código de las gráficas descriptivas:
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1u2yell027euCiwvkOboGbsfQM-DD9BrK?authuser=1&usp=drive_open)

Código del algoritmo de Machine Learning PCA y K-Means:
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1LXBCwLxjGMZb7gqufWuxz7n9gVswOAuC?usp=drive_link) *(código con gráfica del PCA junto con K-Means interactivo)*

Código del algoritmo de Machine Learning MCA:
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ecIRZXfV1vBWAAVi4wCKA6mxR68XfIo1?authuser=1) *(código con gráficas interactivas de MCA, para visualizarlas es importante descargarlo y correrlo en vscode junto con los datos `Pruebas_Genericas_2016-2024_SaberPro.csv` limpios que se encuentran en el drive de abajo)*

Puedes visualizar el documento PDF de las gráficas creadas aquí: 
[![Abrir PDF](https://img.shields.io/badge/Abrir_PDF-4285F4?style=for-the-badge&logo=googledrive&logoColor=white&labelColor=4285F4&color=34A853)](https://drive.google.com/file/d/1npoOE4lJssVwxEa9dKnMRV8pCJpSEXl8/view?usp=drive_link)



- `pandas`, `numpy` para manipulación de datos  
- `scikit-learn` para PCA, K-Means y modelos de regresión  
- `matplotlib`, `seaborn` para visualización  
- `prince`,  para análisis de correspondencias múltiples

---
## 📊 Resultados destacados del PCA & K-Means

El análisis de 2.2 millones de registros reveló hallazgos clave sobre el desempeño académico a nivel nacional a lo largo de estos últimos nueve años:


El análisis de varianza explicada confirma que **PC1 es el componente más importante (46.3%)**, seguido por **PC2 (14.7%)** y **PC3 (11.2%)**, representando colectivamente el **72.2%** de la varianza total (es decir que en una sola gráfica de tres dimensiones se encuentra el 72.2% de la información de los 2.2 millones de datos con 70 columnas).

---

### 🎯 **Análisis Refinado de los Clusters Identificados**

### **📈 Cluster 0 - "Estudiantes promedio" (37.6%)**
| **Característica** | **Valor** | **Interpretación** |
|-------------------|-----------|-------------------|
| **Rendimiento** | 153.35 puntos globales | Nivel académico medio |
| **Nivel socioeconómico** | Estrato 2.24, INSE 51.37 | Bajo-medio |
| **Fecha de nacimiento promedio** | Nacimiento promedio en el año 1995 | Población estudiantil típica |
| **Fortalezas** | Inglés (154.71) y Lectura crítica (158.07) | Competencias lingüísticas sólidas |
| **Interpretación** | Representan el grupo más numeroso del sistema educativo colombiano, con rendimiento sólido pero no excepcional |

### **⚠️ Cluster 1 - "Estudiantes en desventaja académica" (28.7%)**
| **Característica** | **Valor** | **Interpretación** |
|-------------------|-----------|-------------------|
| **Rendimiento** | 121.42 puntos globales | El más bajo de todos los clusters |
| **Nivel socioeconómico** | Estrato 2.10, INSE 50.36 | Bajo |
| **Fecha de nacimiento promedio** | Nacimiento promedio en el año 1994 | Similar al cluster promedio |
| **Debilidades** | Todos los módulos < 133 puntos | Dificultades académicas generalizadas |
| **Interpretación** | Estudiantes que requieren mayor apoyo educativo y nivelación académica |

### **👨‍🎓 Cluster 2 - "Estudiantes adultos" (12.9%)**
| **Característica** | **Valor** | **Interpretación** |
|-------------------|-----------|-------------------|
| **Rendimiento** | 133.96 puntos globales | Medio-bajo |
| **Nivel socioeconómico** | Estrato 2.39, INSE 47.21 | El más bajo socioeconómicamente |
| **Fecha de nacimiento promedio** | Nacimiento promedio en el año 1980 | Significativamente mayor |
| **Característica única** | Mayor edad con rendimiento intermedio | Posiblemente estudiantes-trabajadores |
| **Interpretación** | Estudiantes que retoman educación superior después de tiempo, con desafíos adicionales |

### **🏆 Cluster 3 - "Estudiantes de alto rendimiento" (20.8%)**
| **Característica** | **Valor** | **Interpretación** |
|-------------------|-----------|-------------------|
| **Rendimiento** | 179.53 puntos globales | Excelente desempeño académico |
| **Nivel socioeconómico** | Estrato 3.47, INSE 62.27 | Medio-alto, el más alto |
| **Fecha de nacimiento promedio** | Nacimiento promedio en el año 1996 | Los más jóvenes |
| **Fortalezas destacadas** | Inglés (193.87) y Competencias ciudadanas (179.47) | Dominio sobresaliente |
| **Interpretación** | Estudiantes de élite académica, probablemente de universidades de alto prestigio |

---

### 🔑 **Patrones clave identificados**

### 📉 **Brechas y desigualdades**
1. **Brecha socioeconómica evidente**: 
   - Cluster 3 (alto rendimiento): Estrato 3.47
   - Cluster 1 (bajo rendimiento): Estrato 2.10
   - **Diferencia**: 1.37 estratos

2. **Edad como factor influyente**:
   - Los clusters más jóvenes (0 y 3) tienen mejor rendimiento
   - El cluster adulto (2) muestra rendimiento medio-bajo a pesar de mayor experiencia

3. **El inglés como mayor diferenciador**:
   - Cluster 3: 193.87 puntos en inglés
   - Cluster 1: 132.57 puntos en inglés
   - **Brecha**: 61.3 puntos (la más grande entre todas las competencias)

4. **Distribución académica desigual**:
   - **66.3%** de estudiantes en clusters de rendimiento medio o bajo
   - Solo **20.8%** en el cluster de alto rendimiento

---

### 🎓 **Recomendaciones basadas en los hallazgos**

| **Cluster** | **Intervención Recomendada** | **Objetivo** |
|------------|-----------------------------|--------------|
| **Cluster 1** | Programas de nivelación académica y tutorías personalizadas | Reducir brechas de aprendizaje |
| **Cluster 2** | Flexibilidad horaria y metodologías adaptadas a estudiantes adultos | Mejorar retención y desempeño |
| **Cluster 0** | Mentorías para potenciar rendimiento medio a alto | Maximizar potencial académico |
| **Cluster 3** | Programas de profundización y liderazgo académico | Desarrollar futuros investigadores |

---

### 📈 **Implicaciones para políticas educativas**

1. **Focalización de recursos**: Dirigir apoyos a Clusters 1 y 2 donde las necesidades son mayores
2. **Programas diferenciados**: Diseñar estrategias según perfil estudiantil identificado
3. **Reducción de brechas**: Implementar acciones específicas para disminuir la brecha de inglés (61.3 puntos)
4. **Sistemas de alerta temprana**: Usar estos perfiles para identificar estudiantes en riesgo académico

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
