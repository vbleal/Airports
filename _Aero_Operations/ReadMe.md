# Aeropuertos - Operaciones y Pasajeros



Creado por:

*  **V. D. Betancourt**


<img src="https://github.com/vbleal/Airports/blob/main/_Aero_Operations/Imag/DE_Aero_Op.png" width="500" height="300">

<sub>Créditos: Imagen Generada con IA.</sub>




<br>

---

## 📃 Introducción


<details>
<summary>Expandir </summary>

<br>


### 🎯 Objetivo


El presente proyecto tiene por objetivo analizar los **datos operativos** presentados en distintos aeropuertos, lo cual incluye operaciones comerciales y generales, así como el flujo de pasajeros, el número de aerolíneas, y los destinos nacionales e internacionales. 

Adicionalmente, se propone un modelo para obtener **predicciones** sobre el comportamiento de esta operativa. Dicho modelo está basado en **Redes Neuronales (Neural Networks)**.


<br>

### 📄 Descripción

El análisis de la operativa en distintos aeropuertos depende de la información disponible y la calidad de la misma.

En ese proyecto se han creado **datos sintéticos** que constan de **11 variables (columnas)**, para un período parametrizable de fechas mensuales.


  
</details>





<br>

---
## 🧪 Generación de Datos Sintéticos

<details>
<summary>Expandir </summary>

<br>

Se creará un dataset llamado **`datos_aeropuertos.csv`**, que contendrá **"datos sintéticos"** (generados aleatoriamente) con los siguientes 11 campos (columnas):

* **`'fecha'`**: Es la fecha de cada registro (fila) que comprenderá el rango del **`'2022-03-31'`** al **`'2024-03-31'`**, y siempre corresponderán a las fechas del último día del mes.

* **`'nombre_aeropuerto'`**: Se refiere al nombre del aeropuerto, el cual, para simplificar este análisis, corresponderán a 12 nombres de la forma: **`'Aeropuerto_1'`**, **`'Aeropuerto_2'`**, ..., **`'Aeopuerto_12'`**.

* **`'tipo_aeropuerto'`**: Se considerarán solamente aeropuertos del tipo **`'Internacional'`**.

* **`'numero_aerolineas'`**: Será un número aleatorio entre 5 y 20 aerolíneas.

* '**`destinos_nacionales'`**: Será un número aleatorio entre 5 y 30 destinos nacionales.

* **`'destinos_internacionales'`**: Será un número aleatorio entre 1 y 10 destinos internacionales.

* **`'destinos_total'`**: Es la suma de '**`destinos_nacionales'`** y **`'destinos_internacionales'`**.

* **`'Operaciones_comercial'`**: Será un número aleatorio entre 1,000 y 50,000.

* **`'Operaciones_general'`**: Será un número aleatorio entre 100 y 5,000.

* **`'pasajeros_comercial'`**: Será un número aleatorio entre 100,000 y 5,000,000.

* **`'pasajeros_general'`**: Será un número aleatorio entre 1000 y 15,000.



  
</details>






<br>

---
## 🧮 Modelo

<details>
<summary>Expandir </summary>

<br>

🔮 [Modelo Python para Datos Sintéticos y Predicciones de Operaciones y Pasajeros en Aeropuertos](https://github.com/vbleal/Airports/blob/main/_Aero_Operations/Report/GH_Aeropuertos%20-%20Operaciones%20y%20Pasajeros.pdf)

<br>

Resumen del Modelo de Redes Neuronales (Neural Networks) empleado para la predicción del dataset de Operaciones y Pasajeros:

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_Operations/Imag/Modelo_Proy_Operaciones.png" width="500" height="300">

  
</details>






<br>

---
##  📊 Resultados

<details>
<summary>Expandir </summary>

<br>


* **Operaciones Comerciales por Mees**

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_Operations/Imag/Operaciones_Comerciales_Subplots_Meses.png" width="700" height="500">

<br>
<br>






* **Operaciones Comerciales Outliers**

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_Operations/Imag/Operaciones_Comerciales_Outliers.png" width="700" height="500">

<br>
<br>




* **Operaciones Comerciales Tendencia**

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_Operations/Imag/Operaciones_Comerciales_Tendencia.png" width="700" height="500">

<br>
<br>





* **Pasajeros Comerciales por Mes**

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_Operations/Imag/Pasajeros_Comerciales_Subplots_Meses.png" width="700" height="500">

<br>
<br>






* **Pasajeros Comerciales Tendencia**

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_Operations/Imag/Pasajeros_Comerciales_Tendencia.png" width="700" height="500">

<br>
<br>







* **Pronóstico Operaciones Comerciales**

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_Operations/Imag/Forecast_Operaciones_Comerciales.png" width="700" height="500">







  
</details>








<br>

---
## 💼 Documentación

<details>
<summary>Expandir </summary>

<br>

🔮 [Modelo Python para Datos Sintéticos y Predicciones de Operaciones y Pasajeros en Aeropuertos](https://github.com/vbleal/Airports/blob/main/_Aero_Operations/Report/GH_Aeropuertos%20-%20Operaciones%20y%20Pasajeros.pdf)

  
</details>


<br>

---
