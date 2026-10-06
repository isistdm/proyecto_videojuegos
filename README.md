# 🎮 Análisis de Ventas de Videojuegos — ICE (2016)

## 📌 Descripción del Proyecto
Este proyecto fue desarrollado para **ICE**, una tienda online que comercializa videojuegos a nivel mundial.  
El objetivo es **identificar patrones de éxito en los videojuegos** a partir de reseñas de usuarios y críticos, géneros, plataformas y datos históricos de ventas.  
Con esta información se busca **detectar proyectos prometedores y planificar campañas publicitarias efectivas**.

---

## 🗂️ Dataset
Fuente: `/datasets/games.csv`  
Columnas principales:
- **Name**: Nombre del videojuego  
- **Platform**: Plataforma (PS4, Xbox, etc.)  
- **Year_of_Release**: Año de lanzamiento  
- **Genre**: Género del juego  
- **NA_sales, EU_sales, JP_sales, Other_sales**: Ventas por región (en millones USD)  
- **Critic_Score**: Calificación de críticos (0–100)  
- **User_Score**: Calificación de usuarios (0–10)  
- **Rating**: Clasificación ESRB  

---

## 🛠️ Pasos del Proyecto
1. **Preparación de datos**  
   - Normalización de nombres de columnas  
   - Conversión de tipos de datos  
   - Tratamiento de valores ausentes y casos “TBD”  
   - Creación de columna de ventas globales  

2. **Análisis exploratorio**  
   - Evolución de lanzamientos por año  
   - Ciclo de vida de plataformas  
   - Distribución de ventas por género y región  
   - Relación entre reseñas y ventas  

3. **Perfil de usuario por región**  
   - Top 5 plataformas y géneros en NA, EU y JP  
   - Impacto de clasificaciones ESRB en cada mercado  

4. **Pruebas de hipótesis**  
   - Comparación de calificaciones de usuarios entre plataformas (XOne vs PC)  
   - Diferencias en calificaciones entre géneros (Action vs Sports)  

5. **Conclusión general**  
   - Identificación de plataformas líderes (PS4 y XOne)  
   - Segmentación de campañas por región  
   - Importancia de reseñas de críticos en ventas  
   - Géneros más rentables: Action, Shooter, Sports y Role-Playing  

---

## 📊 Principales Hallazgos
- Las plataformas alcanzan su **máximo de ventas alrededor de los 4 años** tras su lanzamiento y mantienen relevancia por ~10 años.  
- El mercado está **altamente concentrado**: pocos títulos generan ventas extraordinarias.  
- Las reseñas de críticos tienen **correlación positiva moderada (~0.4)** con las ventas, mientras que las de usuarios no muestran relación significativa.  
- **Norteamérica y Europa concentran el 75% de las ventas globales**, con patrones similares; Japón presenta preferencias distintas (Role-Playing y Action).  
- Los géneros más rentables son **Action, Shooter, Sports y Role-Playing**.  

---

## 🚀 Conclusión
El análisis sugiere que la campaña de 2017 debe enfocarse en:
- **Plataformas PS4 y XOne**, aún vigentes y con ventas altas.  
- **Segmentación regional**: campañas conjuntas para NA y EU, diferenciadas para JP.  
- **Géneros clave**: Action, Shooter, Sports y Role-Playing.  
- **Reseñas de críticos** como factor estratégico en marketing.  

---

## 📌 Tecnologías utilizadas
- **Python** (pandas, matplotlib, seaborn, scipy)  
- **Jupyter Notebook**  
- **Git/GitHub** para control de versiones  

## 📂 Estructura del Repositorio

proyecto_videojuegos/
├── datasets/
│   └── games.csv
├── videojuegos_analysis.ipynb
├── README.md
└── .gitignore
