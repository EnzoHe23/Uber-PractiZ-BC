# Proyecto Especial: Análisis a empresa Uber (21/09 - 05/10)

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
5. [📂 Ingresar al análisis en código 📂](#-ingresar-al-análisis-en-código-)

## 📰 Acerca del proyecto 📰

El proyecto fue realizado durante el bootcamp "Data Analytics for Business". Como proyecto final, se tuvo que generar datasets con información variada de valor para Uber, como los clientes y viajes hechos, por ejemplo, y después analizarlos en un dashboard para obtener hallazgos que puedan ayudar a mejorar las ganancias de la empresa.

Para generar los datos, utilizamos en su mayoría archivos de Google Sheets, con ayuda de funciones que mantengan los datos inicialmente en un estado aleatorio, para luego dejar los datos estáticos; en el caso de tablas como la tabla "Hechos", las generamos en archivos Excel con ayuda de ChatGPT, y tras unos retoques los subimos como archivos de Google Sheets.

La visualización de datos final fue hecha con ayuda de un dashboard en Power BI.

*(Los datos de la empresa Uber fueron generados artificialmente, así que no hay información confidencial en juego)*

Las tablas creadas son las siguientes:

- Clientes: Información de los clientes de Uber. Incluye por cada uno su código, DNI, edad, número de celular, distrito y provincia, nombre completo, estado, y última fecha activa.
- Conductores: Información de los conductores: Incluye por cada uno su código, DNI, edad, fecha de ingreso y de última carrera, número de celular, nombre completo, estado, y código del tipo de auto.
- Tipo de Auto: Información de los autos que utiliza la empresa. Incluye por cada uno su código, marca, modelo, y color.
- Medio de pago: Lista de los medios de pago. Incluye solamente códigos y nombres de los medios de pago.
- Precios: Lista de precios por distancia y horario. Incluye éstos dos últimos, junto al precio y al código respectivo.
- Hechos: Información conjunta de todas las tablas anteriores. Representa los viajes hechos con el servicio de Uber desde agosto del 2023 hasta agosto del 2024.
- Metas: Lista de monto transaccionado a alcanzar (meta) por cada mes y por cada año.

