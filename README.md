# Proyecto Especial: Análisis a Uber Priority (12/09 - 05/10)

### Dashboard

[![Javascript](https://img.shields.io/badge/Clic%20para%20abrir-Power%20BI%20dashboard-yellow.svg)](https://app.powerbi.com/view?r=eyJrIjoiN2UxMjdlZTEtNTI4Yy00Zjg5LWJkODYtNmJlYTIzMjc2MGZjIiwidCI6IjBlMGNiMDYwLTA5YWQtNDlmNS1hMDA1LTY4YjliNDlhYTFmNiIsImMiOjR9)

Haga clic en el badge de arriba ('Clic para abrir Power BI dashboard'). Si no le funciona el link, puede hacer click en el enlace resaltado para entrar al [dashboard en Power BI](https://app.powerbi.com/view?r=eyJrIjoiN2UxMjdlZTEtNTI4Yy00Zjg5LWJkODYtNmJlYTIzMjc2MGZjIiwidCI6IjBlMGNiMDYwLTA5YWQtNDlmNS1hMDA1LTY4YjliNDlhYTFmNiIsImMiOjR9) del análisis.

### OJO: Tabla "Hechos"

[![Javascript](https://img.shields.io/badge/Clic%20para%20abrir-Tabla%20"Hechos"-darkgreen.svg)](https://docs.google.com/spreadsheets/d/1pkTw3qGlKyNZaqCL80ctQxo8Yy2i45V0/edit?usp=sharing&ouid=102135868896282565138&rtpof=true&sd=true)

El dashboard también utiliza una tabla llamada "Hechos". Debido a que pesa más de 25mb, no se puede agregar en el repositorio. Para descargar dicha tabla, puede hacerlo yendo al [archivo en Google Drive](https://docs.google.com/spreadsheets/d/1pkTw3qGlKyNZaqCL80ctQxo8Yy2i45V0/edit?usp=sharing&ouid=102135868896282565138&rtpof=true&sd=true) con el enlace resaltado o al badge de arriba.

## Resumen

El proyecto busca analizar información de la empresa Uber y generar insights de valor. Para ello, se generaron datos en tablas de conductores, clientes, metas en ganancia meta por mes, etc. desde archivos Excel, Google Sheets y con ayuda de IA, y después se utilizó Power BI para elaborar un dashboard con toda la información.

## 📖 Contenidos 📖

1. [📰 Acerca del proyecto 📰](#-acerca-del-proyecto-)
2. [📃 Objetivos y preguntas 📃](#-objetivos-y-preguntas-)
3. [📊 Procedimientos 📊](#-procedimientos-)
4. [📝 Conclusiones e ideas post-análisis 📝](#-conclusiones-e-ideas-post-análisis-)
5. [💡 Campañas propuestas 💡](#-campañas-propuestas-)

## 📰 Acerca del proyecto 📰

El proyecto fue realizado durante el bootcamp "Data Analytics for Business". Como proyecto final, se tuvo que generar datasets con información variada de valor para Uber en su servicio Priority, como los clientes y viajes hechos, por ejemplo, y después analizarlos en un dashboard para obtener hallazgos que puedan ayudar a mejorar las ganancias de la empresa.

Para generar los datos, utilizamos en su mayoría archivos de Google Sheets, con ayuda de funciones que mantengan los datos inicialmente en un estado aleatorio, para luego dejar los datos estáticos; en el caso de tablas como la tabla "Hechos", las generamos en archivos Excel con ayuda de ChatGPT, y tras unos retoques los subimos como archivos de Google Sheets.

La visualización de datos final fue hecha con ayuda de un dashboard en Power BI.

*(Los datos de la empresa Uber fueron generados artificialmente, así que no hay información confidencial en juego)*

Las tablas creadas son las siguientes:

- Clientes: Información de los clientes de Uber. Incluye por cada uno su código, DNI, edad, número de celular, distrito y provincia, nombre completo, estado, y última fecha activa.
- Conductores: Información de los conductores: Incluye por cada uno su código, DNI, edad, fecha de ingreso y de última carrera (viaje), número de celular, nombre completo, estado, y código del tipo de auto.
- Tipo de Auto: Información de los autos que utiliza la empresa. Incluye por cada uno su código, marca, modelo, y color.
- Medio de pago: Lista de los medios de pago. Incluye solamente códigos y nombres de los medios de pago.
- Precios: Lista de precios por distancia y horario. Incluye éstos dos últimos, junto al precio y al código respectivo.
- Hechos: Información conjunta de todas las tablas anteriores. Representa los viajes hechos con el servicio de Uber desde agosto del 2023 hasta agosto del 2024.
- Metas: Lista de monto transaccionado a alcanzar (meta) por cada mes y por cada año.

## 📃 Objetivos y preguntas 📃

El proyecto tuvo como único objetivo hallar oportunidades de mejora para el negocio de Uber.

Hubieron 5 preguntas que se respondieron en este análisis:

1. ¿Qué porcentaje de la meta total se cumplió en realidad?
2. ¿Quiénes son los conductores que más viajes han realizado?
3. ¿Cuál es el grupo de edad que más viajes realiza con Uber Priority?
4. ¿Cuántos viajes alcanza Uber Priority a lo largo del tiempo?
5. ¿En qué horarios se genera más dinero?

## 📊 Procedimientos 📊

1) Se generaron datos en archivos de Google Sheets para las tablas de Clientes, Conductores, Medio de pago, Tipo de auto y precios.
2) Se generaron datos en archivos de Excel para las tablas de Excel y Metas.
3) Se subieron los datasets a un dashboard en Power BI y se realizaron los toques finales a los datates.
4) Se crearon dos indicadores para el análisis general.
5) Se mejoró el análisis de información mediante varios gráficos.
    1. Un mapa que muestra la ubicación de los viajes hechos con Uber Priority, con tamaños según la cantidad de viajes hechos.
    2. Un gráfico de pastel que muestra las proporciones de viajes hechos por cada grupo de edad de los clientes.
    3. Un gráfico de líneas que muestra la evolución de los viajes hechos por mes y año.
    4. Un gráfico de barras verticales que muestra el monto transaccionado total por el horario de los viajes realizados.
    5. Un gráfico de barras horizontales que muestra los 10 conductores con mayor número de viajes hechos.
    6. Un gráfico de medidor radial que muestra el porcentaje de cumplimiento de las metas en total.
6) Se realizaron 8 indicadores con ayuda de medidas DAX:
    1. Número total de viajes
    2. Número total de clientes
    3. Ganancia neta (23% del monto transaccionado)
    4. Monto transaccionado
    5. Viajes cancelados
    6. Porcentaje de conductores inactivos
    7. Porcentaje de clientes inactivos
    8. Minutos de espera promedio
7) Se agregó un texto incluyendo el número promedio de viajes hechos por cliente, dentro del gráfico de líneas.
8) Se publicó el dashboard en la web de forma pública.

## 📝 Conclusiones e ideas post-análisis 📝

1. Uber Priority alcanzó un porcentaje de cumplimiento del 93.98% durante todo el periodo. Ya que supera el 80% de cumplimiento, se puede deducir que hay buena oferta para la demanda. Se debería elaborar un plan para elevar el número de clientes.
2. Quienes más usan Uber Priority se encuentran en el grupo de Adultez Temprana. Esto se puede deber a que se encuentran en una etapa donde se más importante salir a trabajar e ir a eventos de importancia social y laboral, además de que están acostumbrados al uso de tecnología.
3. A nivel de viajes por mes en total, febrero del 2024 es el peor mes. Sin embargo, a nivel de viajes por día en promedio, ¡febrero del 2024 es el mejor mes!

## 💡 Campañas propuestas 💡

Para ver más información, puede ver nuestra [presentación en PDF](https://github.com/EnzoHe23/Uber-PractiZ-BC/blob/main/Presentaci%C3%B3n%20de%20An%C3%A1lisis.pdf).

1. Limpieza de Playas con Uber Priority

<p align="center">
  <img src="https://github.com/user-attachments/assets/f5d7aef3-301e-4112-b057-3e6465feab97" height="300" align="center"/>
</p>

- Objetivo: Incrementar el uso de Uber Priority en febrero, vinculando la campaña con actividades de impacto social durante el verano.
- Resumen: Promover la limpieza de las playas junto a organizaciones y municipios, y promocionarla por redes sociales. Junto a ello, ofrecer un descuento del 30% en viajes hacia las playas a limpiar durante los días requeridos. Esto puede mejorarse si se coordina bien con los grupos de limpieza.

2. Refiere y Gana con Uber Priority

<p align="center">
  <img src="https://github.com/user-attachments/assets/44568781-6083-4175-a11e-e2ff61abc887" height="300"/>
</p>

- Objetivo: Incentivar a los usuarios de UberPriority a referir nuevos clientes, ofreciendo viajes gratis al referidor tras alcanzar un número de referidos.
- Resumen: Los usuarios comparten un código para referir clientes. Por cada 3 clientes, el usuario gana un viaje gratis, y sólo puedo obtener 3 viajes gratis por mes. El sistema se gestionará desde la propia app, y la campaña se promocionará por correo y redes sociales.

3. Tercer Viaje con Descuento en playas y discotecas

<p align="center">
  <img src="https://github.com/user-attachments/assets/d16e8ae1-f344-4a90-8532-03d24bea8c75" height="300"/>
</p>

- Objetivo: Aumentar el número de viajes realizados con Uber Priority durante el mes de febrero, incentivando a los usuarios con un 30% de descuento en su tercer viaje a playas y discotecas.
- Resumen: Por cada 2 viajes de ida o vuelta a playas y discotecas, los usuarios obtienen un descuento del 30% en su próximo viaje. El descuento es aparte del propuesto en la primera campaña, y no es acumulable.

