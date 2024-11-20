# Análisis para una empresa de Telecomunicaciones (Internet)

Este repositorio contiene un análisis detallado sobre sobre el acceso y la calidad del servicio de internet en Argentina.
El objetivo del proyecto es evaluar el acceso a la tecnología, las tendencias de velocidad y las métricas clave para mejorar la conectividad a nivel nacional y por provincias específicas.

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

- **Dataset Utilizado**: `p_totales_provincia.csv`

### KPI 2: Incremento de velocidad en provincias rezagadas
- **Objetivo**: Aumentar la velocidad de Internet en al menos 2 provincias rezagadas en más de 10 Mbps.
- **Fórmula**:
KPI_Velocidad = ((Velocidad Promedio Actual (2024-1) - Velocidad Promedio Anterior (2023-1)) * 100) / Velocidad Promedio Anterior (2023-1)

- **Provincias Rezagadas**: `Santiago Del Estero`, `La Pampa`, `San Juan`, `Santa Cruz`, `Tierra Del Fuego`
- **Dataset Utilizado**: `velocidad_provincia.csv`

### KPI 3: Aumento de conexiones a nivel nacional
- **Objetivo**: Aumentar las conexiones de Internet en un 2% a nivel nacional por cada 100 habitantes, de 2023-1 a 2024-1.
- **Fórmula**:
KPI = ((AccesosActual (2024-1) - AccesosAnterior (2023-1)) / AccesosAnterior (2023-1)) * 100

- **Dataset Utilizado**: `p_totales_provincia.csv`

## Conclusiones

Los análisis realizados y los KPIs establecidos son fundamentales para mejorar la conectividad a nivel provincial y nacional. Las visualizaciones generadas en los dashboards ayudan a entender las tendencias y áreas críticas, mientras que los KPIs permiten medir el impacto de las acciones propuestas para mejorar el acceso y la velocidad de Internet.

### Tendencias en Velocidades y Conexiones
1. Tendencia General:

Las velocidades promedio han crecido de manera consistente, con un salto marcado durante y después de la pandemia debido a la creciente demanda de conectividad.
Buenos Aires y Capital Federal destacan por su constante crecimiento, reflejo de una infraestructura tecnológica consolidada.

2. Impacto del COVID-19:

La pandemia aceleró el desarrollo de infraestructura en regiones clave, principalmente en áreas urbanas densas, pero dejó al descubierto la brecha digital en zonas rurales y remotas.

3. Provincias Rezagadas:

Tierra del Fuego y Santiago del Estero requieren mayores inversiones para cerrar la brecha digital, mientras que otras provincias rurales también presentan desafíos de conectividad.
4. Proyecciones Futuras:

Invertir en infraestructura para provincias rezagadas será crucial para mejorar la conectividad general y reducir la desigualdad digital.


## Tendencias por Tecnología
- ADSL:
Declive significativo desde 2014, con una caída drástica desde 2018 debido a la migración hacia tecnologías más modernas.

- Cablemódem:
Estable, con ligeros altibajos. Sigue siendo relevante para mantenimiento, aunque su crecimiento es menor comparado con la fibra óptica.

- Fibra Óptica:
Crecimiento acelerado y constante, pasando de 150,323 conexiones en 2014 a 4,169,958 en 2024. Es la tecnología preferida por su velocidad y confiabilidad.

- Wireless y Otros:
Fluctuaciones moderadas y bajo crecimiento. Estas tecnologías no son atractivas frente a las opciones modernas como fibra óptica.

## Evaluación General de las Tendencias

- Crecimiento:
Fibra óptica lidera el crecimiento absoluto y proporcional, mientras que el cablemódem se mantiene como una alternativa relevante.
- Disminución:
ADSL pierde relevancia debido a limitaciones tecnológicas, mientras que las conexiones inalámbricas permanecen estancadas.


## Cómo Ejecutar los Archivos

Para ejecutar los cuadernos de Jupyter y reproducir los análisis:

1. Clona este repositorio en tu máquina local:

git clone https://github.com/tu-usuario/repositorio.git


2. Ejecuta los cuadernos de Jupyter:
- `EDA.ipynb`: Para el análisis exploratorio de los datos.
- `ETL.ipynb`: Para el proceso de extracción, transformación y carga de los datos.

3. Abre el archivo de Power BI para explorar los dashboards:
- `Dashboard/p2_DA.pbix`




