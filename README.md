# Reporte de ventas y segmentación de clientes para "El Mercado"
![image](https://github.com/karlarochaes/el-mercado-rfm/assets/88100992/4f83b2a8-f1a4-44f1-8dfa-290b151840ed)
---
## Tabla de contenidos
- [Introducción](#introducción)
- [Herramientas](#herramientas)
- [Procesamiento de los datos](#procesamiento-de-los-datos)
- [Segmentación](#segmentación)
- [Visualización](#visualización)
- [Resultados](#resultados)
- [Conclusiones y recomendaciones](#conclusiones-y-recomendaciones)

## Introducción
La tienda El Mercado busca entender las preferencias de sus consumidores para personalizar sus campañas de marketing y mejorar el porcentaje de retención de clientes. En consecuencia, esto aumentaría sus ventas e ingresos. Para abordar estos retos, en este proyecto se analizaron las ventas de la tienda correspondientes al periodo del 30 de julio de 2020 al 29 de junio de 2022. 

## Herramientas
- Google Spreadsheets - [Consulta el resultado final aquí](https://docs.google.com/spreadsheets/d/1Z3RvUoFn5QbKlxlfVnVh9NZ13rlMTiD2MVn0HBWjVz4/edit?usp=sharing)
- Looker Studio - [Consulta el resultado final aquí](https://lookerstudio.google.com/reporting/1660c1fb-761e-4779-b939-f96382361a8c)

## Procesamiento de los datos
Se eliminaron de la base de datos los siguientes clientes:
- Sin dato de ingreso (24)
- Con ingreso atípico (1)
- Con edad mayor a 95 (3)
- Sin transacciones (10)

Se crearon nuevas variables
- edad
- transacciones
- transacciones_en_linea
- transacciones_en_tienda

Después del procesamiento, se obtuvo una base de datos con un total de 2202 clientes.

## Segmentación
Para poder segmentar la base de clientes, se utilizó la técnica RFM, la cual considera los siguientes criterios:
- Recency. Tiempo desde la última transacción.
- Frequency. Número de transacciones.
- Monetary value. Valor total de las transacciones.
  
Con base en estas características, se agrupó a los clientes en siete categorías balanceadas (con aproximadamente la misma cantidad de clientes por categoría). Los clientes no similares a alguna de las otras categorías se dejaron sin clasificar.

![image](https://github.com/karlarochaes/el-mercado-rfm/assets/88100992/10c21582-d17a-447e-8326-6399e6514da2)

![image](https://github.com/karlarochaes/el-mercado-rfm/assets/88100992/678c0989-9262-4faf-840b-37b3f4775749)

## Visualización
Los resultados se visualizaron mediante un dashboard en [Google Spreadsheets](https://docs.google.com/spreadsheets/d/1Z3RvUoFn5QbKlxlfVnVh9NZ13rlMTiD2MVn0HBWjVz4/edit?usp=sharing) y un dashboard complementario en [Looker Studio](https://lookerstudio.google.com/reporting/1660c1fb-761e-4779-b939-f96382361a8c).

![image](https://github.com/karlarochaes/el-mercado-rfm/assets/88100992/f61ab84a-ef19-4c61-af76-05b55eb92979)

## Resultados
- El vino representó la mitad de las ganancias totales.
- Pocos clientes realizaron transacciones en los meses posteriores a su primera compra.
- Tres categorías de clientes representan el 80% del monto de ventas. Esas mismas tres categorías son grandes consumidores de vino y carnes.
- Los segmentos tuvieron algunas diferencias en las preferencias de compra y respondieron de manera distinta a la campaña de marketing.
  
![image](https://github.com/karlarochaes/el-mercado-rfm/assets/88100992/9e13aaa6-09e5-4632-82c6-093f318ea51f)

## Conclusiones y recomendaciones
- Los clientes frecuentes en el pasado aportan gran valor monetario y es probable que respondan a las campañas de marketing, por lo que es conveniente traerlos de vuelta para que realicen compras nuevamente.
- Los clientes recientes no frecuentes tienen un perfil similar al de los Clientes frecuentes en el pasado, por lo que es conveniente ofrecerles promociones a fin de que realicen más transacciones.
- Para los Clientes top y los Clientes de valor monetario es conveniente implementar promociones para compras en productos clave como el vino y las carnes.
- Para los Clientes en desarrollo se pueden implementar estrategias de marketing de varios tipos. Por sus características, podrían convertirse en un grupo de gran valor (podrían migrar hacia los sectores con las puntuaciones más altas de RFM).
- Los Clientes durmientes tuvieron un buen crecimiento en el pasado pero sus transacciones disminuyeron. Sería conveniente generar estrategias de retención para evitar que se incluyan en las puntuaciones más bajas.
- Finalmente, para los Clientes bottom, es necesario mejorar las estrategias para que sean clientes más recientes y/o más frecuentes incluso si no realizan compras de gran valor monetario.
