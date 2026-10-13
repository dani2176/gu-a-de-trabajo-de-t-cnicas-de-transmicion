# 27.11 · Evidencias prácticas y registro de resultados

> **Área:** Osciloscopio · Instrumentación y transmisión de señales  
> **Guía:** [Índice y navegación](./README.md)

Esta sección explica cómo respaldar la práctica para que cualquier compañero, profesor o lector pueda entender **qué se midió**, **cómo se configuró el equipo** y **qué resultados se obtuvieron**.

Una práctica técnica debe indicar **qué se quiso medir, cómo se configuró el equipo, qué se observó y cómo se interpreta**. Las fotografías sin explicación no demuestran por sí solas el procedimiento.

## Plantilla de mediciones

| Magnitud | Valor esperado | Valor medido | Instrumento/ajuste | Observaciones |
|---|---:|---:|---|---|
| `Vpp` | 4.00 V | Pendiente | CH1, 10X, DC | — |
| `T` | 1.00 ms | Pendiente | 250 µs/div | — |
| `f` | 1.00 kHz | Pendiente | Medida automática/manual | — |
| `Vrms` (senoidal sin offset) | 1.41 V | Pendiente | Medición RMS correspondiente | — |

**Importante:** reemplaza `Pendiente` solo por los valores obtenidos en el laboratorio. No presentes los cálculos teóricos como mediciones reales.

## Capturas recomendadas

1. **Equipo:** fotografía de marca, modelo y conexiones.
2. **Configuración:** fotografía legible de CH1, sonda, V/div, s/div y trigger.
3. **Onda senoidal:** captura completa con la señal visible y estabilizada.
4. **Mediciones:** captura de `Vpp`, `Period` y `Frequency`.
5. **Comparación:** captura de onda cuadrada o dos canales, si se realizó esa práctica.
6. **Conclusión:** breve análisis sobre lo esperado, lo observado y posibles diferencias.

## Cómo insertar una fotografía en esta sección

Crea una carpeta opcional `imagenes/` dentro de `27-osciloscopio/` y utiliza una ruta relativa: 

```markdown
![Osciloscopio con señal senoidal de 1 kHz](./imagenes/senoidal-1khz.jpg)
```

Acompaña la fotografía con un texto que indique el canal, las escalas y la lectura observada. Sustituye el nombre de ejemplo por el archivo real que hayas subido.

## Autoevaluación

1. ¿Qué representan los ejes vertical y horizontal del osciloscopio?
2. ¿Por qué cambiar `V/div` no significa cambiar el voltaje del generador?
3. ¿Cómo obtendrías `Vpp` utilizando las divisiones de pantalla?
4. ¿Por qué hay que hacer coincidir el factor `10X` entre sonda y osciloscopio?
5. ¿Qué ocurre si el trigger está configurado en un nivel que la señal nunca cruza?
6. ¿Qué diferencia existe entre acoplamiento `AC` y `DC`?
7. ¿Por qué no se debe colocar la pinza de tierra sobre un conductor energizado en un osciloscopio de sobremesa convencional?
8. Si `T = 0.5 ms`, ¿cuál es la frecuencia?
9. ¿Por qué podría observarse `4 Vpp` si el generador indica `2 Vpp`?
10. ¿Qué aporta el osciloscopio al estudio de transmisión de señales que un multímetro no muestra de la misma manera?

<details>
<summary><strong>✅ Respuesta del cálculo de la pregunta 8</strong></summary>

$$
f=\frac{1}{0.0005\ s}=2000\ Hz=2\ kHz
$$

</details>

---

## Cómo cerrar la práctica

Escribe una conclusión con tres elementos: **resultado esperado**, **resultado medido** e **interpretación de la diferencia**, si la hubo. Evita inventar lecturas o mostrar el ejemplo teórico como evidencia propia.

---

[← Tema anterior: Errores comunes y soluciones](./27.10-errores-comunes.md) | [🏠 Índice del osciloscopio](./README.md)
