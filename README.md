<p align='center'>
<img src ="https://media.istockphoto.com/id/1211804890/es/foto/buenos-aires-skyline.jpg?s=612x612&w=0&k=20&c=U1l5amCp1qAPQvnE5ji7y2Nqx3WX5zDTODDOrMka0I0=">


<h3 align=center> Proyecto Individual Nº2: "SINIESTROS VIALES" </h3>
 
## Introducción

Ahora si! Manos a la obra! :muscle:

Para este segundo proyecto indivudual de HENRY tuve que establecer un rol como DATA ANALYST y trabajar con un dataset propuesto.
Realicé una lectura de los datos, limpieza de la información y armado de dashboard, sumado a información acerca de factores de riesgo que aporte yo y creo aporta valor al análisis.

Espero que el desarrollo del presente proyecto le resulte intuitivo y ameno al lector. 😄


## Marco teórico acerca de Siniestros Viales

Primero comparto la definición de lo que es un siniestro vial:

*Los **`siniestros viales`** 🚗, también conocidos como accidentes de tráfico o accidentes de tránsito, son eventos que involucran vehículos en las vías públicas y que pueden tener diversas causas, como colisiones entre automóviles, motocicletas, bicicletas o peatones, atropellos, choques con objetos fijos o caídas de vehículos. Estos incidentes pueden tener consecuencias que van desde daños materiales hasta lesiones graves o fatales para los involucrados.*

Los datos a procesar corresponden a información aportada por la Secretaria de Transporte de la Ciudad Autonoma de Buenos Aires, en el cual se detallada la cantidad de homicidios y lesiones en siniestros viales durante un lapso de tiempo.

Se toma como referecia dicha ciudad debido al volumen de trafico diario que maneja y población que contiene, siendo más propenso a sufrir accidentes en todo su territorio. Al ser la pricipal ciudad de Argentina, el Gobierno pone foco en las tasas de mortalidad relacionada con siniestros viales y desarrollar politicas para su disminución para mejorar la calidad de vida de las personas, sean argentinas o extranjeros. Por tal motivo el seguimiento de las estadísticas y la implementación de políticas efectivas son esenciales para alcanzar objetivos propuestos.

Los informes del Sistema Nacional de Información Criminal (SNIC), del Ministerio de Seguridad de la Nación, revelan que entre 2018 y 2022 se registraron 19.630 muertes en siniestros viales en todo el país. Estas cifras equivalen a 11 personas por día que resultaron víctimas fatales por accidentes de tránsito.

Solo en 2022, se contabilizaron 3.828 muertes fatales en este tipo de hechos. Los expertos en la materia indican que en Argentina es dos o tres veces más alta la probabilidad de que una persona muera en un siniestro vial que en un hecho de inseguridad delictiva.


## Información adicional acerca de Factores de Riesgo

Como en nuestra vida cotidiana es usual que tengamos que trasladarnos de un lado a otro, es importante conocer que estamos expuestos a todo tipo de riesgos viales que pueden concatenar en un accidente.

Para los accidentes viales hay 3 factores de riesgo: el medio ambiente, la máquina y el hombre. Dicho trío es conocido como *"El triángulo accidentológico"*

+ **`El medio ambiente`**: representa el 2% de los factores causales en accidentes viales. Contituído por las condiciones meteorológicas y las condiciones del camino en sí, que dificulten la maniobrabilidad.

+ **`La máquina`**: representa el 3% de los factores causales en accidentes viales. Hace referencia a la herramienta mecánica o automotriz que es utilizado como medio de transporte por parte del usuario. El vehículo dentro de su estructura cuenta con ciertos componentes que contribuyen a evitar o mitigar los resultados de un accidente de tránsito, estos se pueden clasificar como elementos de seguridad vial activa y elementos de seguridad vial pasiva; por ejemplo frenos ABS y cinturones de seguridad, respectivamente.

+ **`El hombre`**: representa el **`95%`** de los factores causales en accidentes viales. Corresponden al accionar o hábitos del conductor que interrumpen la correcta conducción de la unidad utilizada. Formar e informar al usuario es vital para que adopte valores permanentes desde el conocimiento.

En esta instancia ampliare información con la suministrada por la Secretaria de Transporte acerca de estudios observacionales de factores de Riesgo Vial en CABA en un periodo de tiempo, tanto para automóviles como para motos.


## Proyecto a desarrollar 

La finalidad del proyecto es la elaboración de un proyecto de anális de datos, con el fin de generar información que permita a las autoridades locales tomar medidas para disminuir la cantidad de víctimas fatales de los siniestros viales.

Para ello, disponemos de un dataset sobre homicidios en siniestros viales ocurridos en la Ciudad de Buenos Aires durante el periodo 2016-2021. Este dataset se encuentra en formato *xlsx* y contiene dos hojas llamadas: **hechos** y **víctimas**. 

Adicionamente trabajaremos tambien con un dataset acerca de lesiones en siniestros viales en el periodo 2019-2021, y dos datasets con observaciones de factores de riesgos viales en automóviles y motos durante dos meses del año 2022.


