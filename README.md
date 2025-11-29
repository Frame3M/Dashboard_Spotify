# 🎧 Spotify SaaS Retention Dashboard | Power BI

![Power BI](https://img.shields.io/badge/Power_BI-Desktop-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

Un Dashboard Ejecutivo end-to-end diseñado para analizar métricas clave de un modelo de negocio SaaS (Software as a Service), simulando datos de suscripción de Spotify. El proyecto se enfoca en la retención de clientes, análisis de Churn y patrones de comportamiento del usuario.

## 📸 Vista Previa del Proyecto

### Página 1: Executive Performance Overview
Esta vista proporciona una radiografía financiera y operativa del negocio.

![SpotifyDashboard_page-0001](https://github.com/user-attachments/assets/8cba10c1-6ccb-45a1-90c6-ff5e18c580ab)


### Página 2: User Behavior Analysis
Un análisis profundo para diagnosticar las causas raíz de la cancelación (Churn).

![SpotifyDashboard_page-0002](https://github.com/user-attachments/assets/9757b913-1218-47fb-bb91-b49da7c7db35)

---

## 💼 El Reto de Negocio
El objetivo principal fue transformar datos crudos de comportamiento y transacciones en insights accionables para responder:
1.  **Salud Financiera:** ¿Cómo evoluciona el MRR (Monthly Recurring Revenue) y el crecimiento de suscriptores?
2.  **Retención:** ¿Cuál es la Tasa de Churn actual y cómo se compara con periodos anteriores?
3.  **Comportamiento:** ¿Qué acciones específicas de los usuarios (saltar canciones, tiempo de escucha) predicen una futura cancelación?

## 🛠️ Stack Tecnológico & Habilidades Aplicadas

* **Herramienta:** Microsoft Power BI Desktop.
* **Lenguajes:** DAX (Data Analysis Expressions), Power Query (M).
* **Modelado de Datos:** Esquema en Estrella (Star Schema) con tablas de hechos y dimensiones.
* **Diseño UI/UX:** Interfaz moderna en "Dark Mode" consistente con la identidad de marca de Spotify, navegación tipo App.

### Características Técnicas Destacadas:
* **Inteligencia de Tiempo:** Cálculos de `Last Month` y `Last Year` para variaciones porcentuales (YoY, MoM).
* **DAX Avanzado:** Uso de `CALCULATE`, `KEEPFILTERS` para segmentación compleja y `USERELATIONSHIP` para manejar fechas de registro y cancelación en una misma tabla calendario.
* **Transformación de Datos:** Limpieza de lógica booleana (True/False) y agrupación de datos (Binning) para histogramas y gráficos de dispersión.

---

## 🔍 Insights Clave Descubiertos

A través del análisis visual, se detectaron los siguientes patrones:

1.  **El Factor "Skip Rate":** Existe una correlación positiva clara entre la tasa de saltos y el Churn. Los usuarios que saltan contenido frecuentemente tienen un riesgo de abandono significativamente mayor.
2.  **Duración vs. Cantidad:**
    * El volumen de canciones escuchadas por día (~50) es idéntico entre usuarios retenidos y cancelados, indicando que la cantidad no predice fidelidad.
    * Sin embargo, el **tiempo de escucha total** sí muestra una correlación inversa con el Churn: a mayor tiempo en la plataforma, menor riesgo de fuga.
3.  **Plataformas:** Los usuarios de dispositivos móviles presentan una tasa de cancelación ligeramente superior a los de escritorio, lo que sugiere revisar la experiencia de usuario en la App móvil.

---

## 📂 Estructura del Dataset
El dataset original contiene información simulada de usuarios de Spotify, incluyendo:
* **Demografía:** Edad, Género.
* **Suscripción:** Tipo de Plan (Family, Individual, Student), Fecha de Alta, Fecha de Baja.
* **Comportamiento:** Tiempo de escucha, Canciones por día, Tasa de saltos (Skip Rate).

Fuente: https://www.kaggle.com/datasets/nabihazahid/spotify-dataset-for-churn-analysis

## 🚀 Cómo usar este archivo
1.  Descarga el archivo `.pbix` de este repositorio.
2.  Abre el archivo en **Power BI Desktop**.
3.  Navega entre las páginas usando el menú lateral interactivo.
4.  Interactúa con los filtros de Año, Mes y Tipo de Suscripción para ver cómo cambian los KPIs dinámicamente.

---

### 👤 Autor
**Marco Ortega**
* LinkedIn: https://www.linkedin.com/in/ortegamarco03/
* Portfolio: https://portfolio-three-smd.vercel.app/

*Este proyecto es una simulación con fines educativos y de portafolio.*
