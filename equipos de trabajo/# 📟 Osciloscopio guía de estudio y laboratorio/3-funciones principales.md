# 27.3 · Funciones principales

> **Área:** Osciloscopio · Instrumentación y transmisión de señales  
> **Guía:** [Índice y navegación](./README.md)

Esta sección explica **qué hace cada función** y cómo afecta a la visualización. Si lo que necesitas es localizar físicamente los botones, consulta la [sección de partes y controles](./27.4-partes-y-controles.md).

## 3.1 Escala vertical: `VOLTS/DIV`

Indica los voltios que corresponden a **una división vertical**. Por ejemplo, si la señal ocupa cuatro divisiones desde el máximo hasta el mínimo con `1 V/div`:

$$
V_{pp}=4\ \text{div}\times1\ \frac{V}{\text{div}}=\boxed{4\ V}
$$

**Ojo:** mover la posición vertical no modifica el voltaje real. Solo desplaza la imagen en pantalla.

## 3.2 Escala horizontal: `TIME/DIV`

Indica cuánto tiempo corresponde a **una división horizontal**. Si un ciclo completo ocupa cuatro divisiones con `250 µs/div`:

$$
T=4\ \text{div}\times250\ \frac{\mu s}{\text{div}}=1000\ \mu s=\boxed{1\ ms}
$$

## 3.3 Disparo o `trigger`

El disparo define **en qué condición el instrumento organiza una captura**. Para una senoidal sencilla, lo habitual es seleccionar el canal de entrada, disparo por flanco y un nivel que la señal atraviese periódicamente.

**Ejemplo:** `Source = CH1`, `Type = Edge`, `Slope = Rising`, `Level ≈ 0 V`, `Mode = Auto`.

Si la onda se desplaza o parece inestable, revisa primero la fuente, el nivel y el modo del trigger. Si no se ve nada en modo Normal, el equipo podría estar esperando la condición de disparo.

## 3.4 Acoplamiento `DC` y `AC`

- **DC:** conserva en pantalla la componente continua y la variable. Es el ajuste recomendado para comenzar.
- **AC:** reduce o elimina la componente continua mediante un acoplamiento pasa-altos; facilita observar señales pequeñas sobre un offset grande, pero puede alterar señales de frecuencia baja.

**Ejemplo:** una onda senoidal de `2 Vpp` con `+1 V` de offset varía aproximadamente entre `0 V` y `+2 V`. En `DC` se aprecia que está desplazada hacia arriba. En `AC`, su posición media se aproxima a `0 V` si la frecuencia es suficientemente alta para ese acoplamiento.

---

## Funciones de adquisición y medición

- **`MEASURE`:** calcula automáticamente magnitudes como frecuencia, período y Vpp, según el modelo.
- **`CURSORS`:** permite medir manualmente intervalos verticales (ΔV) y horizontales (Δt).
- **`AUTOSET`:** propone un ajuste de visualización; es un punto de partida, no una garantía de medición correcta.
- **`RUN/STOP`:** inicia o congela la adquisición.
- **`SINGLE`:** solicita una captura asociada a una condición de disparo.

## Ejemplo rápido de selección de controles

Si la onda está muy pequeña, revisa `VOLTS/DIV`. Si solo ves un pequeño fragmento de un ciclo, revisa `TIME/DIV`. Si la onda se mueve lateralmente, revisa `TRIGGER`. Si el valor medido difiere por un factor de diez, revisa `PROBE 1X/10X`.

---

[← Tema anterior: ¿Para qué se utiliza?](./27.2-para-que-se-utiliza.md) | [🏠 Índice del osciloscopio](./README.md) | [Tema siguiente: Partes y controles del equipo →](./27.4-partes-y-controles.md)