## Etapas de desarrollo

+ `Descarga de datos`⏬:
  Descarga y almacenamiento de los datasets mencionados en su formato original en la carpeta "01 - Datasets".

+ `ETL`📝:
  Mediante dos archivos júpiter ".ipynb" procedí a la lectura de los datos, selección de aquellas columnas que sean de interés para su análisis, segregación de las mismas, cruce de tablas para facilitar su tratamiento y conversión de los datos en un archivo tipo ".csv", con nomenclaturas que inician con "Datos_".

+ `EDA`📖:
  Realicé el análisis exploratorio de datos en un archivo júpiter ".ipynb", en el cual realicé la busqueda de valores faltantes, valores atípicos, eliminación de registros duplicados, visualización de datos, correlación entre variables, conclusiones a priori.

+ `Dashboard`🎨:
  Mediante el uso de 5 páginas, implemente interactivamente la interpretación gráfica de los datos para su fácil lectura y que acompañe al storytelling a desarrollar durente la presentación del proyecto.
  Como lo datos de Lesiones corresponden al período de 2019-2021, decidí tomar dicho periodo para el análisis de Homicidios y realizar una comparativa de cantidad de accidentes.
  También tener en cuenta que los datos de factores de riesgo corresponden a los meses de Octubre y Noviembre 2022. Si bien es un corto periodo de análisis, esa muestra permite ayudarnos a ver la incidencia de distracciones en el día a día de la población.


## Contenido de archivos

Dentro de github se encuentran los siguientes archivos/carpetas:

+ 01 - Datasets: Contiene los archivos originales extraidos desde la web; compuesto por una carpeta con los siniestros viales y otra carpeta con los factores de riesgo

+ Datos_FR_Autos.csv: Archivo procesado que contiene los factores de riesgo observados en el manejo de automóviles. Está compuesto por las columnas Año, Mes, Dia hábil, Turno, Zona, Antiguedad, Tipo de distracción y Protección total (uso de cinturón por todos los pasajeros)

+ Datos_FR_Motos.csv: Archivo procesado que contiene los factores de riesgo observados en el manejo de motos. Está compuesto por las columnas Año, Mes, Dia hábil, Turno, Zona, Antiguedad, Tipo de distracción y Uso de casco (uso de casco por todos los pasajeros)

+ Datos_Homicidios.csv: Archivo procesado que contiene información de la cantidad de victimas fatales en siniestros viales. Está compuesto por las columnas ID, Año, Mes, Dia, Lugar, Calle principal, Calle secundaria, número de Comuna, Longitud, Latitud, Victima, Acusado, Rol de la Victima, Sexo, Edad, Fallecido.

+  Datos_Lesiones.csv: Archivo procesado que contiene información de la cantidad de victimas fatales en siniestros viales. Está compuesto por las columnas ID, Año, Mes, Dia, Lugar, número de Comuna, Victima, Sexo, Edad, Gravedad.

+  EDA.ipynb: todo el proceso de análisis exploratorio de datos realizado para proceder con su presentación en una herramienta gráfica, la cual en este caso fue POWER BI

+  ETL_Riesgo.ipynb: Archivo júpiter con los pasos detallados en la lectura de los archivos originales de factores de riesgo, limpieza de datos y porterior almacenamiento a csv.

+  ETL_Siniestros.ipynb: Archivo júpiter con los pasos detallados en la lectura de los archivos originales de siniestros viales, limpieza de datos, cruce de información y porterior almacenamiento a csv.

+  Siniestros Viales CABA.pbix: archivo de POWER BI en el cual se encuentra plasmado todo el desarrollo de visualización de la información e indicadores


## Análisis de los datos

Como conclusiones generales en la visualización de los datos del dashboard, tenemos:

+ 24475 accidentes registrados durante el periodo 2019-2021, los cuales tuvieron 715 víctimas fatales. Para dicho período, los accidentes ocurren en mayor frencuencia entre los meses de noviembre a enero, los fines de semana  y en una franja horaria entre las 05 AM hasta las 9AM.

  🙋‍♂️**Propuesta para su mitigación**: `INCREMENTAR` los recursos necesarios para el control de transito en esa franja horaria, ya que en día hábil corresponde al traslado de las personas a lugares de trabajo, y los fin de semana a salidas de boliches/bares. Con respecto a los meses, `INVESTIGAR` su origen; puede que se deba a época de movimiento turístico, fechas escolares, variación de frecuencias de servicios de transporte, por mencionar algunos. `REALIZAR` campañas publicitarias al respecto, mencionando valores de forma tal invitar a la comunicar ser concientes de cantidad de víctimas fatales.

