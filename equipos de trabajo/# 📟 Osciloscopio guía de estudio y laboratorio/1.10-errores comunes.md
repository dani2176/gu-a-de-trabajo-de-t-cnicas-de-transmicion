# 27.10 · Errores comunes y soluciones

> **Área:** Osciloscopio · Instrumentación y transmisión de señales  
> **Guía:** [Índice y navegación](./README.md)

Cuando una señal no se ve como esperabas, revisa el montaje de forma ordenada. Primero descarta riesgos de conexión; luego revisa sonda, canales, escalas, trigger y limitaciones del equipo.

| Lo que observas | Causa posible | Qué revisar |
|---|---|---|
| No aparece ninguna señal | Canal apagado o escala incorrecta | Activa CH1, revisa conexión y usa AUTOSET |
| La forma de onda se mueve | Trigger inadecuado | Fuente, flanco y nivel de disparo |
| El voltaje es diez veces mayor o menor | Desajuste `1X/10X` | Sonda física y configuración del canal |
| La amplitud es casi el doble de lo previsto | Generador en `50 Ω` con carga alta | Ajusta/consulta `Load = Hi-Z` |
| Los bordes cuadrados se ven deformados | Sonda mal compensada o limitaciones del sistema | Compensación, ancho de banda y conexión |
| Se ve demasiado ruido | Mala referencia, cableado o sensibilidad alta | Conexiones, longitud de tierra y escalas |
| La señal aparece recortada | Escala vertical insuficiente o señal fuera de rango | Aumenta V/div y comprueba límites de entrada |
| La frecuencia aparente es extraña | Muestreo insuficiente o aliasing | Frecuencia de muestreo, escala temporal y memoria |
| El offset desaparece | Acoplamiento `AC` | Vuelve a `DC` |

> [!TIP]
> **Ruta de diagnóstico:** primero comprueba seguridad y conexiones, después canal y factor de sonda, luego escalas y trigger. Por último evalúa las mediciones automáticas.

---

## Límites de los instrumentos: por qué importan

Aunque no siempre haya que modificarlas directamente, estas características influyen en la calidad de una medición:

- **Ancho de banda:** límite de frecuencias que el sistema puede representar con fidelidad especificada. No basta con que la señal “aparezca”.
- **Frecuencia de muestreo (`Sa/s`):** cantidad de muestras por segundo que toma el equipo. Debe ser suficiente para representar la señal y sus cambios rápidos.
- **Profundidad de memoria:** determina cuántas muestras puede conservar el instrumento en una adquisición.
- **Número de canales:** cantidad de señales que puede observar a la vez.
- **Resolución vertical:** cantidad de niveles digitales usados para cuantificar el voltaje.
- **Impedancia de entrada:** puede afectar la señal observada; una sonda pasiva 10X normalmente se utiliza con entradas de alta impedancia compatibles.

**Conexión con teoría:** el criterio de Nyquist señala una condición mínima de muestreo para señales limitadas en banda, pero medir con fidelidad pulsos y transiciones suele exigir márgenes de ancho de banda y muestreo considerablemente mayores. No basta con tomar únicamente dos muestras por ciclo para un análisis práctico completo.

---

## Revisión rápida de tres errores habituales

**Onda inestable:** revisa `TRIGGER Source`, flanco, nivel y modo.

**Voltaje diez veces diferente:** comprueba que la sonda física y el canal estén ambos en `10X` o ambos en `1X`, según corresponda.

**Amplitud aproximadamente duplicada:** comprueba el ajuste de carga `50 Ω`/`Hi-Z` del generador y la impedancia real conectada.

Si existe riesgo eléctrico o desconoces la referencia del circuito, suspende la conexión y consulta al responsable del laboratorio.

---

[← Tema anterior: Ejemplos y prácticas de laboratorio](./27.9-ejemplo-practico.md) | [🏠 Índice del osciloscopio](./README.md) | [Tema siguiente: Evidencias prácticas y registro de resultados →](./27.11-evidencias-practicas.md)
