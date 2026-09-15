# 2. Parámetros Técnicos de Transmisión

Los parámetros técnicos permiten describir y analizar las características de una señal y de un enlace de comunicación.

---

## 2.1 Frecuencia

La frecuencia indica cuántos ciclos de una señal ocurren por segundo.

### Símbolo

**f**

### Unidad

**Hertz (Hz)**

### Fórmula

La frecuencia se puede calcular mediante la siguiente fórmula:

$$
f = \frac{1}{T}
$$

Donde:

- **f** = frecuencia, medida en Hertz (Hz).
- **T** = período, medido en segundos (s).

### Ejemplo

Si una señal tiene un período de:

$$
T = 0,01\ s
$$

Entonces:

$$
f = \frac{1}{0,01}
$$

Por lo tanto:

$$
f = 100\ Hz
$$

### Interpretación

La señal realiza **100 ciclos por segundo**.

La frecuencia y el período son magnitudes inversamente proporcionales. Por lo tanto, mientras menor sea el período, mayor será la frecuencia.

---

## 2.2 Nivel de señal

El nivel de señal indica la magnitud de una señal y puede expresarse utilizando diferentes unidades, dependiendo de lo que se quiera medir.

En este trabajo se utilizan principalmente:

- **dBm** para expresar potencia.
- **Vpp** para expresar tensión o voltaje pico a pico.

---

## 2.3 dBm

dBm es una unidad utilizada para expresar potencia tomando como referencia **1 mW (miliwatt)**.

### Fórmula

$$
P(dBm) = 10\log_{10}\left(\frac{P(mW)}{1mW}\right)
$$

### Ejemplo

Si tenemos una potencia de:

$$
P = 10\ mW
$$

Entonces:

$$
P(dBm) = 10\log_{10}(10)
$$

Por lo tanto:

$$
P(dBm) = 10\ dBm
$$

### Valores de referencia

| Potencia | dBm |
|---:|---:|
| 1 mW | 0 dBm |
| 10 mW | 10 dBm |
| 100 mW | 20 dBm |

### Interpretación

El valor en dBm permite expresar diferentes niveles de potencia utilizando una escala logarítmica con referencia de **1 mW**.

---

## 2.4 Vpp

Vpp significa **voltaje pico a pico**.

Representa la diferencia entre el valor máximo y el valor mínimo de una señal.

### Fórmula

$$
V_{pp} = V_{max} - V_{min}
$$

### Ejemplo

Si:

$$
V_{max} = 5\ V
$$

y:

$$
V_{min} = -5\ V
$$

Entonces:

$$
V_{pp} = 5 - (-5)
$$

Por lo tanto:

$$
V_{pp} = 10\ V
$$

### Representación

```text
             Vmax
               ▲
               │
               │      ╭──╮
               │     ╱    ╲
───────────────┼────╯      ╰──────
               │
               │     ╲    ╱
               │      ╰──╯
               │
               ▼
             Vmin

        <──────────────>
               Vpp
---
Interpretación

El voltaje pico a pico corresponde a la diferencia total entre el valor máximo y el valor mínimo de la señal.
---
