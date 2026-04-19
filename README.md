# sprint7-final-project
telecom-analysis
# Análisis de Comportamiento de Usuarios y Uso de Servicios

## Descripción del proyecto

Este proyecto analiza el comportamiento de usuarios en una plataforma de telecomunicaciones, integrando datos de uso (llamadas y mensajes) con información demográfica para identificar patrones de actividad y segmentar usuarios según su nivel de uso.

El objetivo principal es entender cómo interactúan los usuarios con los servicios y detectar diferencias entre planes, lo que permite generar insights accionables para negocio.

##  Objetivos

* Analizar el uso de llamadas y mensajes por usuario
* Identificar patrones de comportamiento y distribución
* Detectar valores atípicos (outliers)
* Segmentar usuarios según nivel de uso (bajo, medio, alto)
* Comparar comportamiento entre planes (Básico vs Premium)

## Datos utilizados

### 1. Users

* `user_id`
* `age`
* `city`
* `reg_date`
* `plan`

### 2. Usage

* `user_id`
* `type` (call / text)
* `duration`
* `length`


##  Procesamiento de datos

###  Limpieza

* Reemplazo de valores sentinels.
* Conversión de fechas a formato datetime
* Eliminación de fechas futuras
* Validación de tipos de datos y consistencia

## Análisis exploratorio (EDA)

### Distribución de variables

* Histogramas para:

  * edad
  * cantidad de mensajes
  * cantidad de llamadas
  * comparación entre planes
  * segmentación por tipo de uso y edad.

###  Outliers

* Detección mediante método IQR

##  Insights principales

* Los adultos son el grupo de edad mas importante para la empresa, seguido de los adultos mayores.
* EL numero de mensajes incluidos en el plan básico es muy alto comparado con el promedio de mensajes usados por los usarios, en cuestion de llamadas, lo usuarios con mas llamadas realizadas son 12 mientras que la duración promedio es de 20min, una combinación que en los usuarios que se cumplen es el doble de los minutos del plan básico pero muy por debajo del plan premium.




