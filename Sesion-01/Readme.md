[`Análisis de Datos con Python`](../README.md) > `Sesión 1`

## Sesión 01: Estimados de Locación y Variabilidad

<img src="../imagenes/pizarron.png" align="right" height="100" width="100" hspace="10">

### 1. Objetivos :dart:

- Utilizar Google Colab en conjunción con Google Drive y Github.
- Identificar los tipos de datos estructurados existen.
- Identificar los estimados de locación y en qué momento son útiles.
- Identificar valores típicos y atípicos.
- Realizar cálculos estadísticos robustos.
- Identificar los estimados de variabilidad y en qué momento son útiles.
- Identificar los estadísticos de orden.

### 2. Contenido :blue_book:

#### <ins>Utilización de software</ins>

Antes que nada, vamos a asegurarnos de que las siguientes cosas estén resueltas:

a) Todos tenemos una cuenta en Google Drive.
b) Todos hemos creado un Acceso Directo desde la carpeta [Datasets](https://drive.google.com/drive/u/1/folders/1oXUNacyjuHpGBkmESnKIDA5s03UnS8Vg) a nuestro Drive.
c) Todos sabemos cómo montar nuestro Google Drive en un Notebook de Google Colab y leer nuestros conjuntos de datos usando `pandas`.
d) Todos sabemos cómo leer Jupyter Notebooks desde el repositorio del módulo en Google Colab.

---

#### <ins>Datos estructurados</ins>

Hay dos grandes categorías de datos que manejamos en Ciencia de Datos: datos estructurados y datos no estructurados. Por el momento sólo vamos a hablar sobre datos estructurados. Los datos estructurados pueden subdividirse de la siguiente manera:

1. Numéricos: Datos representados por números que pueden tomar una cantidad no predefinida de valores.
  a) Discretos: Datos que sólo pueden tomar el valor de un número entero.
  b) Continuos: Datos que pueden toman cualquier valor dentro de un intervalo.
2. Categóricos: Datos que sólo pueden tomar un conjunto específico de valores que representan un conjunto de posibles categorías.
  a) Binarios: Datos categóricos que sólo tienen dos categorías posibles.
  b) Ordinales: Datos categóricos que tienen un orden explícito.

<a href="Reto-01/datos_estructurados.ipynb" target="_blank"> **`Reto 1`** </a>

---

#### <ins>Estimados de locación</ins>

Los estimados de locación nos sirven para determinar qué valor describe mejor un conjunto de datos. A este valor le llamamos el "valor típico" de nuestro conjunto. Dos estimados son los más comunes y lo más utilizados:

1. Promedio (o media)
2. Mediana

Veamos cómo se calculan usando `pandas`.

<a href="Ejemplo-01/estimados_de_locacion.ipynb" target="_blank"> **`Ejemplo 1`** </a>
<a href="Reto-02/estimados_de_locacion.ipynb" target="_blank"> **`Reto 2`** </a>

---

#### <ins>Valores atípicos</ins>

Hemos aprendido a conseguir "valores típicos" se sirven para describir un conjunto de datos. Así como existen valores que se parecen a la norma, hay también valores que difieren mucho de la norma. Estos valores suelen sobresalir de nuestro conjunto de datos porque se encuentran a mucha distancia del grueso de las muestras.

Estos valores son los "valores atípicos". Hay veces en las que tener valores atípicos no nos preocupa, pero otras veces pueden ser peligrosos porque modifican nuestros estimados de locación, dándonos descripciones erróneas de nuestro conjunto de datos.

Más adelante aprenderemos a detectar valores atípicos, pero por lo pronto vamos a aprender un estimado de locación que es más *robusto* (menos sensible a valores atípicos) que el promedio y la mediana: la media truncada.

<a href="Ejemplo-02/media_truncada.ipynb" target="_blank"> **`Ejemplo 2`** </a>

---

#### <ins>Estimados de variabilidad</ins>

Los estimados de locación se utilizan para intentar encontrar un "valor típico" que describa adecuadamente nuestro conjunto de datos. Los estimados de variabilidad, en cambio, nos sirven para determinar qué tan dispersos están los datos alrededor de nuestro valor típico. Nuestros datos pueden estar en general o muy cerca o muy distantes del valor típico, y los estimados de variabilidad nos ayudan a determinar esto.

Uno de los estimados más utilizados es la desviación estándar. Veamos cómo funciona.

<a href="Ejemplo-03/desviacion_estandar.ipynb" target="_blank"> **`Ejemplo 3`** </a>
<a href="Reto-03/desviacion_estandar.ipynb" target="_blank"> **`Reto 3`** </a>

---

#### <ins>Estadísticos de Orden</ins>

Existen otras formas de calcular la dispersión de nuestros datos que requieren que nuestros datos estén ordenados ascendentemente. Estos cálculos nos dan otra perspectiva acerca de la distribución de nuestros datos que puede sernos de mucha utilidad. 

Tres de los estadísticos de orden más comunes son el **Rango**, los **Percentiles** y el **Rango intercuartílico**. Veamos cómo funcionan.

<a href="Ejemplo-04/estadisticos_de_orden.ipynb" target="_blank"> **`Ejemplo 4`** </a>
<a href="Reto-04/estadisticos_de_orden.ipynb" target="_blank"> **`Reto 4`** </a>

---

### 3. Postwork :memo:

[**`Postwork Sesión 1`**](Postwork/Readme.md)
