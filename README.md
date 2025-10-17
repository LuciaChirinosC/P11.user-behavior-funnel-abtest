# P11.user-behavior-funnel-abtest
# 📲 Proyecto: Análisis del comportamiento del usuario y test A/A/B

Este proyecto forma parte del curso **"La toma de decisiones de negocios basadas en datos"**, y tiene como objetivo analizar el comportamiento de los usuarios dentro de una aplicación móvil de una empresa de productos alimenticios, a través del estudio del embudo de ventas y un experimento A/A/B.



## 🧠 Contexto
La empresa busca comprender cómo los usuarios interactúan con la aplicación, identificar los puntos donde se pierden en el proceso de compra y evaluar el impacto de un cambio en las fuentes del diseño de la app mediante un **test A/A/B**.


## 🎯 Objetivos del proyecto

1. **Analizar el embudo de conversión** para identificar las etapas críticas donde los usuarios abandonan el proceso.
2. **Evaluar el test A/A/B** para determinar si el cambio de fuente tiene un efecto significativo en el comportamiento del usuario.
3. **Comprobar la validez experimental** comparando los grupos de control A1 y A2 antes de contrastar con el grupo B.


## 📁 Datos

**Dataset:** `logs_exp_us.csv`

Cada registro representa un evento realizado por un usuario en la aplicación.  
Columnas principales:

- `EventName`: nombre del evento.  
- `DeviceIDHash`: identificador único del usuario.  
- `EventTimestamp`: marca de tiempo del evento.  
- `ExpId`: número del experimento  
  - **246 y 247** → grupos de control (fuentes antiguas)  
  - **248** → grupo experimental (fuentes nuevas)

## ⚙️ Etapas del análisis

### 1️⃣ Preparación de datos
- Carga y exploración del dataset.
- Limpieza de datos y conversión de tipos.
- Creación de columnas de fecha y hora.
- Verificación de la completitud del periodo de análisis.

### 2️⃣ Análisis del embudo de ventas
- Identificación de eventos y frecuencia.
- Construcción del embudo de conversión.
- Cálculo de tasas de retención entre etapas.
- Determinación de la etapa con mayor pérdida de usuarios.

### 3️⃣ Análisis del test A/A/B
- Verificación de equilibrio entre grupos A1 y A2.
- Pruebas de hipótesis para cada evento entre:
  - Grupos de control (246 vs 247).
  - Grupo experimental (248) vs grupos de control.
- Evaluación estadística de diferencias significativas.
- Conclusión sobre el impacto del cambio de fuentes.


## 🧮 Herramientas utilizadas
- **Python:** Pandas, NumPy, Matplotlib, Seaborn, SciPy  
- **Jupyter Notebook / VS Code**  
- **GitHub** para documentación y control de versiones  


## 📈 Resultados esperados
- Identificación del punto crítico de pérdida de usuarios en el embudo.  
- Confirmación de la validez experimental (A/A).  
- Determinación del impacto real del cambio de diseño (A/B).  
- Recomendaciones para futuras pruebas de usabilidad o diseño.


## 👩‍💻 Autor
**Lucía Chirinos Cornejo**  
Analista de Datos | Ingeniera Ambiental  

