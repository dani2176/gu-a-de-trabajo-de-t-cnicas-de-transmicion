# 27.4 · Partes y controles del equipo

> **Área:** Osciloscopio · Instrumentación y transmisión de señales  
> **Guía:** [Índice y navegación](./README.md)

Los modelos de osciloscopio presentan paneles distintos, pero sus controles suelen estar agrupados por función. **Compara siempre esta guía con el manual del equipo real.**

Los controles varían de lugar según el modelo, pero se agrupan en cuatro áreas: **vertical, horizontal, disparo (trigger) y adquisición/mediciones**.

| Control o término | Función | Qué ocurre al ajustarlo |
|---|---|---|
| `CH1`, `CH2` | Activa o selecciona un canal | Permite ver una o dos señales |
| `VOLTS/DIV` | Escala vertical | Cambia cuántos voltios representa cada cuadro vertical |
| `VERTICAL POSITION` | Posición vertical | Sube o baja la representación de la señal |
| `SEC/DIV` o `TIME/DIV` | Escala horizontal | Cambia cuánto tiempo representa cada cuadro horizontal |
| `HORIZONTAL POSITION` | Posición horizontal | Desplaza la señal a izquierda/derecha |
| `TRIGGER` | Criterio de captura | Permite mostrar una señal periódica estable |
| `TRIGGER LEVEL` | Umbral de disparo | Define el voltaje al cual se activa el disparo |
| `EDGE / RISING / FALLING` | Tipo y dirección de flanco | Dispara al cruzar un nivel hacia arriba o abajo |
| `COUPLING DC/AC` | Acoplamiento de entrada | Incluye o elimina la componente continua |
| `PROBE 1X/10X` | Factor de sonda | Ajusta la escala indicada al tipo de sonda |
| `MEASURE` | Mediciones automáticas | Muestra frecuencia, período, Vpp, RMS, etc. |
| `CURSORS` | Cursores de medición | Permite medir diferencias manuales de voltaje/tiempo |
| `AUTOSET` | Ajuste automático | Busca una primera presentación útil de la señal |
| `RUN/STOP` | Control de adquisición | Inicia o congela la captura |
| `SINGLE` | Captura única | Registra un evento si se cumple la condición de disparo |

## Esquema orientativo del panel

```text
┌───────────────────────────────────────────────────┐
│                      PANTALLA                     │
│        Voltaje (vertical) / Tiempo (horizontal)   │
└───────────────────────────────────────────────────┘
  [CH1] [CH2]   [VOLTS/DIV]   [TIME/DIV]  [TRIGGER]
                   Vertical     Horizontal  Disparo
                 [MEASURE] [CURSORS] [AUTOSET]
```

> **Importante:** este diagrama representa las **zonas funcionales** habituales; no reproduce la posición real de ningún fabricante.

## Qué debes identificar al tomar una fotografía del equipo

1. Pantalla y escala vertical/horizontal.
2. Conector del canal utilizado (`CH1`, por ejemplo).
3. Control de `VOLTS/DIV`.
4. Control de `TIME/DIV`.
5. Controles de `TRIGGER`.
6. Menús de sonda, acoplamiento y mediciones automáticas.

Puedes añadir una fotografía propia y rotularla después de identificar el modelo del laboratorio.

---

[← Tema anterior: Funciones principales](./27.3-funciones-principales.md) | [🏠 Índice del osciloscopio](./README.md) | [Tema siguiente: Configuración inicial →](./27.5-configuracion-inicial.md)
