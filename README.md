# Inferencia causal mediante correlación sintáctica


## Ejemplo de uso

Ejecutar una simulación (un "multirun") con un modelo funcional y múltiples tests de independencia:

```python parametric_model_execution_example.py```

Modificando el script se puede elegir el modelo y los tests a emplear.
Una vez creado el archivo .pkl con los resultados de la simulación, para generar mejores figuras de los resultados:

```python generate_pydot_figures_example.py```

## Simulaciones en la tesis

Para las simulaciones presentadas en la tesis, se utilizaron las funciones definidas en `analysis/models.py`, `analysis/multiruns.py` y `analysis/statistical.py`.

## Dependencias

Versión de Python: >=3.8
Requiere `graphviz` (`sudo apt install graphviz`)
Paquetes de Python necesarios:
* `numpy`
* `matplotlib`
* `scipy`
* `networkx`
* `graphviz`
* `pydot`
* `dill`
* `rpy2` (opcional, para test de contingencia exacto)
* `joblib`

## Instalación via pip

    pip install git+https://github.com/gabrielgoren/tesislic-public@pip_installable

Actualmente no todas las funciones funcionan correctamente al instalarse como paquete.
**TODO**: adaptar el código de guardado en disco para que funcione como paquete.