+ De 715 víctimas fatales en accidentes viales, 42% la víctima se trasladaba en moto y 37% la víctima era peatón. El 62% de los accidentes ocurrieron en Avenidas y un 20% en calle/cruce, dejando en monoría autopistas o vias de acceso principal a la ciudad.
  Las comunas 1, 4, 7, 8 y 9 (zona este y sur) representan los lugares donde los accidentes tienen mayor frecuencia.

  🙋‍♂️**Propuestas para su mitigación**: determinar zonas donde se trasladaban las victimas en moto y peatón y `INVESTIGAR` si existe falta de señalización, problemas del camino, falta iluminación, por mencionar algunos; en caso de su ausencia, `DESTINAR` recursos para su mejoría. Con respecto a accidentes en avenidas y calles/cruces, investigar lo mismo.

  Las comunas 1 y 4 son zonas de mucho tránsito vehicular (comercios, entidades estatales, empresas), y al conectarse con las comunas 7, 8 y 9, nos puede indicar que las vias de conexión entre ambas zonas puede ser deficiente para el tránsito y existir puntos de riesgo donde se produzcan esos accidentes. Lo correcto es `INVESTIGAR` más en detalle y `DESTINAR` recursos para una mejoría.

+ De un total de 9403 observaciones de factores de riesgo, el uso de celular representan la mayor distracción tanto en autos como en motos. 40% de los datos registrados en automóviles no registraban el uso de cinturón de seguridad por TODOS sus ocupantes, lo cual llama mucho la atención; y el 13% de datos en categoria motos no registraban el uso de casco por TODOS sus ocupantes.

  🙋‍♂️**Propuestas para su mitigación**: Como es elevado el porcentaje de personas que usan el celular mientras conducen, es conveniente incrementar la `SEVERIDAD` de las multas por su uso, asi tambien la cantidad de unidades de control. `CONCIENTIZAR` a la comunidad en el uso de cinturón de seguridad por todos los pasajeros y uso de casco para pasajeros de motos, sin evitar compartir las consecuencias de su ausencia. `ANALIZAR` si existe una relación de dichas observaciones con las zonas donde ocurren los accidentes, ya que se podría abarcar mas focos de riesgo.


## KPIs

El proyecto solicitaba el desarrollo de 2 KPIs:

+ *Reducir en un 10% la tasa de homicidios en siniestros viales de los últimos seis meses, en CABA, en comparación con la tasa de homicidios en siniestros viales del semestre anterior*.
  
  Definimos a la **tasa de homicidios en siniestros viales** como el número de víctimas fatales en accidentes de tránsito por cada 100,000 habitantes en un área geográfica durante un período de tiempo específico.
  Su fórmula es: (Número de homicidios en siniestros viales / Población total) * 100,000

  ⬇️**Redujo en un 15% aproximadamente dicha tasa, respecto al semestre anterior**😄 **`CUMPLE`**
  
+ *Reducir en un 7% la cantidad de accidentes mortales de motociclistas en el último año, en CABA, respecto al año anterior*.
  
  Definimos a la **cantidad de accidentes mortales de motociclistas en siniestros viales** como el número absoluto de accidentes fatales en los que estuvieron involucradas víctimas que viajaban en moto en un determinado periodo temporal.
  Su fórmula para medir la evolución de los accidentes mortales con víctimas en moto es: (Número de accidentes mortales con víctimas en moto en el año anterior - Número de accidentes mortales con víctimas en moto en el año actual) / (Número de accidentes mortales con víctimas en moto en el año anterior) * 100

  ⬆️**Creció 76% aproximadamente la cantidad de víctimas fatales de motociclistas, respecto al año anterior**☹️ **`NO CUMPLE`**

Como tercer indicador se propone:

+ *Incrementar en un 5% la relación de uso de cinturon de seguridad en el automóvil (por todos los pasajeros) del ultimo mes, respecto al anterior*.

  Defino la relación de uso de cinturon de seguridad como: (Cantidad de observaciones de automoviles CON uso de cinturón de seguridad) / (Cantidad de observaciones de automoviles SIN uso de cinturón de seguridad), en un periodo de tiempo. Mientras más alto el valor, se observa más la presencia de cinturón por todos los pasajeros.

  ⬇️**Disminuyó 0,14% aproximadamente la relación de uso de cinturon en el automóvil, respecto al mes anterior**☹️ **`NO CUMPLE`**


## Fuente de datos

- [Buenos Aires Data](https://data.buenosaires.gob.ar/dataset/victimas-siniestros-viales): dataset denominado `Homicidios`.

- [Buenos Aires Data](https://data.buenosaires.gob.ar/dataset/victimas-siniestros-viales): dataset denominado `Lesiones`.

- [Buenos Aires Data](https://data.buenosaires.gob.ar/dataset/estudio-observacional-factores-riesgo-vial): datasets denominados `Automóviles` y  `Motovehículos`.

- [Factores de riesgo viales](https://www.linkedin.com/pulse/qu%C3%A9-es-el-tri%C3%A1ngulo-accidentol%C3%B3gico-factores-de-y-mocondino-r-/?originalSubdomain=es): información acerca de factores de riesgo y triángulo de accidentología.

- [Censo 2022 CABA](https://www.indec.gob.ar/indec/web/Nivel4-Tema-2-41-165): Datos de censo nacional realizado en el año 2022.
