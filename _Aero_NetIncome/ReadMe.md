# Aeropuertos y Combustibles: Ingresos y Gastos

Ingresos, Gastos, Aeropuertos, Combustibles, Pronóstico

Creado por:

*  **V. D. Betancourt**


<img src="https://github.com/vbleal/Airports/blob/main/_Aero_NetIncome/Imag/DE_Aero_Income.png" width="500" height="300">

<sub>Créditos: Imagen Generada con IA.</sub>





<br>

---

## 📃 Introducción


<details>
<summary>Expandir </summary>

<br>


### 🎯 Objetivo

El objetivo del presente proyecto consiste en realizar proyecciones de Ingresos y Gastos para Aeropuertos y Combustibles en distintos aeropuertos.



<br>

### 📄 Descripción

Este proyecto permite generar **datos sintéticos** para los Ingresos y Gastos correspondientes a Aeropuertos y Combustibles que sirvan como datos de entrada para la generación de las **Proyecciones**.

En caso de que los **datos reales** estuviesen disponibles, se podrán introducir en el Modelo (VBA-Excel) para que genere las respectivas predicciones, respetando la estructura de datos (combinaciones y columnas) que se asume en los datos sintéticos.


  
</details>





<br>

---
## 🧪 Generación de Datos Sintéticos

<details>
<summary>Expandir </summary>

<br>

Los **datos sintéticos** generados constan de **15 variables (columnas)**, que son:

* **`'Fecha'`**: Son fechas parametrizables mensuales, en este caso, generadas para el período: **`'2023-01-31'`** al **`'2024-03-31'`**. Cabe señalar que para generar predicciones, el modelo requerirá contar con al menos 2 fechas históricas.

* **`'División'`**: Son 2 categorías: **`'Aeropuertos'`** y **`'Combustibles'`**.

* **`'Concepto'`**: Son 2 categorías para cada **`'División'`**: '**`Ingresos Cobrados'`** y **`'Gastos'`**.

* **`'Subconcepto'`**: Son categorías que dependen de la **`'División'`** y el **`'Concepto'`**.

  - Para Aeropuertos e Ingresos cobrados: **`'Arrendamiento', 'Servicios Aeroportuarios', 'Tarifa de Uso Aeroportuario (TUA)'`**  

  - Para Aeropuertos y Gastos:  **`'Servicios Personales', 'Materiales' `** 

  - Para Combustibles e Ingresos Cobrados: **`'Almacenamiento', 'Expendio'`**  

  - Para Combustibles y Gastos: **`'Servicios Personales', 'Materiales', 'Servicios Generales'`** 

* **11 columnas** más correspondientes a los nombres de cada aeropuerto.

  - Se ha creado un catálogo (diccionario) para los nombres de los aeropuertos (**`'nombres_aropuertos'`**) con la flexibilidad de poder adecuarlo con los nombres reales cuando se tenga dicha información.
 

<br>

**Tabla de Ejemplo de los Datos Sintéticos**:

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_NetIncome/Imag/Datos_Sintéticos_Ene-Mar.png" width="1000" height="600">




  
</details>





<br>

---

## 🧮 Modelo

<details>
<summary>Expandir </summary>

<br>


🔮 [Modelo VBA-Excel de Predicciones de Ingresos y Gastos para Aeropuertos y Combustibles](https://github.com/vbleal/Airports/blob/main/_Aero_NetIncome/Report/Proyecciones%20Ingresos%20y%20Gastos%20para%20Aeropuertos%20y%20Combustibles.pdf)

<br>

🐍 [Modelo Python para Generar Datos Sintéticos de Ingresos y Gastos para Aeropuertos y Combustibles](https://github.com/vbleal/Airports/blob/main/_Aero_NetIncome/Report/Aeropuertos%20y%20Combustibles%20-%20Ingresos%20y%20Gastos.pdf)



  
</details>






<br>

---
##  📊 Resultados

<details>
<summary>Expandir </summary>

<br>



<details>
<summary>AEROPUERTOS </summary>

<br>

### Aeropuertos - Ingresos Cobrados

#### Gráfico de Barras

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_NetIncome/Imag/Aeropuertos_Ingresos_Barras.png" width="900" height="700">


#### Boxplots y Outliers

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_NetIncome/Imag/Aeropuertos_Ingresos_Outliers.png" width="900" height="700">


### 🔮 Proyecciones

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_NetIncome/Imag/Aeropuertos_Ingresos_Proyecciones_DatosSintéticos.png" width="1700" height="300">




<br>
<br>

### Aeropuertos - Gastos

#### Gráfico de Barras

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_NetIncome/Imag/Aeropuertos_Gastos_Barras.png" width="900" height="700">

#### Boxplots y Outliers

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_NetIncome/Imag/Aeropuertos_Gastos_Outliers.png" width="900" height="700">


### 🔮 Proyecciones

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_NetIncome/Imag/Aeropuertos_Gastos_Proyecciones_DatosSintéticos.png" width="1700" height="300">






</details>





<br>


<details>
<summary>COMBUSTIBLES </summary>

<br>

### Combustibles - Ingresos Cobrados

#### Gráfico de Barras

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_NetIncome/Imag/Combustibles_Ingresos_Barras.png" width="900" height="700">

#### Boxplots y Outliers

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_NetIncome/Imag/Combustibles_Ingresos_Outliers.png" width="900" height="700">


### 🔮 Proyecciones

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_NetIncome/Imag/Combustibles_Ingresos_Proyecciones_DatosSintéticos.png" width="1700" height="200">




<br>
<br>

### Combustibles - Gastos

#### Gráfico de Barras

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_NetIncome/Imag/Combustibles_Gastos_Barras.png" width="900" height="700">

#### Boxplots y Outliers

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_NetIncome/Imag/Combustibles_Gastos_Outliers.png" width="900" height="700">


### 🔮 Proyecciones

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_NetIncome/Imag/Combustibles_Gastos_Proyecciones_DatosSintéticos.png" width="1700" height="200">




</details>

  
</details>








<br>

---
## 💼 Documentación

<details>
<summary>Expandir </summary>

<br>

🔮 [Modelo VBA-Excel de Predicciones de Ingresos y Gastos para Aeropuertos y Combustibles](https://github.com/vbleal/Airports/blob/main/_Aero_NetIncome/Report/Proyecciones%20Ingresos%20y%20Gastos%20para%20Aeropuertos%20y%20Combustibles.pdf)

<br>

🐍 [Modelo Python para Generar Datos Sintéticos de Ingresos y Gastos para Aeropuertos y Combustibles](https://github.com/vbleal/Airports/blob/main/_Aero_NetIncome/Report/Aeropuertos%20y%20Combustibles%20-%20Ingresos%20y%20Gastos.pdf)

  
</details>


<br>

---
