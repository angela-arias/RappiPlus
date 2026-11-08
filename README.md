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


## Desarrollo ##
Para lograr responder las preguntas de negocio se debe iniciar con datos confiables. Para ello:

Se importaron las librerias, se cargaron los datasets, se validó su calidad, se diagnosticaron que tan completos estaban los datos.

Se detectaron columnas con Dtype incorrecto,  como por ejemplo columnas de fechas con otros tipos, se procedió a su corrección.

Se identificaron 100 duplicados en orders, luego de ser revisados se encontró que efectivamente eran datos duplicados y que su eliminación era necesaria para no inflar los valores como ventas, costos, marketing.

En orders se encontraron 50 NaNs los cuales no tenian información categoria_producto, cantidad, precio_unitario, monto_descuento. Pero si tenia información en **monto_total**. Luego de su revisión se puedo recuperar la categoria_producto desde la columna nombre_producto. Se mantuvieron los 50 registros ya que al contener el monto total serviria para futuras métricas, sin embargo, se marcaron como "detalle incompleto".

Además, 30 filas más no tenian información ni en categoria_producto ni en nombre_producto, pero si contenian el resto de información util para futuras métricas,  por tal motivo, se marcaron como "Sin dato" las columnas en mención.



04 valores negativos que no correspondian a devoluciones, 10 outilers




