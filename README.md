# Proyecto de Análisis de Accesos a Internet y Velocidad por Provincia

Este repositorio contiene un análisis detallado sobre el acceso a Internet y la velocidad de conexión por provincia en base a varios conjuntos de datos. El objetivo del proyecto es evaluar el acceso a la tecnología, las tendencias de velocidad y las métricas clave para mejorar la conectividad a nivel nacional y por provincias específicas.

## Estructura del Repositorio

El repositorio contiene los siguientes archivos y carpetas:

### Archivos y Carpetas

- **Dashboard/p2_DA.pbix**: Proyecto de Power BI que contiene los dashboards con la visualización de los datos analizados y los KPIs calculados.
  
- **Data/**: Carpeta que contiene los archivos de datos utilizados en el análisis:
  - **accesos_tecnologia_provincia.csv**: Datos sobre las conexiones por tipo de tecnología en diferentes provincias.
  - **ingresos.csv**: Datos sobre los ingresos anuales generados por el servicio de Internet.
  - **p_totales_provincia.csv**: Datos sobre la cantidad de accesos a Internet por cada 100 hogares/habitantes en las provincias.
  - **totales_accesos_tecnologia.csv**: Datos sobre las conexiones por tipo de tecnología.
  - **velocidad_provincia.csv**: Datos sobre la velocidad de Internet promedio por provincia.

- **EDA.ipynb**: Cuaderno de Jupyter que contiene el análisis exploratorio de los datos, incluyendo la limpieza, el análisis de tendencias y la visualización de patrones en las variables.
  
- **ETL.ipynb**: Cuaderno de Jupyter que contiene el proceso de extracción, transformación y carga (ETL) de los datos, asegurando que estén listos para el análisis.

- **Internet.xlsx**: Archivo Excel que contiene los datos fuente que se utilizaron para construir los CSVs anteriores.

## Análisis Realizado

### EDA - Análisis Exploratorio de Datos

A continuación, se describe brevemente el análisis realizado en cada conjunto de datos.

#### 1. Velocidad de Conexión por Provincia
   - **Distribución porcentual**: Análisis de la distribución de la velocidad de conexión a Internet por provincia, identificando valores nulos, duplicados y outliers.
   - **Ranking de Provincias por Velocidad Media**: Se creó un ranking de las provincias en base a la velocidad promedio anual, utilizando un gráfico de barras horizontales.
   - **Análisis de Tendencias Temporales**: Se visualizó la variación de la velocidad promedio por provincia a lo largo del tiempo mediante un gráfico de líneas.

#### 2. Totales de Conexiones por Tecnología
   - **Evolución de las Conexiones por Tecnología**: Análisis de la evolución de las conexiones por tecnología a lo largo del tiempo, utilizando gráficos de líneas.
   - **Participación Porcentual de Tecnología**: Se calculó la proporción de cada tecnología en el total de conexiones, utilizando gráficos de barras al 100%.

#### 3. Accesos por Provincia
   - **Análisis Temporal**: Se analizó la evolución de los accesos a Internet por provincia mediante gráficos de líneas.
   - **Distribución Porcentual por Provincia**: Se visualizó la distribución porcentual de cada tecnología por provincia, utilizando gráficos de barras y gráficos de tortas.

#### 4. Accesos Totales por Provincia
   - **Distribución de Accesos**: Se graficó la distribución de accesos para cada 100 hogares/habitantes en las provincias, utilizando histogramas.
   - **Análisis Temporal**: Se graficó la evolución anual de los accesos por cada 100 hogares/habitantes en ciertas provincias, utilizando gráficos de líneas.

#### 5. Análisis de Ingresos
   - **Evolución Anual de Ingresos**: Se graficó la evolución de los ingresos anuales desde 2014 hasta 2024.
   - **Crecimiento Anual**: Se calculó la tasa de crecimiento de los ingresos, utilizando gráficos de líneas.

## KPIs (Indicadores Clave de Desempeño)

Se definieron y calcularon tres KPIs para medir el impacto de las mejoras en la penetración de Internet y la calidad de la conexión.

### KPI 1: Aumento del acceso a Internet por cada 100 hogares
- **Objetivo**: Aumentar en un 2% el acceso al servicio de internet para el próximo trimestre, por provincia.
- **Fórmula**: 

KPI = ((Nuevo acceso - Acceso Actual) / Acceso Actual) * 100

