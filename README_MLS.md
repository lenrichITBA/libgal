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



```python
NumNormTransformer
```

```python
NumLogTransformer
```


```python
CategoricalReduceTransformer
```

  
