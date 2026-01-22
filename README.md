# 📊 ZAKIDATA Empowerdata - Seguimiento Financiero Retail

<div align="center">

**Dashboard Estratégico para el Monitoreo de Ventas, Facturación y Distribución Geográfica**

[🚀 Características](https://www.google.com/search?q=%23-caracter%C3%ADsticas) • [📊 Instalación](https://www.google.com/search?q=%23-instalaci%C3%B3n) • [🏗️ Arquitectura](https://www.google.com/search?q=%23%EF%B8%8F-arquitectura) • [🎨 Diseño](https://www.google.com/search?q=%23-dise%C3%B1o-del-dashboard) • [📈 Métricas](https://www.google.com/search?q=%23-m%C3%A9tricas-analizadas) • [👨‍💻 Autor](https://www.google.com/search?q=%23-autor)

</div>

---

## 📊 Descripción del Proyecto

**ZAKIDATA Empowerdata - Seguimiento Financiero** es una solución analítica avanzada desarrollada en **Power BI** para la cadena de tiendas "EmpowerTravel Store" en Brasil. El dashboard centraliza la información de facturación, volumen de pedidos y comisiones, permitiendo una visión de 360° sobre el rendimiento de los productos y la eficiencia de las sucursales físicas.

### 🎯 Objetivos del Proyecto

* **Visualizar el rendimiento financiero** global (Facturación total de $3.57 millones).
* **Analizar la estacionalidad** de las ventas mediante una vista mensual detallada.
* **Identificar productos estrella** a través de un selector visual intuitivo (Botellas, Mochilas, etc.).
* **Monitorear la expansión geográfica** en el territorio brasileño.
* **Evaluar el market share interno** de cada tienda física.

---

## 🚀 Características

### 📈 Métricas Principales

| Característica | Descripción | Estado |
| --- | --- | --- |
| **Facturación Total** | Indicador clave (KPI) de ingresos brutos | ✅ Implementado |
| **Volumen de Pedidos** | Conteo total de transacciones (611 pedidos) | ✅ Implementado |
| **Comisiones** | Cálculo del margen destinado a comisiones ($178.6K) | ✅ Implementado |
| **Facturación por Período** | Análisis de tendencias temporales de enero a diciembre | ✅ Implementado |
| **Geolocalización** | Mapa de burbujas con presencia de tiendas en Brasil | ✅ Implementado |
| **Ranking de Tiendas** | Comparativa de rendimiento relativo y porcentual | ✅ Implementado |

### 🔍 Filtros e Interactividad

* **Selector de Productos Visual**: Filtro táctil para categorías (Audífonos, Gorra, Billetera, Maleta, Bolso, Mochila, Botella, Tennis).
* **Mapa Interactivo**: Filtrado por ubicación geográfica al seleccionar puntos de venta.
* **Análisis de Pareto**: Tabla de tiendas con barras de datos para identificar el 80/20 de los ingresos.
* **Tooltips dinámicos**: Detalle de facturación mensual al pasar el cursor sobre las barras.

---

## 📊 Instalación

### **Requisitos Previos**

1. **Power BI Desktop** (Última versión).
2. **Dataset de Ventas**: Archivo Excel o base de datos SQL con registros de facturación, tiendas y productos.

### **Pasos de Instalación**

```bash
# 1. Clonar el repositorio
git clone https://github.com/tu-usuario/seguimiento-financiero-brasil.git

# 2. Abrir el archivo
# ZAKIDATA_Seguimiento_Financiero.pbix

# 3. Refrescar Datos
# Configurar parámetros de origen si los nombres de los archivos locales difieren.

```

---

## 🏗️ Arquitectura

### **Medidas DAX Principales**

```dax
// Facturación Total Format
Facturacion_Millones = DIVIDE(SUM(Ventas[Importe]), 1000000)

// Cálculo de Comisión (Ejemplo 5%)
Total_Comision = SUM(Ventas[Importe]) * 0.05

// % de Participación por Tienda
Market_Share_Tienda = 
DIVIDE(
    SUM(Ventas[Importe]), 
    CALCULATE(SUM(Ventas[Importe]), ALL(Tiendas))
)

```

---

## 🎨 Diseño del Dashboard

### **Estética y UI**

* **Dark Mode**: Fondo oscuro para reducir la fatiga visual y resaltar los colores vibrantes (Rojo/Rosa).
* **Layout Moderno**: Uso de contenedores redondeados y sombras para separar secciones.
* **Visuales Personalizados**:
* Mapa de calor/burbujas para distribución regional.
* Slicer de imágenes para selección de categorías de productos.



### **Organización de Pantalla**

1. **Header**: Título y branding (ZAKIDATA | Empowerdata).
2. **Panel Central Izquierdo**: Selector de productos con imágenes reales.
3. **Panel Central Derecho**: KPIs destacados y Mapa de Brasil.
4. **Footer**: Gráfico de barras mensual y tabla de ranking de tiendas.

---

## 📈 Métricas Analizadas (Snapshot Actual)

### **1. Desempeño General**

* **Facturación:** $3,572,319.20
* **Total Pedidos:** 611
* **Comisión Generada:** $178,615.96

### **2. Top 3 Tiendas por Facturación**

1. **Tienda 4:** $1,433,866.7 (40.14% del total)
2. **Tienda 6:** $644,100.7 (18.03% del total)
3. **Tienda 5:** $600,198.3 (16.80% del total)

### **3. Tendencia Mensual**

* **Mes Pico:** Mayo ($0.49 mill.)
* **Meses de Estabilidad:** Enero ($0.4 mill.) y Septiembre ($0.40 mill.)
* **Valle de Ventas:** Noviembre ($0.17 mill.)

---

## 👨‍💻 Autor

<div align="center">

**DARWIN OVALLES**

**Analista de BI especializado en Retail y Finanzas**

*"Convertir datos de ventas en decisiones estratégicas es el motor del crecimiento empresarial moderno."*

**#PowerBI #DataVisualization #RetailAnalytics #BrazilSales #FinancialReporting**

</div>

---

### ⭐ ¿Te gustó este proyecto?

¡No olvides darle una estrella al repositorio para apoyar el desarrollo de más dashboards de acceso libre!

Would you like me to adjust any specific metric or add a section about the data cleaning process (Power Query)?
