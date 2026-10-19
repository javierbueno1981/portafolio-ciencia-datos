# SQL y Python · recursos humanos

**Autor:** Javier Bueno Sánchez · EBAC, Profesión Científico de Datos

## Propósito

Crear una base SQLite y resolver consultas sobre permanencia y condiciones laborales.

## Técnicas

SQLite, pandas, filtros y agregaciones SQL.

## Archivos

- [Tarea M40 SQLite Javier Bueno Sanchez-1.pdf](Tarea%20M40%20SQLite%20Javier%20Bueno%20Sanchez-1.pdf)
- [Tarea M40 SQLite Javier Bueno Sanchez.pdf](Tarea%20M40%20SQLite%20Javier%20Bueno%20Sanchez.pdf)
- [Tarea M41 SQL con Python Javier Bueno Sanchez.ipynb](Tarea%20M41%20SQL%20con%20Python%20Javier%20Bueno%20Sanchez.ipynb)
- [Tarea M41 SQL con Python Javier Bueno Sanchez.pdf](Tarea%20M41%20SQL%20con%20Python%20Javier%20Bueno%20Sanchez.pdf)

## Datos y reproducción

Consulte [DATOS.md](DATOS.md). Abra Jupyter desde esta carpeta y ejecute las celdas en orden después de aportar los datos. El entorno sugerido está en [requirements.txt](../../requirements.txt); no se ha validado un entorno único para todas las actividades. Las salidas incluidas son históricas, no una ejecución nueva. Los archivos `.pbix` requieren Power BI Desktop y pueden necesitar restablecer las rutas de origen.

## Conclusiones documentadas en el trabajo

Los siguientes extractos proceden de los notebooks originales; no son resultados recalculados.

### Tarea M41 SQL con Python Javier Bueno Sanchez.ipynb

**9. Conclusiones.**

En esta actividad se creó correctamente la base de datos SQLite `RH.db` a partir del archivo externo `recursos_humanos.csv`. La información de **14,999 empleados** fue almacenada en la tabla `Detalle` y posteriormente consultada mediante instrucciones SQL ejecutadas desde Python.

Los principales resultados fueron los siguientes:

- Los empleados que permanecieron en la empresa presentaron una satisfacción promedio de **0.6668**, superior al **0.4401** registrado por quienes abandonaron la organización.
- Los **13,762 empleados** con salario bajo o medio trabajaron un promedio conjunto de **201.16 horas mensuales**.
- Por nivel salarial, el promedio fue de **201.00 horas** para salarios bajos y **201.34 horas** para salarios medios, mostrando una diferencia mínima.
- Se identificaron **19 empleados** que recibieron una promoción durante los últimos cinco años y que, aun así, abandonaron la empresa.
- Se localizaron **2,988 empleados** cuya última evaluación fue igual o superior a **0.9**.

Los resultados muestran que una menor satisfacción laboral está asociada con el abandono de la empresa. También evidencian que variables como una promoción o una evaluación elevada no explican por sí solas la permanencia del empleado, por lo que deben analizarse junto con el salario, la carga de trabajo y la antigüedad.

La actividad permitió integrar Python como herramienta de administración y presentación de resultados con SQLite como motor para almacenar, filtrar y resumir los datos mediante SQL.

## Limitaciones

Trabajo formativo. Las asociaciones no establecen causalidad. El resultado depende de la fuente, la partición y los supuestos descritos en cada archivo. Revisar la disponibilidad y los derechos de los datos antes de publicarlos.
