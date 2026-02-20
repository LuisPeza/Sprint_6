# Proyecto 6: Análisis del Mercado Global de Videojuegos
> **Predicción de Éxito y Planificación Estratégica para la Tienda Online "ICE"**

---

## 📝 Descripción del Proyecto
Como analista de datos para la tienda online **ICE**, el objetivo es identificar patrones que determinen si un videojuego tendrá éxito o no. Utilizando datos históricos de ventas, plataformas, géneros y calificaciones (ESRB y críticas), este análisis permite detectar proyectos prometedores y planificar campañas publicitarias efectivas para el siguiente año.

### 🎯 Objetivo Principal
Determinar los factores críticos (plataforma, género, clasificación y reseñas) que impulsan las ventas de un videojuego en las diferentes regiones del mundo.

---

## 📂 Diccionario de Datos
El dataset incluye información de ventas y críticas hasta finales de 2016:

| Columna | Descripción |
| :--- | :--- |
| `Name` | Nombre del videojuego. |
| `Platform` | Plataforma (Xbox, PS4, PC, etc.). |
| `Year_of_Release` | Año de lanzamiento. |
| `Genre` | Género del juego. |
| `NA_sales` | Ventas en Norteamérica (millones de USD). |
| `EU_sales` | Ventas en Europa (millones de USD). |
| `JP_sales` | Ventas en Japón (millones de USD). |
| `Critic_Score` | Puntuación de expertos (máximo de 100). |
| `User_Score` | Puntuación de usuarios (máximo de 10). |
| `Rating` | Clasificación ESRB (E, T, M, etc.). |

---

## 📈 Hallazgos del Análisis de Datos

### 1. Ciclo de Vida de las Plataformas
* **Tendencia:** El sector alcanzó su auge entre **2008 y 2009**. Tras un declive post-crisis financiera, el mercado se ha vuelto más competitivo y selectivo.
* **Duración:** Las plataformas tienen una vida útil promedio donde las nuevas tardan en aparecer y las antiguas desaparecen gradualmente. Para el pronóstico de 2017, se priorizaron los datos de los **últimos 5 a 10 años**.
* **Líderes:** PS2, X360, Wii y DS dominan el histórico, pero se observa el crecimiento de PS4 y Xbox One hacia el final del periodo.

### 2. Perfil de Usuario por Región
El comportamiento de compra varía drásticamente según la geografía:

* **Norteamérica (NA):** Prefieren Xbox y PlayStation; el género líder es Acción y Deportes.
* **Europa (EU):** Dominio claro de PlayStation; tendencia similar en géneros a NA.
* **Japón (JP):** El mercado es liderado por **Nintendo (3DS)** y juegos portátiles. El género más vendido es **Role-Playing**.

### 3. Impacto de las Reseñas y Clasificación
* **Críticos vs Ventas:** Existe una correlación positiva. Las reseñas de expertos tienen un mayor peso en el éxito comercial inicial que las reseñas de usuarios.
* **Clasificación ESRB:** La categoría **E (Para todos)** es la más vendida globalmente, seguida de **M (Maduro)** y **T (Adolescentes)**, que compiten estrechamente en Occidente.

---

## 🧪 Pruebas de Hipótesis Estadísticas
Se utilizó la prueba **t de Student** con un nivel de significancia ($\alpha$) de **5%**.

1.  **Plataformas (Xbox One vs PC):** * **Resultado:** Se rechazó la hipótesis nula ($p < 0.05$).
    * **Conclusión:** Las calificaciones promedio de los usuarios son estadísticamente **diferentes** entre ambas plataformas.
2.  **Géneros (Acción vs Deportes):** * **Resultado:** No se pudo rechazar la hipótesis nula ($p > 0.05$).
    * **Conclusión:** Las calificaciones de los usuarios para Acción y Deportes son estadísticamente **similares**.

---

## 🏁 Conclusión General
Para asegurar una campaña exitosa en 2017, la tienda ICE debe:
1.  **Focalizar la publicidad** en los géneros **Action, Sports y Shooter** para los mercados de América y Europa.
2.  **Invertir en RPG** para el mercado japonés, priorizando plataformas portátiles de Nintendo.
3.  **Monitorear los lanzamientos de PS4 y Xbox One**, ya que son las plataformas con mayor potencial de crecimiento actual.
4.  **Priorizar juegos con Clasificación "E"**, debido a su volumen de ventas constante en las tres regiones.

---

## 🛠️ Metodología Aplicada
* **Limpieza de Datos:** Estandarización de nombres a minúsculas (*snake_case*).
* **Tratamiento de Datos:** Conversión de tipos de datos y manejo de valores ausentes en *Rating* y *Scores*.
* **Visualización:** Uso de histogramas, diagramas de caja (boxplots) y gráficos de dispersión para identificar correlaciones.

---

## 🔗 Entregables
* [📂 Ver Notebook de Análisis ICE (GitHub)](https://github.com/LuisPeza/Sprint_6/blob/main/Proyecto_6_Integral-%20Tienda%20de%20video%20juegos%20en%20linea.ipynb)
