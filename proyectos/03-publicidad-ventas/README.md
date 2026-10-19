# Publicidad y ventas

**Autor:** Javier Bueno Sánchez · EBAC, Profesión Científico de Datos

## Propósito

Evaluar la asociación de TV, Radio y Newspaper con ventas e interpretar intervalos.

## Técnicas

Regresión múltiple, selección de variables e intervalos de confianza/predicción.

## Archivos

- [M53_Advertising_intervalos_supuestos.ipynb](M53_Advertising_intervalos_supuestos.ipynb)
- [M53_Advertising_intervalos_supuestos.pdf](M53_Advertising_intervalos_supuestos.pdf)

## Datos y reproducción

Consulte [DATOS.md](DATOS.md). Abra Jupyter desde esta carpeta y ejecute las celdas en orden después de aportar los datos. El entorno sugerido está en [requirements.txt](../../requirements.txt); no se ha validado un entorno único para todas las actividades. Las salidas incluidas son históricas, no una ejecución nueva. Los archivos `.pbix` requieren Power BI Desktop y pueden necesitar restablecer las rutas de origen.

## Conclusiones documentadas en el trabajo

Los siguientes extractos proceden de los notebooks originales; no son resultados recalculados.

### M53_Advertising_intervalos_supuestos.ipynb

**Interpretación integrada.** La ecuación final utiliza TV y Radio; el efecto estimado del periódico no supera la selección al 10%. Los coeficientes representan asociaciones condicionales por una unidad adicional invertida, no retornos causales. La comparación R²/MAE/RMSE en prueba describe utilidad predictiva fuera del entrenamiento. La inversión de Radio=50 excede ligeramente el máximo observado en entrenamiento (49.4); corresponde señalar esta extrapolación marginal. Cook identifica observaciones para revisión, sin justificación para eliminarlas automáticamente. Fuentes metodológicas: documentación de `statsmodels` (OLS, `get_prediction`, `het_white`, `durbin_watson`) y SciPy (`skew`, `kurtosis`).

## Limitaciones

Trabajo formativo. Las asociaciones no establecen causalidad. El resultado depende de la fuente, la partición y los supuestos descritos en cada archivo. Revisar la disponibilidad y los derechos de los datos antes de publicarlos.
