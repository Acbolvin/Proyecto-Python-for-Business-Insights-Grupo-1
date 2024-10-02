# Proyecto-Python-for-Business-Insights-Grupo-1
Predecir la variable churn de una muestra del tercer trimestre de un conjunto de datos de Telecomunicaciones 

Las variables que se excluyeron fueron las siguientes:

   Zip Code porque no es pertinente para el caso de estudio sobre la tasa de abandono del servicio.
   Longitude no se necesita para la variable predicción churn.
   Population no se busca proyectar la población por codigo postal.
   Customer ID se elimina esta columna ya que su codificación atrasaria al modelo para que realice las predicciones porque son muchos clientes.
   Country y State no hay diferencias significativas en el servicio entre estados o países.
   Quarter porque todos los clientes tienen el mismo trimestre del año que es el tercero.

  En la variable Offer existe una categoría llamada 'None' la cual no aparece en la data a pesar de que se especifica que forma parte en el diccionario de la misma, por lo que se asume que 'None' representa los valores nulos de este feature. Y se procede a reemplazar "None" en los nulos.
  (Offer
 No         3877
 Offer B     824
 Offer E     805
 Offer D     602
 Offer A     520
 Offer C     415
 Name: count, dtype: int64,
 Internet Type
 Fiber Optic    3035
 DSL            1652
 No             1526
 Cable           830
 Name: count, dtype: int64)

Como se observa en el código de abajo se solucionó el problema de los nulos y los únicos valores que quedaron con nulos son aquellos que no se incluyeron para el estudio por parte de la misma data.

El objetivo es minimizar los falsos positivos y asegurarse de que las predicciones negativas sean correctas
![imagen](https://github.com/user-attachments/assets/3f154856-4714-4643-94a6-368f04c612ff)


En el sector de telecomunicaciones, el costo promedio de adquisición de clientes (CAC) es de aproximadamente $694 USD.

![imagen](https://github.com/user-attachments/assets/87e6acba-dc38-4746-96f0-9baa95b49e02)

True Negative (TN): La empresa ha ahorrado o evitado costos por un valor de $3,086,051 USD, ya que estos clientes no abandonaron y no fue necesario gastar dinero para retenerlos o adquirir nuevos clientes.

False Negative (FN): Este valor es crítico, ya que la empresa no identificó a estos clientes como en riesgo de churn, lo que resultó en $153,662 USD en costos de adquisición para reemplazar a los clientes que abandonaron. 
Reducir los falsos negativos debería ser una prioridad para disminuir estos costos.

True Positive (TP): La empresa pudo haber evitado un costo de $185,992 USD, ya que identificó correctamente a los clientes en riesgo de churn y probablemente aplicó estrategias para retenerlos.

Pese a los gastos mensuales de marketing por mantener a mis clientes leales me queda una ganancia de $224.162





