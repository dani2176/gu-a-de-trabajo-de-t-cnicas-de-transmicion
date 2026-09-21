2.1 Frecuencia
🔄 Concepto

La frecuencia indica cuántos ciclos de una señal periódica ocurren durante un segundo.

Se representa:

[
f
]

y se mide en Hertz:

[
Hz
]

Fórmula

[
f=\frac{1}{T}
]

Donde:

f = frecuencia.
T = período.
Ejemplo

Si:

[
T=0,01s
]

entonces:

[
f=\frac{1}{0,01}
]

[
\boxed{f=100Hz}
]

Desarrollo

Una señal de mayor frecuencia completa más ciclos en el mismo tiempo.

Frecuencia baja:

/¯\____________/¯\

Frecuencia alta:

/¯\_/¯\_/¯\_/¯\_/¯\

Por lo tanto:

[
f\uparrow \Rightarrow T\downarrow
]

y:

[
f\downarrow \Rightarrow T\uparrow
]

🔗 Relación con Telecomunicaciones

La frecuencia es fundamental para distinguir canales de radio, estudiar espectros y determinar el ancho de banda de diferentes sistemas.

2.2 Nivel de señal y amplitud
📈 Concepto

La amplitud representa el nivel instantáneo de una señal respecto de una referencia.

       ▲
       │ Amplitud
       │
      /¯\
     /   \
────/─────\────
Desarrollo

Una señal puede tener:

Valor máximo.
Valor mínimo.
Valor pico.
Valor pico a pico.
Valor eficaz.

La amplitud no debe confundirse con frecuencia.

Amplitud → nivel de la señal

Frecuencia → ciclos por segundo

Una señal puede tener la misma frecuencia pero diferente amplitud:

Señal A:

  /¯\_/¯\_/¯\_

Señal B:

    /¯¯¯\___/¯¯¯\

El patrón temporal puede repetirse a la misma frecuencia, pero el nivel de la señal es diferente.

2.3 dBm
⚡ Concepto

dBm es una unidad logarítmica utilizada para expresar potencia utilizando como referencia:

[
1mW
]

Por definición:

[
0dBm=1mW
]

Keysight utiliza dBm como potencia referenciada a 1 mW. [4]

Fórmula

[
P(dBm)=10\log_{10}\left(\frac{P(mW)}{1mW}\right)
]

Ejemplo

Si:

[
P=10mW
]

entonces:

[
P(dBm)=10\log_{10}(10)
]

[
\boxed{P=10dBm}
]

Valores de referencia
Potencia	dBm
1 mW	0 dBm
10 mW	10 dBm
100 mW	20 dBm
1000 mW	30 dBm
Desarrollo del concepto

dBm es especialmente útil en telecomunicaciones porque permite trabajar con valores de potencia muy grandes o muy pequeños utilizando una escala logarítmica.

Por ejemplo:

1 mW  → 0 dBm
10 mW → 10 dBm
100 mW → 20 dBm

Cada aumento de 10 dB representa un factor 10 en potencia.

⚠️ No confundir
dBm → potencia absoluta referenciada a 1 mW

dB → relación entre dos niveles
2.4 Vpp
⚡ Concepto

Vpp significa Voltaje pico a pico.

Representa la diferencia entre el máximo y el mínimo de una señal.

[
V_{pp}=V_{max}-V_{min}
]

Ejemplo

Si:

[
V_{max}=5V
]

y:

[
V_{min}=-5V
]

entonces:

[
V_{pp}=5-(-5)
]

[
\boxed{V_{pp}=10V}
]

Representación
          Vmax
            ▲
            │
         /¯¯¯¯\
        /      \
───────/────────\──────
      /          \
     /            \
    ▼
   Vmin

<-------- Vpp ------->
Desarrollo del concepto

Vpp permite describir la excursión total de una señal.

Si una onda va desde:

+5 V

hasta:

-5 V

la diferencia es:

10 V

Por eso:

[
V_{pp}=10V
]

2.5 Ancho de banda
📏 Concepto

El ancho de banda es el rango de frecuencias comprendido entre una frecuencia mínima y una frecuencia máxima.

Una expresión sencilla es:

[
BW=f_{max}-f_{min}
]

Ejemplo

Si:

[
f_{min}=2MHz
]

y:

[
f_{max}=10MHz
]

entonces:

[
BW=10-2
]

[
\boxed{BW=8MHz}
]

Representación
fmin                                      fmax
 │                                         │
 ▼                                         ▼
─|=========================================|─
                 8 MHz
Desarrollo

El ancho de banda permite saber qué extensión del espectro utiliza una señal o qué rango de frecuencias puede manejar un sistema.

Por ejemplo:

Señal A
2 MHz ─────────── 4 MHz

BW = 2 MHz

Mientras que:

Señal B
2 MHz ───────────────────── 10 MHz

BW = 8 MHz
🔗 Relación con Shannon

El ancho de banda también aparece en la ecuación de capacidad de Shannon:

