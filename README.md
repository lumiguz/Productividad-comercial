<img src='https://res.cloudinary.com/dzc8agefr/image/upload/v1691860198/5_ajw7vx.png' alt='Dashboard'>

# Análisis Exploratorio de Datos


Este proyecto tiene como objetivo hacer un analisis EDA del [🔗 Dataset](./Dataset/data_prueba_cpa_v1%20-%20copia.xlsx) y asi poder extraer algunos insights para la toma de decisiones tanto del area Comercial como el area de Mercadeo


## Dataset

El dataset abarca el periodo del año 2021 de una empresa SaaS donde se observan las ventas por asesor


## Dashboard

Puedes descargar el archivo del [📊 Dashboar](./Dashboard/Analisis%20de%20productividad%20comercial.pbix) y visualizarlos en `Power BI`

## Variables de la tabla

|Index|Campo|Descripción|forma de calculo|
|-|-|-|-|
|1|Año_mes|Año y mes del registro (periodo)|No aplica|
|2|Celula|Equipo al que pertenece el asesor|No aplica|
|3|Asesor|Identificador del asesor comercial|No aplica|
|4|0021_meta|Meta de ventas del asesor|No aplica|
|5|0022_ventas|Ventas realizadas por el asesor comercial|No aplica|
|6|0023_cumplimiento|Cumplimiento de la meta del mes|=5/4|
|7|0045_%_Efectividad_SQL|Conversion de seg creados mismo mes a venta mismo mes|=9/18|
|8|0044_%_Ventas_mercadeo|Participacion % de ventas de origen mercadeo respecto a ventas totales|=(9+11)/5|
|9|0031_ventas_mismo_mes|Ventas origen mercadeo con leads del mes|No aplica|
|10|0041_%_Ventas_leads_mes|Participacion % de ventas de origen mercadeo mismo mes respecto a ventas totales|=9/5|
|11|0032_ventas_mes_anterior|Ventas origen mercadeo con leads de meses anteriores|No aplica|
|12|0042_%_Ventas_leads_mes_anterior|Participacion % de ventas de origen mercadeo meses anteriores respecto a ventas totales|=12/5|
|13|0033_ventas_0_a_100|Ventas cerradas el mismo dia que ingresa el lead (subcojunto de ventas leads mes)|No aplica|
|14|0043_%_Ventas_leads_cero_a_cien|Participacion % de ventas de origen mercadeo cero a cien  respecto a ventas totales|=13/5|
|15|0024_seg_atrasados|Cantidad de seguimientos atrasados|No aplica|
|16|0025_seg_abiertos|Cantidad de seguimientos abiertos (compuesto por leads mercadeo de cualquier periodo y oportunidades de otros origenes (ej. Referidos))|No aplica|
|17|0026_descartes_totales|Descartes de seguimientos con origen mercadeo de cualquier periodo|No aplica|
|18|0027_seg_creados_mismo_mes|Seguimientos (Leads) generados por mercadeos en el mes en curso|No aplica|
|19|0028_descartes_mismo_mes|Descarte de seguimientos con origen mercadeo en el mismo mes de creacion|No aplica|
|20|0029_%_descarte_mismo_mes|Participacion % del descarte de leads de mercadeo creados en el mismo mes|=19/18|
|21|00291_descartes_dia|Descarte de leads de mercadeo generados en el mes en el ultimo dia evaluado del periodo|No aplica|
|22|00292_avg_seg_creados_dia|Promedio de leads entregados por mercadeo por dia habil (depende de la atraccion de leads por parte de mercadeo y la conexion de los asesores a franja)|No aplica|


### Keywords del dataset a tener en cuenta

- `Leads`:  Oportunidades de venta (prospectos) generados por mercadeo.
- `Seguimiento`: En el CRM los Leads son creados como seguimientos.
- `Seguimiento atrasado`: Todo seguimiento esta compuesto por una fecha de compromiso de contacto, cuanto esta vence, se contabiliza el seguimiento como atrasado en el dia.
- `Descarte`: Los seguimientos pueden ser cerrados por multiples motivos, Ej. No hay interes, No hay dinero, El producto no es lo que busca, etc.
- `Franja`: Horarios del dia en los que los asesores son organizados para conectarse al marcador telefonico y recibir nuevas oportunidades (Leads).
