# Clima-Bogota-Oct-2018-Sept-2019

 Analisis a la información sobre el clima de la ciudad de Bogota Colombia en el periodo del mes de Octubre 2018 a  el mes de septiembre de 2019.


         # Como Instalar
clonar o descargar el repositorio
 ``` git clone [repo] ```
copiar y pegar el contenido en una carpeta utilizar
* NodeJS-> ejecutar comando live-server en la carpeta con los archivos
* Python-> ejecutar el comando python -m http.server en la carpeta con los archivos


Ejecutar la aplicación desde el explorador

# Tecnologias usadas
* D3 V5
* Api de darksky.net

# **_Insight:_** :shipit:
* El 10 de Marzo de 2019 se registro un pico de temperatura de 92 grados farenheit equivalente a 33 grados celcius una cifra muy alta para el promedio de de temperatura de Bogota de 22 grados celcius.

* La mayor parte del año el indice de UV que representa la intensidad de radiacion ultra violeta en la ciudad de Bogota es mayor o igual a 8 lo cual puede llevar producir lesiones en la piel de los Bogotanos.



# De donde vienen los Datos

Los datos provienen de https://darksky.net/forecast/4.6355,-74.0877/us12/en , se usa la api para obtener los datos de los 365 dias, se usa el archivo get_weather_data.py utilizando los valores de longitud y latitud de bogota.

# What
Dataset Availability: Static

Data Types: Table -> Items -> Attributes

Data and Dataset Types: Temporal

Dataset Types: Temporal

_Attributes:_

| item   |      Type      |  Description |
|----------|:-------------:|------:|
| TemperatureMin |  ordered -> cuantitativo divergente | La temperatura minima registrada en el dia en la ciudad de Bogota |
| TemperatureMax|    ordered->cuantitativo divergente   |   La temperatura maxima registrada en el dia en la ciudad de Bogota |
| UvIndex | ordered->cuantitativo secuencial |  Medicion de la radiacion ultra violeta en la ciudad de bogota |
| PrecipProbability | ordered->cuantitativo secuencial |    valor de la probabilidad de lluvias(rain)/aguanieve(sleet)/nieve(snow) |
| Date | ordered->cuantitativo secuencial |  Fecha del dia donde se toman las mediciones ciudad de Bogota |

# Why

Tarea principal: ¿Que días fueron los más calurosos y los más fríos en bogotá?(Locate Outliers)

Tarea secundaria:¿Qué época del año es más nublada y se correlaciona con los días más fríos?(Compare-correlation)

Tarea secundaria:¿Los días nublados tienen índices UV más bajos o son más lluviosos?(Identify-features)

Tarea secundaria:¿Cómo varía el clima cada mes?(Compare-Trends)

Tarea secundario:Como ha sido el clima en la ciudad de bogotá desde octubre del año pasado a finales de septiembre de este año(summarize-trends)



# How
Idiom :Radar Chart

# Marcas
*Área -> Temperatura Minima y maxima en Bogota

*Lines -> Identificador de uvIndex arriba de 8

# Canales
*color saturation->Temperatura Minima y maxima en Bogota

*colorhue-> Precipitacion y Cobertura de las nuves

*shape->Uv Index
