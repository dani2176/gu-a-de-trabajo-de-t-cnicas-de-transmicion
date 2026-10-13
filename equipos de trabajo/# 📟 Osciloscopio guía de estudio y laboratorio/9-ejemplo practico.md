# 27.9 · Ejemplos y prácticas de laboratorio

> **Área:** Osciloscopio · Instrumentación y transmisión de señales  
> **Guía:** [Índice y navegación](./README.md)

Una vez dominada la medición inicial, se pueden comparar distintas formas de onda y dos canales. Las actividades siguientes son **propuestas**, no registros de prácticas ya realizadas.

## Práctica 1 — Señal senoidal de referencia

- **Objetivo:** visualizar una senoidal conocida y medir Vpp, período y frecuencia.
- **Montaje:** generador de baja tensión + osciloscopio + sonda apropiada.
- **Configuración orientativa:** señal de 1 kHz, 4 Vpp, offset 0 V y carga correcta.
- **Mediciones:** captura de pantalla, Vpp, T, f y, si corresponde, Vrms.
- **Comprobación:** compara los valores con los cálculos de [27.7](./27.7-medicion-de-amplitud-frecuencia-y-periodo.md).

## Práctica 2 — Señal cuadrada y ciclo de trabajo

**Objetivo:** diferenciar una señal senoidal de una señal cuadrada y medir su ancho de pulso.

1. Cambia el generador a una señal cuadrada de baja tensión con valores seguros para el equipo.
2. Conserva una frecuencia conocida, por ejemplo `1 kHz`.
3. Observa las transiciones entre nivel bajo y alto.
4. Usa mediciones de `Period`, `Pulse Width` y `Duty Cycle` cuando estén disponibles.

Para una señal con `T = 1 ms` y tiempo alto de `0.4 ms`:

$$
\text{Duty Cycle}=\frac{T_{alto}}{T}\times100\%=\frac{0.4}{1}\times100\%=\boxed{40\%}
$$

**Interpretación:** el pulso está en nivel alto durante el 40 % de cada período. Un aumento de frecuencia no implica por sí solo un aumento del ciclo de trabajo.

## Práctica 3 — Comparación de dos canales

**Objetivo:** observar diferencias de voltaje y tiempo entre dos señales compatibles con las referencias de los canales.

- `CH1`: señal de entrada.
- `CH2`: señal de salida de un circuito de baja tensión apropiado.
- Verifica que **ambos puntos de referencia puedan unirse a la tierra común** del osciloscopio de sobremesa.
- Mide las dos amplitudes y el retraso temporal con cursores.

Si ambas señales son periódicas de la misma frecuencia:

$$
\varphi=360^\circ\frac{\Delta t}{T}
$$

Por ejemplo, `Δt = 0.25 ms` y `T = 1 ms` corresponden a un desplazamiento de `90°`. Para afirmar cuál señal adelanta o retrasa, identifica qué evento ocurre primero en la pantalla.

## Práctica 4 — FFT (solo si el modelo la tiene)

**Objetivo:** distinguir el análisis en dominio del tiempo del análisis en dominio de la frecuencia.

1. Captura una senoidal de frecuencia conocida.
2. Abre la función `FFT` o análisis espectral, si está disponible.
3. Localiza la componente principal alrededor de la frecuencia de la señal.
4. Cambia a una onda cuadrada y observa el espectro, teniendo en cuenta los límites del equipo y su configuración.

**Interpretación:** una onda cuadrada ideal contiene una fundamental y armónicos impares. Los resultados reales dependen del ancho de banda, la resolución espectral y la configuración de adquisición.

---

## Preguntas para el análisis de resultados

1. ¿La forma de onda coincide con la señal seleccionada en el generador?
2. ¿Se observan todos los ciclos esperados a la escala temporal elegida?
3. ¿Coinciden los cálculos manuales con las mediciones automáticas?
4. Si hay diferencias, ¿podrían explicarse por atenuación, terminación de carga o ajustes?

Incluye respuestas basadas en **observaciones de laboratorio** y no únicamente en valores teóricos.

---

[← Tema anterior: Sonda X1 y X10: conexión, compensación y seguridad](./27.8-medicion-con-sonda-x1-y-x10.md) | [🏠 Índice del osciloscopio](./README.md) | [Tema siguiente: Errores comunes y soluciones →](./27.10-errores-comunes.md)
