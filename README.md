## Introducción ##

**RappiPlus** es un servicio de suscripción dentro del ecosistema de Rappi diseñado para aumentar la frecuencia de compra y el valor generado por usuario. 

## 🎯 Objetivo del proyecto ##
A lo largo de este proyecto se responderá si el negocio es rentable, si los usuarios regresan a comprar, si los cambios en las plataformas generan impacto, todo esto basado en información confiable. 

## 🗂️ Fuentes usados ##

rappiplus_orders_raw.csv

rappiplus_catalog.csv

rappiplus_marketing_spend.csv

Tabla de Events

Tabla de Users

Tabla de User Activity

experiment_checkout_ui.csv


## Metodología ##

Limpieza de datasets: se encontraron duplicados, NaNs, valores negativos y outliers.

Análisis exploratorio

Visualizaciones

Análisis de cohortes

Prueba estadistica: Z test


## Principales hallazgos ##

El negocio es rentable en el periodo, incluso después de descontar marketing.

Marketing es la partida que más pesa: equivale a cerca del 30% del ingreso y a casi la mitad del profit bruto.

En el funnel, la mayor pérdida ocurre entre begin_checkout y add_payment_info: se pierden 958 usuarios (13,29%).

La retención semanal es estable (entre ~40% y ~44%) en todas las cohortes de registro.

El cambio de UI del checkout no mostró un efecto estadísticamente significativo (p = 0,4161).

Las ventas están repartidas de forma pareja entre categorías (~33% del ingreso cada una). Hogar y Moda venden más unidades que Electrónica.


## Herramientas ##

Python, SQL, pandas, numpy, seaborn, matplotlib









