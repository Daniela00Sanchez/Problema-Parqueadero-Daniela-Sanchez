# Simulación del sistema de pago de parqueaderos

## Descripción del proyecto

Este proyecto corresponde a la actividad de Ingeniería de Simulación, en la cual se analiza el funcionamiento del sistema de pago de un parqueadero del centro comercial ficticio Supercentro.

El objetivo es evaluar los tiempos de espera de los usuarios, el comportamiento de las filas y las alternativas de atención, utilizando una simulación desarrollada en Python mediante Google Colab.

## Objetivo

Analizar el funcionamiento de tres cajeros de pago y comparar diferentes estrategias para determinar cuál permite atender a los usuarios de manera más eficiente.

## Metodología

Se desarrolló una simulación de eventos discretos que representa la llegada de vehículos, la selección de una fila y el proceso de atención en los cajeros.

Se consideraron cuatro tipos de usuarios:

- Rápido: tiempo promedio de atención de 1 minuto.
- Normal: tiempo promedio de atención de 3 minutos.
- Lento: tiempo promedio de atención de 4 minutos.
- Muy lento: tiempo promedio de atención de 6 minutos.

Para completar la distribución de usuarios se asumieron porcentajes de 25 % para rápidos, 20 % para normales, 27,5 % para lentos y 27,5 % para muy lentos.

Se compararon estrategias de selección de fila, el funcionamiento con tres y cuatro cajeros y escenarios de mayor demanda. También se analizaron el período transitorio, las réplicas independientes y la sensibilidad de los resultados ante cambios en los tipos de usuarios.

## Principales resultados

| Escenario | Espera promedio |
|---|---:|
| 3 cajeros, fila más corta | 0,19 minutos |
| 3 cajeros, selección aleatoria | 1,49 minutos |
| 4 cajeros, fila más corta | 0,03 minutos |
| 3 cajeros, demanda triple | 4,38 minutos |
| 4 cajeros, demanda triple | 1,10 minutos |

Los resultados muestran que, para la demanda normal simulada, tres cajeros pueden ofrecer una atención adecuada cuando los usuarios eligen la fila más corta.

Cuando la demanda aumenta considerablemente, disponer de un cuarto cajero ayuda a reducir los tiempos de espera.

## Herramientas utilizadas

- Python
- Google Colab
- NumPy
- Pandas
- Matplotlib
- SciPy

## Cómo ejecutar la simulación

1. Abrir el archivo `Sanchez_Daniela_Problema_Parqueadero.ipynb` en Google Colab.
2. Seleccionar la opción **Entorno de ejecución → Ejecutar todo**.
3. Revisar los resultados, las tablas y las gráficas generadas.
4. Consultar los archivos CSV para examinar los resultados de la simulación.

## Archivos del repositorio

El repositorio incluye:

- **Cuaderno de Python (.ipynb):** contiene el código y el desarrollo de la simulación.
- **Informe en Word (.docx):** presenta la metodología, el análisis y las conclusiones.
- **8 archivos CSV:** contienen los resultados obtenidos.
- **9 gráficas PNG:** muestran el comportamiento de los cajeros, las filas y los escenarios estudiados.

## Conclusiones

La simulación permitió estudiar cómo influyen la cantidad de cajeros y la estrategia de selección de filas en los tiempos de espera.

Se encontró que elegir la fila más corta ofrece mejores resultados que seleccionar un cajero aleatoriamente. Además, incorporar un cuarto cajero puede ser útil cuando se presentan aumentos importantes en la demanda.

Los resultados dependen de los supuestos utilizados y constituyen una evaluación académica. Para aplicar las recomendaciones a un parqueadero real sería necesario contar con datos observados y realizar una validación adicional.

## Responsable

Daniela María Sánchez Sánchez  
Ingeniería de Software y bases de datos

Asignatura:Simulación  

Noviembre de 2026
