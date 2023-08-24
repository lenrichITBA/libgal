# Librería MLS

Una serie de funciones y Objetos que facilitan el trabajo de los Cientificos de Datos.


Evaluación de modelos: 

Cálculo de Métrica: KS

```python
evaluate_ks_and_roc_auc(y_real, y_proba)
```

Consta de 2 parámetros:

*	**y_real:** *(Requerido, lista de elementos booleanos)* Indica los valores reales que toma la variable.
*	**y_proba:** *(Requerido, lista de elementos float de 0. a 1.)* Indica los valores predichos por el modelo.

El output corresponden a las métricas de:
* Area bajo la curva ROC
* KS (Kolmogorov Smirnov)


Los siguientes objetos tienen sintaxis heredada de sklearn, por lo que heredan los metodos correspondientes  ```fit```, ```transform```,```fit_transform```. Se aprovecha la nomenclatura estandarizada por el Banco Galicia para la ingeniería de variables. Por ejemplo, los objetos que tratan valores númericos afectan las variables con prefijo o sufijo "vl" el cual indica "volumen"y usualmente refiere a montos de dinero.

```python
normalizador = NumNormTransformer() #Genera los Z-scores, es decir, la normalizacion de las variables solo de las columnas numericas
logtransformer = NumLogTransformer() #Agrega el logaritmo de los valores solo de las columnas numericas
reductorcategoricas = CategoricalReduceTransformer() #Se mantienen el 99% de las variables categoricas de mayor frecuencia, y el 1% menos frecuente es reemplazado por la categoria "Otros"
```


