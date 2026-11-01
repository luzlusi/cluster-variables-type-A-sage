# cluster-variables-type-A-sage
# Variables de conglomerado de tipo A_n con coeficientes mediante triangulaciones y grafos de serpientes. 

Código en Sage para calcular variables de conglomerado de tipo A_n con coeficientes usando triangulaciones de polígonos (modelo de superficies) y grafos de serpiente.

Este código fue desarrollado como parte de mi tesis: **Grafos de serpiente y algoritmos en álgebras de conglomerado**, Universidad Nacional de Mar del Plata, dirigida por Ana García Elsener y Jorge N. López. 

## Contenido

- `TesisFinal (1) .ipynb`: notebook con la implementación y ejemplos.

## Requisitos

- [SageMath](https://www.sagemath.org/)
- Jupyter con el kernel de SageMath (incluido en la instalación de SageMath)

## Cómo ejecutarlo

<!--
### Opción 1: Binder (sin instalar nada)

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/luzlusi/cluster-variables-type-A-sage/HEAD)

Hacé clic en el botón y abrí el notebook. La primera vez puede tardar varios minutos. Los cambios no se guardan, así que descargá el notebook si lo modificás.
-->

### Opción 1: CoCalc

1. Creá una cuenta gratuita en [cocalc.com](https://cocalc.com).
2. Creá un proyecto y subí el archivo `.ipynb`.
3. Abrilo y elegí el kernel **SageMath**.

### Opción 2: Instalación local

1. Instalá SageMath siguiendo las [instrucciones oficiales](https://doc.sagemath.org/html/en/installation/) u otras.
2. Desde la carpeta del repositorio, ejecutá:

       sage -n jupyter

3. Abrí el notebook desde la lista de archivos.

## Qué hace el código

El notebook se divide en los siguientes bloques:

1. **Librerías:** importa las librerías necesarias.
2. **Superficie triangulada:** crea la superficie triangulada y sus variables de conglomerado de tipo A_n, indicando el valor de n.
3. **Curva:** traza una nueva curva que corta a la superficie e identifica las variables cortadas.
4. **Grafo de serpiente:** dibuja el grafo de serpiente (*snake graph*) asociado y describe sus *tiles*.
5. **Correspondencias perfectas:** calcula las correspondencias perfectas de un grafo de serpiente.
6. **Funciones auxiliares:** define las funciones previas necesarias para calcular luego la correspondencia minimal y la variable de conglomerado.
7. **Correspondencia minimal:** calcula la correspondencia minimal de un conjunto de correspondencias perfectas.
8. **Variable de conglomerado:** calcula la variable de conglomerado de un grafo de serpiente etiquetado, asociado a la superficie.

## Ejemplo

Para el tipo A_2 (un pentágono), las cinco variables de conglomerado son:

    (1 + y1*x2)/x1,  (y1 + x1 + y1*y2*x2)/(x1*x2),  (y1 + x1)/x2

junto con las variables iniciales x1, x2.

## Cómo citar

Si usás este código, por favor citá:

    [Lusi, Luz]. Variables de conglomerado de tipo A_n mediante triangulaciones y grafos de serpiente (código en Sage).
    Repositorio de GitHub, [URL del repo](https://github.com/luzlusi/cluster-variables-type-A-sage), 2026.
    Código complementario de la tesis "Grafos de serpiente y algoritmos en álgebras de conglomerado",
    Universidad Nacional de Mar del Plata.
