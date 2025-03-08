![image alt](https://github.com/Krystiian5/Ecommerce_Tech/blob/main/Data/Logo.png?raw=true)
# Análisis de Beneficios de Ecommerce_Tech 💶
En este proyecto vamos a trabajar sobre un conjunto de datos para una empresa llamada **Ecommerce_Tech**, en el que vamos a analizar los **beneficios** obtenidos, tanto en un determinado momento, como a lo largo del tiempo, así como entender el comportamiento de los clientes, según su edad, género, región, tipo de producto y método de pago.
## 1. Descripción y objetivo del Proyecto
Este repositorio contiene un análisis de **beneficios** de la empresa Ecommerce_Tech, con datos detallados sobre productos vendidos, clientes, descuentos y beneficios obtenidos. La información será procesada para identificar patrones y tendencias en los beneficios.
El objetivo principal de este proyecto es crear un dashboard interactivo que facilite la visualización de datos relevantes y proporcionen insights prácticos para la toma de decisiones estratégicas.
## 2. Estructura del Repositorio
```bash
--- Data
	-- ecommerce_product_sales #Datos Originales
	-- Datos_Transformados.csv
	-- Logo.png
--- Excels
	-- Carga_Transform_Datos.xlsx
	-- Analisis_Datos.xlsx

```
## 3. Descripción de las columnnas del conjunto de datos

**Hoja: Ecommerce_Product_Sales.csv**
Esta hoja contiene las siguientes columnas clave:
### Datos de los usuarios:
- **Venta_ID:** Identificador único de cada venta.
- **Edad del cliente:** Edad del usuario.
- **Género_:** Género del usuario (Masculino, Femenino).
- **Región:** Ubicación del usuario (Continentes).
### Datos del Producto:
- **Tipo de Producto:** 5 tipos distintos de productos (Teléfono inteligente, reloj inteligente, tablet, portátil y auriculares).
- **Categoría:** Divididos en 2 categorías (Electrónica y Accesorios).

### Datos de Transacción
- **Precio:** Precio por unidad.
- **Cantidad:** Número de cantidades vendidas.
- **Ventas Totales:** Valor total de ventas.
- **Descuento:** Porcentaje de descuento aplicado.
- **Método de Pago:** Método con el que se ha realizado el pago (Tarjeta de Débito, Crédito, Paypal o transferencia bancaria).
- **Beneficio Total:** Ingreso neto tras aplicar descuentos.
- **Fecha de venta:** Momento en el que se realizó la transacción.

## 4. Transformación y Limpieza de Datos 🗂️
A continuación, se explicarán los pasos que se han seguido para transformar y limpiar los datos del csv original "ecommerce_product_sales.csv"
- Se crea Excel "Carga_Tansf_Datos.xlsx y se carga el conjunto de datos original creando una tabla.
- Se crea una nueva hoja llamada "Datos_Transformados".
- Se comprueba si hay duplicados. En este caso no se encuentran duplicados.
- Crear una hoja nueva de "Tablas_Auxiliares" para traducir del inglés al español encabezados, Productos, Categoría, Género, Método de pago y Región.
- Ocultar columnas con los datos en inglés.
- Columnas Precio, Descuento y Ventas Totales no están reconocidas como números ya que están situados a la izquierda. Esto es debido a que hay que cambiar el "punto" por la "coma". Lo reemplazamos.
- Cambiamos el formato de Precio y Ventas totales a número y el de Descuento a formato porcentaje.
- Comprobar si la columna Ventas Totales está bien calculada. Tiene que ser el precio multiplicado por la cantidad restándole el descuento. Está bien en este caso.
- Crear una nueva columna "Rango_Edad": Nos sirve para categorizar las edades por grupos.
- Crear nueva columna "Descuento_Aplicado": Nos sirve para identificar si se ha aplicado descuento o no.
- Crear nueva columna "Cantidad_Descontada": Nos sirve para calcular el total del dinero descontado.
- Guardar Hoja Datos transformados en un archivo .csv

## 5. Análisis Descriptivo Numérico de los Datos 📈
- Cargamos datos nuevo excel de Datos_Transformados.
- Eliminamos las columnnas duplicadas y ocultas del conjunto de datos anterior.
- Creamos una nnueva hoja llamada "Análisis_Descriptivo_Num" en la que vamos a analizar todas las columnas numéricas.
- **Precio:**
- **Edad:** Estadística Descriptiva. Crear gráfico mediante una tabla dinámica y un *box plot:*
	- El primer cuartil de mis datos (el 25%) está por debajo de 30; el segundo cuartil (el 50%) de mis datos están por encima o por abajo de 42; el tercer cuartil (el 75%) de mis datos está por debajo de 54. Vemos que no hay outliers.


## 4. Resultados y Conclusiones 📋
- En términos generales vemos lo siguiente:
	- El producto que genera más beneficios son los smartwatch y el que menos sería el Laptop.
	- La región que genera más beneficios es Sud América y la que menos Europa.
	- El año con más beneficio generado es el 2024.
-	En cuanto a los beneficios a lo largo del tiempo vemos que en el 2023 hay un aumento de los mismos en primavera y en los meses de invierno son los más bajos. Sin embargo, en el 2024, identificamos un comportamiento de los beneficios más lineal y constante a lo largo del año.
-	En relación al rango de edad que genera más beneficios, estaría entre los 48 y 57 años. Sin embargo, el rango de edad con menos beneficios generados se encuentra entre los 58 y 67 años. 
-	Crear estrategias de marketing más efectivas para mejorar los beneficios en términos generales en la época de invierno, del tipo de producto como es el Laptop, en Europa y en la población que se encuentra en un rango de edad entre los 58 y 67 años.

## Fuente de Datos 📖

[Datos](https://www.kaggle.com/datasets/simranjitkhehra/e-commerce-product-sales)
