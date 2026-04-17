# Estudio de los modelos aditivo y multiplicativo en econofísica

Repositorio con el informe en PDF y los notebooks utilizados para simular y analizar dos modelos de transferencia de dinero entre agentes:

* **Modelo aditivo**: intercambio de una cantidad aleatoria entre agentes.
* **Modelo aditivo con deuda**: permite saldo negativo limitado por una deuda máxima.
* **Modelo multiplicativo**: la cantidad transferida es una fracción del dinero del agente donante.

El proyecto estudia la distribución del dinero, la curva de Lorenz, el índice de Gini y propiedades análogas a variables termodinámicas como entropía, temperatura efectiva y calor específico.

## Contenido del repositorio

* `Estudio_de_los_modelos_aditivo_y_multiplicativo_en_econofisica_1.pdf`
  Informe principal con el desarrollo teórico, resultados y conclusiones.
* `Programa1_econofisica.ipynb`
  Simulación del modelo aditivo sin deuda y análisis estadístico.
* `Programa1_econofisica_deuda.ipynb`
  Simulación del modelo aditivo con deuda y comparación con el caso sin deuda.
* `Modelo_multiplicativo.ipynb`
  Simulación del modelo multiplicativo y cálculo de entropía, temperatura y Lorenz.

## Objetivo

Analizar cómo cambian las distribuciones de dinero en sistemas cerrados de agentes y comparar el comportamiento estadístico entre modelos aditivos y multiplicativos.

## Resultados que se estudian

* Histograma y distribución de dinero por agente.
* Prueba de Kolmogorov-Smirnov para verificar ajuste exponencial.
* Curva de Lorenz.
* Índice de Gini.
* Entropía de Shannon.
* Temperatura efectiva y calor específico en la interpretación termodinámica del modelo.

## Requisitos

Los notebooks fueron desarrollados en Python y utilizan principalmente:

* `numpy`
* `pandas`
* `matplotlib`
* `scipy`

También pueden ejecutarse en **Jupyter Notebook** o **Google Colab**.

## Cómo ejecutar

1. Abre el notebook que quieras analizar.
2. Ejecuta las celdas en orden.
3. Verifica que los archivos de datos usados por el notebook estén disponibles en la ruta correspondiente o cámbiala por una ruta local válida.
4. Revisa las gráficas y los valores calculados en cada sección.

Ejemplo de instalación de dependencias:

```bash
pip install numpy pandas matplotlib scipy
```

## Notas importantes

* Algunos notebooks usan rutas absolutas de Google Colab, por ejemplo archivos dentro de `MyDrive`. Es recomendable cambiarlas por rutas relativas si el proyecto se va a subir a GitHub.
* Se generan gráficas como histogramas, curvas acumuladas, Q-Q plots y curvas de Lorenz.
* El caso con deuda desplaza la distribución, pero conserva la forma exponencial al trabajar con el dinero ajustado por la deuda máxima.

## Conclusión general

El proyecto muestra que el **modelo aditivo** produce una distribución exponencial del dinero, mientras que el **modelo multiplicativo** presenta un comportamiento distinto y una menor desigualdad, según la curva de Lorenz y el índice de Gini.



