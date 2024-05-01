# Aeropuertos - Locales y Rentas


Creado por:

*  **V. D. Betancourt**


<img src="https://github.com/vbleal/Airports/blob/main/_Aero_Rent/Imag/DE_Aero_Rent.png" width="500" height="300">

<sub>Créditos: Imagen Generada con IA.</sub>
  

<br>

---

## 📃 Introducción


<details>
<summary>Expandir </summary>

<br>

### 🎯 Objetivo



El objetivo del presente proyecto consiste en proponer un panorama general para la gestión de las **rentas de locales** en distintos aeropuertos. El análisis estará enfocado en:

* **Cantidad de Locales Rentados y No Rentados**

* **Montos por Locales Rentados**

* **Clientes Activos y Clientes con Pagos Atrasados**


Para ello, se ha creado un dataset con **datos sintéticos**. Sin embargo, puede llevarse a cabo con datos reales si es que se cuenta con ellos, siempre y cuando se respeten los campos requeridos, señalados en la Sección "**Descripción**" (se sugiere revisar el código o los datasets generados para corroborar los campos necesarios).



<br>

### 📄 Descripción

El análisis de la renta de locales en distintos aeropuertos depende totalmente de la información disponible. 

Los **datos sintéticos** que se proponen para este proyecto constan de **16 variables (columnas)**, algunas de las cuales contienen un catálogo de opciones posibles (que llamaremos **`'diccionarios'`**).


 
</details>


<br>

---
## 🧪 Generación de Datos Sintéticos

<details>
<summary>Expandir </summary>

<br>

Los datos sintéticos generados con código de Python, constan de 16 variables (columnas), que son:

* **`'fecha'`**: Son fechas mensuales desde el **`'2023-01-31'`** hasta el **`'2024-03-31'`**.

* **`'nombre_aeropuerto'`**: Se han creado nombres genéricos para 12 aeropuertos para efectos de este proyecto, con la flexibilidad de poder sustitiuirlos en cualquier momento por los nombres reales.

* **`'terminal'`**: Se asume que cada aeropuerto puede tener 2 terminales: **`'T1', 'T2'`**.

* **`'planta'`**: Se asume que cada aeropuerto tiene 2 pisos o plantas: **`'Baja', 'Alta'`**.

* **`'local_id'`**: Es un código alfanumérico que consta de 3 letras y 2 números (**'???-##'**), creado con una herramienta especializada.    
       
* **`'local_categoria'`**: Es la categoría principal de los locales, puediendo ser: 
  
  - **`'Transportes', 'Hoteles', 'Compras', 'Alimentos', 'Agencias de Turismo'`**.

* **`'local_subcateg'`**: Corresponde a las posibles subcategorías para cada categoría principal, pudiendo ser:

  - **`'Transportes': ['Taxis']`**,
    
  - **`'Hoteles': ['Hotel']`**,
    
  - **`'Compras': ['Duty free', 'Ropa, accesorios y zapatería', 'Regalos y souvenirs', 'Libros, revistas y música', 'Sorteos y pronósticos']`**,
    
  - **`'Alimentos': ['Comida empaquetada', 'Restaurante bar', 'Bares y cafeterías', 'Comida rápida', 'Cafetería']`**,
    
  - **`'Agencias de Turismo': ['Agencias de viaje', 'Guía de Turistas']`**

* **`'nombre_arrendatario'`**: Se ha creado un catálogo (diccionario) para los nombres de las empresas (arrendatarios) posibles para las diferentes subcategorias (**`'local_subcateg'`**).

* **`'telefono'`**: Es un número generado aleatoriamente que consta de 10 dígitos con el formato: **`'##-####-####'`**.      
       
* **`'horario'`**: Se ha creado un catálogo (diccionario) para los posibles horarios asignados a las diferentes subcategorias (**`'local_subcateg'`**).

* **`'monto_renta'`**: Es el monto del alquiler. Se asume que será un número aleatorio entre **`'50,000'`** y **`'150,000'`** pesos.

* **`'monto_renta_usd'`**: Es la conversión a dólares del **`'monto_renta'`** dado por **`monto_renta / tipo_cambio`**, con un 'tipo_cambio'=20, parametrizable.

* **`'deposito'`**: Se asume que se requiere pagar un mes de alquiler por adelantado como depósito de seguridad.

* **`'fecha_corte'`**: Esta es la fecha en la que se evalúa o determina el pago del alquiler del local.
       
* **`'fecha_pago'`**: Es la fecha en la que efectivamente se realiza el pago del alquiler.

* **`'monto_pago'`**: Es el monto real pagado en la fecha de pago. 
  
  - Si el pago se realiza en o antes de la fecha de corte (**`días_para_pago ≤ 0`**), el monto de pago es igual al monto del alquiler (**`'monto_renta'`**). 
  
  - Si el pago se hace después de la fecha de corte, se podría aplicar una deducción, reflejada en esta columna, posiblemente como un incentivo para el pago puntual o una penalidad por pago tardío.
 

Adicionalmente, algunas de las variables anteriores dependen de otras variables auxiliares:

* **`'dias_para_pago'`**: Esta columna indica el número de días de diferencia entre la fecha de corte y la fecha real en que se realiza el pago. Puede ser negativo, lo que significa que el pago se realizó antes de la fecha de corte, o positivo, lo que indica que el pago se realizó después de la fecha de corte.


  
</details>






<br>

---
## 🧮 Modelo

<details>
<summary>Expandir </summary>

<br>


Sólo se presenta un **Análisis Exploratorio de Datos (EDA)**, tanto a nivel mensual (último mes) como a nivel de evolución histórica (tendencias).

  
</details>






<br>

---
##  📊 Resultados

<details>
<summary>Expandir </summary>

<br>

* **Clientes Último Mes**

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_Rent/Imag/Clientes_Aeropuerto_Mes.png" width="700" height="500">



<br>
<br>

* **Concentración de Clientes Último Mes**

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_Rent/Imag/Concentración_Clientes.png" width="700" height="500">



<br>
<br>

* **Categorías Último Mes**

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_Rent/Imag/Categorías_Mes.png" width="700" height="500">




<br>
<br>

* **Atrasos de Clientes Último Mes**

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_Rent/Imag/Clientes_Atraso_Mes.png" width="500" height="300">




<br>
<br>

* **Evolución Locales Rentados Vista por Aeropuertos**

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_Rent/Imag/Evolución Locales Rentados Vista por Aeropuertos.png" width="700" height="500">




<br>
<br>

* **Evolución Montos por Rentas por Aeropuertos**

<img src="https://github.com/vbleal/Airports/blob/main/_Aero_Rent/Imag/Evolución Montos por Rentas Vista por Aeropuertos.png" width="700" height="500">

  
</details>








<br>

---
## 💼 Documentación

<details>
<summary>Expandir </summary>

<br>

[Reporte con Código (Python)](https://github.com/vbleal/Airports/blob/main/_Aero_Rent/Report/GH_Aeropuertos%20-%20Locales%20y%20Rentas.pdf)
  
</details>


<br>

---