[
C=B\log_2(1+SNR)
]

Por lo tanto, el ancho de banda es importante tanto para describir señales como para analizar la capacidad teórica de un canal.

2.6 Velocidad de propagación
🚀 Concepto

La velocidad de propagación indica qué tan rápido una señal se desplaza a través de un medio.

[
v=\frac{d}{t}
]

Donde:

v = velocidad.
d = distancia.
t = tiempo.
Ejemplo

Si una señal recorre:

[
d=100m
]

en:

[
t=0,0000005s
]

entonces:

[
v=\frac{100}{0,0000005}
]

[
\boxed{v=200.000.000m/s}
]

Desarrollo

La velocidad de propagación depende del medio y de las propiedades físicas asociadas a la propagación.

Es importante distinguir:

Velocidad de propagación
≠
Velocidad de transmisión

La velocidad de propagación describe qué tan rápido se desplaza la señal.

La velocidad de transmisión o bit rate describe cuántos bits se transmiten por segundo.

2.7 Atenuación
📉 Concepto

La atenuación es la pérdida de potencia o nivel que experimenta una señal mientras se propaga.

TRANSMISOR
   📡
    │
    │ Señal
    ▼
════════════════════════
        CANAL
      📉 pérdidas
════════════════════════
              │
              ▼
             📥
          RECEPTOR
Fórmula

[
A(dB)=10\log_{10}
\left(
\frac{P_{entrada}}{P_{salida}}
\right)
]

Ejemplo

Si:

[
P_{entrada}=100mW
]

y:

[
P_{salida}=10mW
]

entonces:

[
A=10\log_{10}
\left(
\frac{100}{10}
\right)
]

[
\boxed{A=10dB}
]

Desarrollo del concepto

La atenuación puede relacionarse con:

Distancia.
Características del cable.
Conectores.
Componentes.
Medio de transmisión.

En una comunicación real:

Potencia transmitida
        ↓
     pérdidas
        ↓
Potencia recibida

Por eso un receptor ubicado más lejos puede recibir una señal con menor nivel.

🔗 Relación con Redes

En sistemas cableados la atenuación es una de las razones por las que existen límites de distancia y especificaciones de los medios de transmisión.

2.8 Ruido
📢 Concepto

El ruido es una perturbación no deseada que se mezcla con la señal que se desea recibir.

Señal útil
────────────────

Ruido
~~~~ ~~~~ ~~~~~

Señal recibida
────≈──~──≈────
Desarrollo

Existen diferentes fuentes de ruido.

Entre ellas:

Ruido térmico.
Ruido electrónico.
Interferencias.
Perturbaciones del entorno.

El ruido puede dificultar la recuperación correcta de la información.

Ejemplo

Supongamos que una señal tiene:

Señal = 100 unidades
Ruido = 1 unidad

El ruido es pequeño respecto de la señal.

Pero si:

Señal = 100 unidades
Ruido = 50 unidades

la señal resulta mucho más difícil de distinguir.

Este concepto conduce directamente a la:

[
SNR
]

2.9 Relación señal a ruido — SNR
📶 Concepto

SNR significa:

Signal-to-Noise Ratio

o:

Relación señal a ruido.

Compara la potencia de la señal útil con la potencia del ruido.

[
SNR(dB)=10\log_{10}
\left(
\frac{P_{señal}}{P_{ruido}}
\right)
]

Ejemplo

Si:

[
P_{señal}=100mW
]

y:

[
P_{ruido}=1mW
]

entonces:

[
SNR=10\log_{10}(100)
]

[
\boxed{SNR=20dB}
]

Desarrollo

Una SNR grande significa que la potencia de la señal es mucho mayor que la del ruido.

SNR alta

Señal █████████████
Ruido ██

Una SNR menor significa que el ruido tiene mayor importancia relativa:

SNR baja

Señal ███████
Ruido █████
🔗 Relación con Shannon

SNR aparece en:

[
C=B\log_2(1+SNR)
]

Por lo tanto:

Ruido
 ↓
SNR
 ↓
Capacidad teórica
2.10 Relación portadora a ruido — C/N
📡 Concepto

C/N significa:

Carrier-to-Noise Ratio

o:

Relación portadora a ruido.

Se utiliza para comparar una portadora con el ruido presente en el sistema.

Una forma de expresarlo es:

[
C/N=10\log_{10}
\left(
\frac{P_C}{P_N}
\right)
]

La terminología técnica de ITU define C/N en términos de la relación entre la potencia de la señal o portadora y la potencia de ruido bajo condiciones de medición determinadas. [5]

Desarrollo

Este concepto es muy importante en sistemas donde existe una portadora claramente definida, especialmente en comunicaciones de radio y otros sistemas de RF.

Diferencia
Parámetro	Comparación
SNR	Señal / Ruido
C/N	Portadora / Ruido

El concepto matemático es parecido, pero la señal utilizada como referencia no es necesariamente la misma.