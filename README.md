# **Proyecto: Análisis de Rendimiento de Tiendas AluraStore**

Este repositorio contiene el análisis de datos realizado para el desafío de AluraStore Latam. El objetivo es evaluar el rendimiento de cuatro tiendas para proporcionar una recomendación de negocio fundamentada.

## **1. Objetivo del Proyecto**

El dueño de la empresa AluraStore, necesita tomar una decisión estratégica sobre cuál de sus cuatro tiendas vender. Para ello, solicitó un análisis exhaustivo basado en datos transaccionales, con el fin de identificar la tienda con el rendimiento más bajo y, por lo tanto, la candidata principal para la venta.

## **2. Descripción de los Datos**

El análisis se basa en cuatro archivos de datos en formato `.csv`, cada uno correspondiente a una tienda:

* `tienda_1 .csv`
* `tienda_2.csv`
* `tienda_3.csv`
* `tienda_4.csv`

Cada archivo contiene registros de transacciones que incluyen información sobre el producto vendido, categoría, precio, costo de envío y la calificación otorgada por el cliente.

## **3. Metodología de Análisis**

El análisis completo se encuentra en el Jupyter Notebook `Challenge_AluraStoreLatam.ipynb`. El proceso siguió los siguientes pasos:

1.  **Importación de Datos:** Se cargaron los cuatro archivos CSV utilizando la biblioteca `pandas` de Python.
2.  **Limpieza y Estandarización de Fechas:** Se identificó la columna de fecha (`Fecha de Compra`) y se convirtió a un formato `datetime` para permitir operaciones temporales.
3.  **Filtrado de Datos para Coherencia:** Para garantizar una comparación justa ("manzanas con manzanas"), todos los datos fueron filtrados a un rango de fechas común y específico: **del 1 de enero de 2020 al 30 de marzo de 2023**.
4.  **Cálculo de Métricas Clave:** Se evaluaron cinco aspectos fundamentales para cada una de las tiendas sobre los datos ya filtrados:
    * Ingresos totales (Facturación).
    * Volumen de ventas por categoría de producto.
    * Calificación promedio del cliente.
    * Productos más y menos vendidos (por unidades).
    * Costo de envío promedio.

## **4. Resumen de Resultados**

La siguiente tabla consolida las métricas más importantes obtenidas del análisis sobre los datos filtrados, permitiendo una comparación directa del rendimiento de las tiendas.

| Métrica                  | Tienda 1      | Tienda 2      | Tienda 3      | Tienda 4      |
| :----------------------- | :------------ | :------------ | :------------ | :------------ |
| **Facturación (Ingresos)** | **$1,149.9 M** | $1,116.3 M    | $1,098.0 M    | **$1,038.3 M** |
| **Calificación Promedio** | **3.98** | 4.04          | **4.05** | 4.00          |
| **Costo Envío Promedio** | **$26,028** | $25,216        | $24,805        | **$23,459** |

---

## **5. Conclusión y Recomendación Final**

Tras un análisis riguroso y comparativo de las cuatro sucursales en un período de tiempo estandarizado, **se recomienda considerar la venta de la Tienda 4.**

Esta recomendación se fundamenta en los siguientes puntos clave:

1.  **Rendimiento Financiero Inferior:** La **Tienda 4** es, por un margen significativo, la que menos ingresos genera, con una facturación de **\$1,038.3 millones**. Esta cifra es considerablemente más baja que la de sus pares, cuya facturación mínima es de \$1,098.0 millones. Esta brecha representa el indicador más fuerte de bajo rendimiento.
2.  **Satisfacción del Cliente Mediocre:** Aunque no es la peor calificada, la Tienda 4 presenta una calificación promedio de **4.00**, inferior a la de las tiendas 2 y 3. No posee un nivel de servicio al cliente destacado que pueda compensar su débil desempeño financiero.
3.  **Contexto General:** Si bien la Tienda 1 presenta la peor calificación (3.98) y los costos de envío más altos, también es la que más factura. Sus problemas parecen ser de índole operativa y potencialmente solucionables, mientras que el problema de la Tienda 4 parece ser una menor capacidad para generar ventas en el mercado.

Para una decisión final, sería valioso enriquecer este análisis con datos adicionales, como los costos operativos de cada tienda y los márgenes de ganancia por producto, para obtener una visión completa de la rentabilidad. Sin embargo, con la información disponible, la **Tienda 4** es la candidata más clara para una desinversión.
