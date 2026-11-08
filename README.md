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


## 🛠️ Herramientas ##

Python, SQL, pandas, numpy, seaborn, matplotlib


## 🔍 Metodología ##

Limpieza de datasets: se encontraron duplicados, NaNs, valores negativos y outliers.

Análisis exploratorio

Visualizaciones

Análisis de cohortes

Prueba estadistica: Z test


## 🚀 Cómo ejecutar el notebook: 
 
#### ⚙️ Abrir en Google Colab:

1. Ve al archivo `.ipynb` dentro de este repositorio. 📓 [Ver notebook del análisis](S12_Estudiante_Proyecto_Final.ipynb)
  
2. Haz clic en el botón **"Open in Colab"** (o copia la URL del notebook y pégala en [https://colab.research.google.com](https://colab.research.google.com) → pestaña "GitHub").
   
3. Una vez abierto, ejecuta las celdas en orden desde el menú **Runtime > Run all**.

> No necesitas instalar Python ni librerías localmente; Colab ya las incluye.


## 📝 Principales hallazgos ##

El negocio es rentable en el periodo, incluso después de descontar marketing.

Marketing es la partida que más pesa: equivale a cerca del 30% del ingreso y a casi la mitad del profit bruto.

En el funnel, la mayor pérdida ocurre entre begin_checkout y add_payment_info: se pierden 958 usuarios (13,29%).

La retención semanal es estable (entre ~40% y ~44%) en todas las cohortes de registro.

El cambio de UI del checkout no mostró un efecto estadísticamente significativo (p = 0,4161).

Las ventas están repartidas de forma pareja entre categorías (~33% del ingreso cada una). Hogar y Moda venden más unidades que Electrónica.

## Gráficos Z test
![ver_1](z_test.JPG)

Rappiplus realizó una modificación en la UI del checkout para evaluar si impactaba la **tasa de conversión de compra**. Para lo cual se utilizó un Z test para su verificación. 

**Concluyendo que:** Las tasas de conversión de control (15.69%) y tratamiento (16.29%) son similares y sus intervalos de confianza al 95% se solapan. El test z (α = 0.05, p = 0.4161) y el intervalo de la diferencia [-0.84, 2.03] pp, que incluye el 0, indican que no hay evidencia estadística de que la nueva UI modifique la conversión. No rechazar H₀ no demuestra que ambas UI sean iguales: significa que con estos datos no se detectó un efecto.


## Gráficos Métricas
![ver_1](z_test.JPG)








