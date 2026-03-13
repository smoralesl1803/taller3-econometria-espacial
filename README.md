# Aglomeración Industrial en Cali: El Caso de la Fabricación de Calzado

**Taller 3 - Econometría Espacial**  
**Autora:** Sofía Morales López  
**Fecha:** 13 de marzo de 2026  

Este repositorio contiene el desarrollo del Taller 3 de Econometría Espacial, enfocado en el análisis de la **aglomeración industrial de la fabricación de calzado en Cali en 2005**. El objetivo del trabajo es estudiar si la localización de esta actividad económica dentro de la ciudad responde a patrones aleatorios o si, por el contrario, evidencia procesos de concentración geográfica, especialización territorial y aglomeración espacial.

## Introducción

La localización de la actividad económica en el espacio no es aleatoria. Las empresas tienden a agruparse en ciertas zonas debido a la existencia de economías de aglomeración, acceso a mercados, disponibilidad de mano de obra especializada, menores costos de transporte y proximidad a proveedores y redes de comercialización. En este contexto, el sector de fabricación de calzado en Cali constituye un caso de interés, dado su carácter tradicional, su vinculación con talleres de pequeña escala y su presencia histórica en corredores urbanos asociados al comercio y la manufactura popular.

Este trabajo analiza la distribución espacial de las empresas del sector de fabricación de calzado (CIIU 192) en Cali utilizando información georreferenciada del **Censo Económico de Cali 2005**. El análisis combina herramientas exploratorias, índices de concentración espacial y funciones de distancia para entender cómo se organiza territorialmente esta industria dentro de la ciudad.

## Objetivo

Analizar la localización espacial de la industria del calzado en Cali en 2005 para identificar:

- patrones de concentración geográfica,
- especialización territorial,
- diferencias entre subsectores,
- y distancias características de aglomeración entre empresas.

## Datos

El análisis utiliza datos del **Censo Económico de Cali 2005**, con información georreferenciada de establecimientos económicos y empleo por empresa. En particular, se trabaja con las empresas del sector **CIIU 192: fabricación de calzado**, junto con su clasificación a cuatro dígitos (CIIU 4), coordenadas espaciales y número de empleados.

También se utilizan capas geográficas de comunas y barrios de Cali para construir mapas de densidad, distribución de puntos y especialización territorial.

## Estructura del análisis

## Punto 1: Mapa de densidad y distribución de puntos

En esta primera parte se construyen mapas de distribución de puntos y densidad kernel para identificar las principales áreas de concentración espacial de las empresas del sector calzado en Cali.

Los resultados muestran un patrón de concentración marcado y no aleatorio, con especial énfasis en la **Comuna 9**, particularmente en barrios como **Sucre** y **Barrio Obrero**, así como en otros sectores del eje centro-oriente de la ciudad. Estos hallazgos sugieren que la actividad se organiza en corredores urbanos asociados históricamente al comercio mayorista y a la manufactura de pequeña escala.

Además, se discute el contexto económico de la industria del calzado en Cali en 2005 para dar una interpretación con sentido económico a los patrones observados.

## Punto 2: Índices de concentración espacial

En esta sección se calculan distintos índices para cuantificar la concentración industrial y geográfica del sector:

### 2.1 Índice de Herfindahl-Hirschman (IHH)

El IHH mide la concentración industrial a partir de la distribución del empleo entre firmas. Los resultados muestran que el sector de fabricación de calzado en Cali presenta una estructura relativamente fragmentada, con muchas empresas pequeñas y sin dominancia clara de unas pocas firmas grandes.

### 2.2 Índice de Ellison y Glaeser (EG)

El índice de Ellison y Glaeser permite medir la concentración geográfica controlando por la estructura de tamaño empresarial. Los resultados indican **alta concentración geográfica** del sector en su conjunto, lo que confirma formalmente el patrón visual observado en los mapas de densidad.

### 2.3 Índice de Maurel y Sédillot (MS)

El índice de Maurel y Sédillot incorpora de manera más explícita el tamaño de las firmas. En el agregado, este índice muestra que la concentración detectada por EG se debilita al considerar el peso relativo de las empresas, sugiriendo que parte del patrón espacial está influido por la distribución del empleo entre establecimientos.

### 2.4 Location Quotient (LQ) e Industry Quotient (IQ)

Se calculan indicadores de especialización espacial por comuna. Los resultados muestran que varias comunas de Cali presentan una fuerte especialización relativa en la fabricación de calzado. En este ejercicio, los valores del \(LQ\) y del \(IQ\) coinciden exactamente debido a que, con las definiciones utilizadas, ambos índices son algebraicamente equivalentes.

## Punto 3: Mapa del LQ

En esta parte se construye el mapa del **Location Quotient por comuna** para visualizar espacialmente la especialización del sector calzado en Cali.

Los resultados muestran que las comunas con mayor especialización relativa son la **Comuna 18**, la **Comuna 9** y la **Comuna 13**, con valores de \(LQ\) muy superiores a 1. Esto confirma que el sector no solo se concentra en términos absolutos, sino que además tiene un peso particularmente alto dentro de la estructura económica local de ciertas comunas.

## Punto 4: Funciones de distancia

Esta sección estima funciones de distancia continua para estudiar la aglomeración espacial del sector evitando el problema del MAUP.

### 4.1 Función \(K_d\) de Duranton y Overman (2005)

La función \(K_d\) se estima directamente a partir de las distancias entre pares de empresas y se compara con una envolvente de confianza obtenida a partir de simulaciones aleatorias dentro del polígono urbano de Cali.

Los resultados muestran evidencia clara de aglomeración espacial a distancias cortas e intermedias, especialmente hasta aproximadamente 6 kilómetros, con máxima intensidad alrededor de los 4 a 5 kilómetros. A distancias mayores, la evidencia sugiere dispersión.

### 4.2 Función \(M\) de Marcon y Puech (2010)

La función \(M\) expresa la concentración espacial en términos relativos, tomando como referencia el valor 1. Los resultados confirman que la industria del calzado presenta concentración geográfica significativa a distancias cortas e intermedias, y dispersión a distancias largas.

En conjunto, las funciones de distancia muestran que las empresas del sector no están distribuidas homogéneamente por toda la ciudad, sino agrupadas en núcleos relativamente próximos entre sí.

## Principales hallazgos

De manera general, el trabajo encuentra que:

- la industria del calzado en Cali está compuesta por numerosas empresas pequeñas;
- existe una concentración geográfica significativa del sector dentro de la ciudad;
- algunas comunas presentan alta especialización relativa en esta actividad;
- la aglomeración se manifiesta con mayor intensidad a distancias urbanas cortas e intermedias;
- y estos patrones son consistentes con una industria tradicional organizada alrededor de talleres, comercio mayorista, redes locales de abastecimiento y mano de obra especializada.

## Archivos del repositorio

- `Taller3.qmd`: archivo fuente en Quarto con el desarrollo del taller.
- `docs/index.html`: versión renderizada del documento, publicada como página web.
- `README.md`: descripción general del proyecto.

## Página web

La versión web del trabajo está disponible en GitHub Pages:

https://smoralesl1803.github.io/taller3-econometria-espacial/Taller3.html#taller-3

## Referencias

El documento completo incluye una sección final de referencias bibliográficas con las fuentes teóricas y empíricas utilizadas en el análisis.
