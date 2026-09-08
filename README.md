
# Evaluación 1: Transmisión de Señales

## Datos del estudiante

**Nombre:** Daniel Videla, NIcolas Bastidas
**Asignatura:** tecnicas de transmicion
**Docente:** Daniel Ruz 
**Sede:** La Serena

========
# Guia en tecnicas de transmicion
guía de la rama de técnicas de transmisión junto a actividades de trabajo que explica el funcionamiento de maquinas de trabajo

========
Introducción

Las señales son fundamentales para transmitir información en los sistemas de telecomunicaciones. Una señal puede representar información como voz, imágenes, datos o video y puede ser transmitida mediante diferentes medios.

En este trabajo se estudian los principales conceptos relacionados con la transmisión de señales. Se revisan las diferencias entre señales analógicas y digitales, el análisis en el dominio del tiempo y de la frecuencia, la Transformada de Fourier, los principales parámetros de transmisión y los mecanismos utilizados para transportar información.

También se estudian conceptos matemáticos importantes, como la capacidad de canal de Shannon y el Teorema de Muestreo de Nyquist-Shannon. Finalmente, se comparan distintos tipos de transmisión para comprender sus características y aplicaciones.

========
1. Naturaleza de la Información y Señales
1.1 ¿Qué es una señal?

Una señal es una representación física de información que puede transmitirse desde un emisor hacia un receptor.

Una señal puede transportar diferentes tipos de información, por ejemplo:

Voz.
Video.
Datos.
Información de sensores.
Señales de control.

Un sistema de comunicación básico puede representarse de la siguiente manera:

┌──────────┐
│ EMISOR   │
└────┬─────┘
     │
     │ Señal
     ▼
┌──────────┐
│  MEDIO   │
│   DE     │
│TRANSMISIÓN│
└────┬─────┘
     │
     ▼
┌──────────┐
│ RECEPTOR │
└──────────┘

========
1.2 Señal analógica

Una señal analógica es una señal que puede variar de manera continua en el tiempo y tomar diferentes valores de amplitud.

Un ejemplo de señal analógica es una señal de audio capturada por un micrófono.

Características
Tiene variación continua.
Puede tomar muchos valores de amplitud.
Puede verse afectada por ruido e interferencias.
Se puede representar mediante una onda continua.
Representación
Amplitud
   │
   │      /¯\       /¯\
   │     /   \     /   \
   │____/     \___/     \____
   │
   └────────────────────────── Tiempo

========
1.3 Señal digital

Una señal digital utiliza valores discretos para representar información. En los sistemas digitales es común utilizar bits representados mediante 0 y 1.

Características
Utiliza valores discretos.
Los datos pueden representarse mediante bits.
Es utilizada ampliamente en sistemas informáticos y de redes.
Permite almacenar y procesar información digitalmente.
Representación
Amplitud
   │
  1│ ┌─────┐       ┌─────┐
   │ │     │       │     │
  0│─┘     └───────┘     └──────
   │
   └────────────────────────── Tiempo

========
## 1.4 Comparación entre señal analógica y digital

Las señales analógicas y digitales se utilizan para transmitir información, pero se diferencian principalmente en la forma en que representan los datos.

### Señal analógica

Una señal analógica es una señal **continua**, es decir, puede tomar una gran cantidad de valores dentro de un determinado rango. Su representación normalmente corresponde a una onda continua.

**Ejemplos:**

* Audio.
* Radio.
* Señales provenientes de sensores.

### Señal digital

Una señal digital representa la información mediante **valores discretos**, normalmente utilizando valores binarios como `0` y `1`. Este tipo de señal es utilizado ampliamente en computadores y redes.

**Ejemplos:**

* Datos de computadores.
* Redes de comunicación.
* Sistemas digitales.

### Comparación

| Característica            | Analógica                                                 | Digital                                                       |
| ------------------------- | --------------------------------------------------------- | ------------------------------------------------------------- |
| **Valores**               | Continuos                                                 | Discretos                                                     |
| **Representación**        | Onda continua                                             | Valores digitales                                             |
| **Ejemplo**               | Audio                                                     | Datos de computador                                           |
| **Sensibilidad al ruido** | El ruido puede modificar directamente la forma de la onda | Puede recuperar la información mediante procesamiento digital |
| **Uso principal**         | Audio, radio y sensores                                   | Redes, computadores y sistemas digitales                      |

### Conclusión

La principal diferencia entre ambas señales es que la **señal analógica cambia de manera continua**, mientras que la **señal digital representa la información mediante valores discretos**.

Por esta razón, las señales digitales son ampliamente utilizadas en computadores y redes, ya que permiten procesar, almacenar y transmitir información de una manera más sencilla y resistente a ciertos tipos de interferencia.

