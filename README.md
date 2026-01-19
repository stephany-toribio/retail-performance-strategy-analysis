# 🏪 Retail Strategic Analysis: Store Divestiture Decision

![Python](https://img.shields.io/badge/Python-Data%20Analysis-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Manipulation-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Business Intelligence](https://img.shields.io/badge/Strategy-Decision%20Making-darkgreen?style=for-the-badge)

## 💼 Escenario de Negocio

**El Desafío:** El propietario de una cadena de retail multi-rubro necesita optimizar sus activos. La empresa posee 4 tiendas físicas, pero por motivos estratégicos, **debe vender/cerrar una de ellas**.

**El Objetivo:** No se trata de una decisión basada en la intuición, sino en los datos. Este proyecto consolida, limpia y analiza la información transaccional de las 4 sucursales para responder: **¿Cuál es la tienda menos eficiente y prescindible?**

---

## 🔬 Enfoque Analítico (Methodology)

Para llegar a una conclusión robusta, se evaluaron tres dimensiones críticas de negocio:

### 1. Dimensión Financiera (Revenue)
* Análisis de **Facturación Total** y Ticket Promedio.
* Evaluación de costos operativos (Costos de envío absorbidos por la empresa).

### 2. Dimensión de Cliente (CX & NPS)
* Análisis de **Satisfacción del Cliente (NPS)** basado en las calificaciones (Ratings).
* Identificación de problemas recurrentes en tiendas específicas.

### 3. Dimensión Operativa & Geográfica
* Distribución de ventas por Categoría de Producto.
* Eficiencia logística según la ubicación (`lat`, `lon`) y tiempos de respuesta.

---

## 🛠️ Ingeniería de Datos & Stack

El flujo de trabajo técnico en Python incluyó:

* **Data Consolidation:** Ingesta y concatenación de 4 fuentes de datos dispersas (`tienda_1.csv` a `tienda_4.csv`) en un único DataFrame maestro utilizando **Pandas**.
* **Data Cleaning:** Normalización de fechas, manejo de valores nulos y estandarización de tipos de datos numéricos.
* **Exploratory Data Analysis (EDA):** Visualización de tendencias de ventas y comparativas de performance usando **Matplotlib/Seaborn**.

---

## 📊 Descripción del Dataset

El análisis se alimenta de datos transaccionales reales con los siguientes campos clave:

| Campo | Descripción | Importancia para el Análisis |
| :--- | :--- | :--- |
| `Producto` / `Categoría` | Tipo de item vendido | Mix de ventas y diversificación. |
| `Precio` | Valor de venta | Ingresos brutos (Revenue). |
| `Costo de envío` | Costo logístico | Impacto en el margen de ganancia. |
| `Calificación` | Rating (1-5 o 1-10) | Métrica clave para calcular NPS y fidelidad. |
| `Lugar de Compra` | Ciudad/Sucursal | Variable pivote para la comparación. |
| `Lat` / `Lon` | Coordenadas | Análisis geoespacial de cobertura. |

---

## 💡 Insights y Veredicto Final

*(Aquí debes resumir brevemente lo que descubriste en tu notebook. Ejemplo genérico basado en tu análisis:)*

Tras el análisis comparativo, se detectaron los siguientes patrones:
* ✅ **Tienda [X]:** Muestra el mayor crecimiento en facturación y el NPS más alto, siendo la "Joya de la Corona".
* ⚠️ **Tienda [Y]:** Aunque factura bien, tiene costos de envío desproporcionados que erosionan el margen.
* ❌ **Tienda [Z] (Candidata a Venta):** Presenta la combinación crítica de **baja facturación** y **baja satisfacción del cliente**. No muestra signos de recuperación a corto plazo.

> **Recomendación Estratégica:** Basado en los datos, se sugiere proceder con la venta de la **Tienda [Nombre de la tienda menos rentable]** para reinvertir capital en la optimización logística de las sucursales restantes.

---

### 👤 Autor

**Stephany Marilyn Toribio Alvarado**
* *Data Scientist & Analyst*
* Expertise: Business Intelligence | Machine Learning | Strategic Planning
* [LinkedIn](https://www.linkedin.com/in/stephany-marilyn-toribio-alvarado-47080b303/) | [Portafolio](https://stephany-toribio.github.io/MWeb/)
