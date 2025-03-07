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
	-- Logo.png
--- Excel
	-- Ecommerce_Tech.xlsx

```
## 3. Descripción de las columnnas del conjunto de datos

**Hoja: Ecommerce_Ventas_Productos.csv**
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

## 1. Transformación y Limpieza de Datos 🗂️
A continuación, se explicarán los pasos que se han seguido para transformar y limpiar los datos del csv original "ecommerce_product_sales.csv"
- Se crea Excel "Carga_Tansf_Datos.xlsx y se carga el conjunto de datos original creando una tabla.
- 


Añadir una nueva columna (Género_) en la cual sustituyamos las palabras en inglés “Male” y “Female” por “Masculino” y “Femenino” y ocultamos la de Género, con la fórmula Sustituir.
- Cambiar el formato de la columna precio por un formato de Moneda.
- Añadir columna Descuento %, y transformar el número de descuento en porcentaje. Ocultar la columna Descuento.
- Añadir una columna nueva calculando las ventas totales.
- Añadir columna nueva para determinar el número de descuentos aplicados.
- Añadir columna nueva para determinar la cantidad exacta descontada.
- Añadir una columna con el día de la semana en la que se produjo la venta con la fórmula Texto.
- Añadir columna nueva de Beneficio total, restando el descuento aplicado a las ventas totales.
- Modificar Formatos de Cantidad y Edad del cliente por número.
## 2. Análisis Descriptivo de los Datos 📈
- Añadir una nueva columna (Género_) en la cual sustituyamos las palabras en inglés “Male” y “Female” por “Masculino” y “Femenino” y ocultamos la de Género, con la fórmula Sustituir.
- Cambiar el formato de la columna precio por un formato de Moneda.
- Añadir columna Descuento %, y transformar el número de descuento en porcentaje. Ocultar la columna Descuento.
- Añadir una columna nueva calculando las ventas totales.
- Añadir columna nueva para determinar el número de descuentos aplicados.
- Añadir columna nueva para determinar la cantidad exacta descontada.
- Añadir una columna con el día de la semana en la que se produjo la venta con la fórmula Texto.
- Añadir columna nueva de Beneficio total, restando el descuento aplicado a las ventas totales.
- Modificar Formatos de Cantidad y Edad del cliente por número.

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
