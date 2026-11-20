# Práctica 1 — Leer y personalizar código M en Power Query

## Objetivo
Explorar la estructura `let ... in` del lenguaje M y modificar manualmente una consulta de Power Query luego de realizar transformaciones desde la interfaz de Power BI Desktop.

## Dataset
**Online Retail**, UCI Machine Learning Repository.

Fuente: https://archive.ics.uci.edu/dataset/352/online-retail

Se eligió por contener datos de transacciones con columnas de texto, cantidades, precios y fechas, además de valores ausentes e identificadores técnicos que permiten practicar transformaciones reales.

## Transformaciones realizadas
1. Convertir `InvoiceDate` al tipo `datetime`.
2. Renombrar `UnitPrice` como `precio_unitario`.
3. Conservar únicamente las filas con `Quantity > 0`.

En el Editor avanzado se renombró un paso como `MiTransformacionManual`, se incorporó un comentario `//` y se actualizó la referencia del paso posterior.

## Archivos del repositorio
- `Practica_1_Lenguaje_M.pdf`: documentación, código M y explicaciones.
- `Practica 1 - Lenguaje M.pbix`: proyecto de Power BI Desktop (nombre sujeto a cómo se guardó localmente).

## Nota sobre la fuente de datos
El `.pbix` se creó con un Excel descargado localmente. Para actualizar los datos en otra computadora, se debe descargar el archivo original de la fuente indicada y configurar de nuevo la ruta desde **Configuración de origen de datos** en Power BI Desktop.
