# 📚 Teoría de Transmisión de Señales — Índice pedagógico

Esta colección contiene **20 secciones principales de teoría**, organizadas en una secuencia progresiva. Cada sección comienza con una explicación introductoria y continúa con el desarrollo técnico, ejemplos, cálculos, relaciones y advertencias sobre errores frecuentes.

La organización busca que un estudiante que todavía no domina Telecomunicaciones pueda avanzar desde la información y los bits hasta las señales, la modulación, Shannon, Nyquist, ADC y los tipos de transmisión sin tener que saltar entre temas para completar conceptos previos.

## 🟢 Bloque 1 — Fundamentos de información y señales

| Sección | Tema |
|---|---|
| [1.0](1.0-introduccion-comunicacion.md) | Introducción a la comunicación y la información |
| [1.1](1.1-informacion-bits-bytes.md) | Información, datos, bits y bytes |
| [1.2](1.2-senales-medios-canal.md) | Señales, medios y canal de comunicación |
| [1.3](1.3-onda-y-senal-sinusoidal.md) | La onda y la señal sinusoidal |
| [1.4](1.4-senal-analogica-digital.md) | Señal analógica y señal digital |
| [1.5](1.5-parametros-forma-onda.md) | Amplitud, pico, Vpp, período y frecuencia |
| [1.6](1.6-dominio-del-tiempo.md) | Dominio del tiempo |
| [1.7](1.7-dominio-frecuencia-fourier.md) | Dominio de la frecuencia, espectro y Fourier |

### 🔗 Secuencia conceptual

```text
Información
   ↓
Bits y bytes
   ↓
Señal
   ↓
Onda
   ↓
Analógica / Digital
   ↓
Amplitud + período + frecuencia
   ↓
Dominio del tiempo
   ↓
Dominio de la frecuencia
   ↓
Fourier
```

---

## 🔵 Bloque 2 — Parámetros técnicos de transmisión

| Sección | Tema |
|---|---|
| [2.0](2.0-nivel-dbm-vpp.md) | Nivel de señal, potencia, dB, dBm y Vpp |
| [2.1](2.1-ancho-de-banda.md) | Ancho de banda |
| [2.2](2.2-propagacion-longitud-onda.md) | Velocidad de propagación y longitud de onda |
| [2.3](2.3-atenuacion.md) | Atenuación y presupuesto de potencia |
| [2.4](2.4-ruido-snr-cn.md) | Ruido, SNR y C/N |

### 🔗 Secuencia conceptual

```text
Nivel
 ↓
dB / dBm / Vpp
 ↓
Ancho de banda
 ↓
Propagación
 ↓
Atenuación
 ↓
Ruido
 ↓
SNR / C/N
```

---

## 🟣 Bloque 3 — Mecanismos de transmisión y modulación

| Sección | Tema |
|---|---|
| [3.0](3.0-banda-base-codificacion.md) | Banda base y codificación |
| [3.1](3.1-modulacion-portadora.md) | Modulación y señal portadora |
| [3.2](3.2-am-fm.md) | Modulación AM y FM |
| [3.3](3.3-modulacion-digital-baud-bit-rate.md) | Modulación digital, símbolos, baud y bit rate |

### 🔗 Secuencia conceptual

```text
Datos
 ↓
Codificación
 ↓
Banda base
 ↓
Portadora
 ↓
Modulación
 ↓
AM / FM
 ↓
ASK / FSK / PSK / QAM
 ↓
Símbolos / Baud / Bit rate
```

---

## 🟠 Bloque 4 — Fundamentos matemáticos y conversión

| Sección | Tema |
|---|---|
| [4.0](4.0-shannon-capacidad.md) | Teoría de Shannon y capacidad de canal |
| [4.1](4.1-nyquist-muestreo-aliasing-adc.md) | Nyquist-Shannon, muestreo, aliasing y conversión A/D |

### 🔗 Secuencia conceptual

```text
BW + SNR
   ↓
Shannon
   ↓
Capacidad

Señal analógica
   ↓
Nyquist
   ↓
Muestreo
   ↓
Aliasing / Filtro
   ↓
ADC
   ↓
Cuantización
   ↓
Codificación
```

---

## 🟤 Bloque 5 — Tipos de transmisión y aplicación

| Sección | Tema |
|---|---|
| [5.0](5.0-tipos-transmision-ejemplos.md) | Tipos de transmisión y ejemplos integradores |

Dentro de esta sección se encuentran los contenidos de:

- Transmisión serie.
- Transmisión paralela.
- Transmisión síncrona.
- Transmisión asíncrona.
- Comparaciones.
- Ejemplo de llamada telefónica.
- Ejemplo de radio AM/FM.
- Ejemplo de transmisión de datos.
- Relaciones generales entre conceptos.

---

# 📖 Material complementario

| Archivo | Uso |
|---|---|
| [Glosario](APENDICES/21-glosario.md) | Repaso rápido de términos |
| [Referencias](APENDICES/22-referencias.md) | Fuentes técnicas |
| [Resumen para la defensa](APENDICES/23-resumen-defensa.md) | Preparación para preguntas |

---

# 🎯 Ruta recomendada de estudio

```text
1️⃣ Entender qué es información
        ↓
2️⃣ Entender bits y bytes
        ↓
3️⃣ Entender qué es una señal
        ↓
4️⃣ Entender qué es una onda
        ↓
5️⃣ Aprender amplitud, período y frecuencia
        ↓
6️⃣ Aprender tiempo y frecuencia
        ↓
7️⃣ Comprender Fourier
        ↓
8️⃣ Aprender nivel, ancho de banda y propagación
        ↓
9️⃣ Comprender atenuación y ruido
        ↓
🔟 Comprender SNR y C/N
        ↓
1️⃣1️⃣ Estudiar banda base y codificación
        ↓
1️⃣2️⃣ Estudiar portadora y modulación
        ↓
1️⃣3️⃣ Estudiar AM y FM
        ↓
1️⃣4️⃣ Estudiar modulación digital
        ↓
1️⃣5️⃣ Conectar símbolos, baud y bit rate
        ↓
1️⃣6️⃣ Estudiar Shannon
        ↓
1️⃣7️⃣ Estudiar Nyquist y muestreo
        ↓
1️⃣8️⃣ Comprender aliasing
        ↓
1️⃣9️⃣ Comprender ADC
        ↓
2️⃣0️⃣ Comparar tipos de transmisión
```
