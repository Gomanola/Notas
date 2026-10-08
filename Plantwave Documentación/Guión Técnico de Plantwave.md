# PLANTWAVE: GENERADOR DE MÚSICA DESDE PLANTAS

# INTRODUCCIÓN

PlantWave es un proyecto que convierte una planta viva en un instrumento musical. Cuando tocas o mueves la planta, esta genera música automáticamente.

**¿Cómo funciona?** Un pequeño dispositivo llamado Arduino mide cambios eléctricos naturales de la planta, una computadora traduce esos cambios a instrucciones musicales, y el resultado es música que escuchas en tiempo real.

# ¿QUÉ ES ARDUINO?

## Definición

Arduino es una **pequeña computadora que lee y controla el mundo físico**. No es como una laptop que juega videos o navega internet. Arduino está diseñado específicamente para:

- Leer sensores (temperatura, luz, electricidad, humedad)
- Controlar dispositivos (motores, luces, relés)
- Procesar esa información muy rápidamente

## ¿Cómo es físicamente?

Arduino es una **placa de circuitos pequeña** (aproximadamente 7cm x 5cm) que contiene:

- Una **procesador ATmega328P** (el "cerebro")
- **Pines de conexión** (puertos para conectar el mundo exterior)
- **Cristal de 16MHz** (reloj que marca el tiempo)
- **Regulador de voltaje** (mantiene la energía estable)
- **Convertidor Analógico-Digital (ADC)** (Para convertir las señales analógicas que entran en los puertos A0, A1, A2.... en señales digitales que podamos manipular)
- **Conector USB** (para comunicarse con tu computadora)

# MÁS SOBRE EL ARDUINO

![[Pasted image 20260624043101.png]]

## Botón de Reinicio (Reset Button)

- **Ubicación:** Arriba a la izquierda
- **Función:** Reinicia el Arduino sin desconectar la energía
- **En nuestro proyecto:** Se puede usar para reiniciar la lectura del sensor

## Conector USB Estándar B

- **Ubicación:** Esquina inferior izquierda
- **Función:** Se conecta a la computadora
- **En nuestro proyecto:** Por aquí Arduino envía los datos que lee de la planta a tu computadora

## ATmega328P (El Procesador Principal)

- **Ubicación:** Centro de la placa
- **Función:** Es el "cerebro" de Arduino. Ejecuta el código que programamos
- **En nuestro proyecto:** Lee constantemente el pin A1, procesa la información, y la envía

## Cristal de 16MHz

- **Ubicación:** Cerca del procesador (componente gris rectangular)
- **Función:** Es como el "corazón" que marca el tiempo
- **Velocidad:** Realiza 16 millones de operaciones por segundo
- **En nuestro proyecto:** Asegura que Arduino lea exactamente 200 veces por segundo

## ATmega16u2 (Controlador USB)

- **Ubicación:** Abajo a la izquierda
- **Función:** Traduce datos entre Arduino y la computadora a través del USB
- **En nuestro proyecto:** Permite que Arduino se comunique con Python

## Regulador de Voltaje

- **Ubicación:** Lado derecho (componente azul pequeño)
- **Función:** Asegura que el voltaje sea exactamente 5 voltios
- **En nuestro proyecto:** Estabiliza la energía para que las lecturas sean precisas

## Pines de Referencia y Tierra

- **Pin de 0 VDC (Tierra/GND):** El punto de referencia eléctrica cero
- **Pin de 5 VDC:** Proporciona 5 voltios
- **En nuestro proyecto:** Estos pines son CRÍTICOS para conectar los jumpers a la planta

## Pines Analógicos (A0-A5)

- **Ubicación:** Lado derecho, abajo
- **Cantidad:** 6 pines (A0 hasta A5)
- **En nuestro proyecto:** Usamos **A1** para leer la resistencia de la planta
- **¿Por qué analógicos?** Pueden leer valores entre 0 y 5 voltios (no solo encendido/apagado)

## Pines Digitales (0-13)

- **Ubicación:** Lado derecho, arriba
- **Función:** Solo pueden ser encendido (5V) o apagado (0V)
- **En nuestro proyecto:** No los usamos, pero son útiles para controlar LED o motores

## Pines PWM (con símbolo ~)

- **Ubicación:** Pines digitales 3, 5, 6, 9, 10, 11
- **Función:** Pueden simular valores entre 0-5V usando pulsos rápidos
- **En nuestro proyecto:** No los usamos

## Comunicación I2C (A4 → SDA, A5 → SCL)

- **Ubicación:** Pines A4 y A5
- **Función:** Protocolo especial para conectar varios sensores
- **En nuestro proyecto:** No lo usamos (solo usamos A1)

## Pin de Referencia Analógica

- **Función:** Define el voltaje máximo que Arduino mide
- **En nuestro proyecto:** Por defecto es 5V (no lo cambiamos)

# ¿CÓMO LEE ARDUINO LA ELECTRICIDAD?

## El Flujo de Voltaje

Cuando conectas los jumpers a la planta:

```
PLANTA (con agua y iones eléctricos)
    ↓
Jumper 1 (conectado a Pin A1)
    ↓
Arduino mide: 0 a 5 VOLTIOS
    ↓
Convertidor Analógico-Digital (ADC) de Arduino
    ↓
Convierte: 0-5V → 0-1023 (números que comprende la computadora)
    ↓
Jumper 2 (conectado a GND/Tierra)
```

## ¿Qué es el Convertidor Analógico-Digital (ADC)?

La planta produce un **voltaje continuo** (analógico): puede ser 0V, 1.5V, 3.27V, 4.99V, etc. (infinitos valores posibles entre 0 y 5)

Pero Arduino es una **computadora digital**, solo entiende números enteros: 0, 1, 2, 3, ... 1023

### Equivalencias de voltaje con valores convertidos entre 0 y 1023

```
Voltaje Analógico         Convertidor ADC         Número Digital
(continuo)                (10-bit)                (discreto)

0.0V         ───────────→    0
0.5V         ───────────→   102
1.0V         ───────────→   205
1.5V         ───────────→   307
2.0V         ───────────→   410
2.5V         ───────────→   512
3.0V         ───────────→   614
3.5V         ───────────→   717
4.0V         ───────────→   819
4.5V         ───────────→   921
5.0V         ───────────→   1023
```

### ¿Por qué 0-1023?

Arduino tiene un convertidor de **10 bits**. Un bit es como una posición que puede ser 0 o 1.

Con 10 bits, tienes: 2^10 = **1024 posiciones** (0 a 1023)

Por eso el rango es exactamente 0-1023.

```
	0000000000 ───────────→ 0
	0000000001 ───────────→ 1
	0000000010 ───────────→ 2
	0000000011 ───────────→ 3
	0000000100 ───────────→ 4
	.
	.
	.
	1111111100 ───────────→ 1020
	1111111101 ───────────→ 1021
	1111111110 ───────────→ 1022
	1111111111 ───────────→ 1023
```
### Fórmula

```
Número Digital = (Voltaje Medido / Voltaje Máximo) × 1023

Sustitución:
Número Digital = (Voltaje Medido / 5) × 1023

Ejemplo:
Si el voltaje actual es 2.5V:
Número = (2.5 / 5) × 1023 = 0.5 × 1023 = 511.5 ≈ 512
```

## Velocidad de Lectura

Arduino puede hacer esta conversión **muy rápidamente**. En nuestro programa:

- Arduino lee A1: **200 veces por segundo**
- Cada lectura toma: ~0.005 segundos (5 milisegundos)
- Esto es **imperceptible para el humano**, así que parece tiempo real

# CÓMO LA PLANTA GENERA VOLTAJE

Las células vivas de la planta contienen:

- **Agua** con iones disueltos (iones = partículas cargadas eléctricamente)
- **Membranas celulares** que permiten el paso selectivo de iones
- Un **potencial eléctrico natural** entre el interior y exterior de las células

## Cambios de Resistencia

**Resistencia = cuánto "cuesta" que la electricidad fluya**

Cuando tocas la planta:

```
SIN CONTACTO (planta sola):
Jumper 1 → [Aire] → Planta → [Aire] → Jumper 2
Resistencia: MUY ALTA (~1 megaohmio)
Arduino lee: Casi 5V (porque no hay contacto)
Número: ~1000-1023
```

```
CON CONTACTO (tus dedos mojados):
Jumper 1 → [Tu dedo mojado] → Planta → [Tu dedo mojado] → Jumper 2
Resistencia: BAJA (~100 kilohmios)
Arduino lee: Menos voltaje (el voltaje "cae" en la resistencia)
Número: ~200-400
```

## Ley de Ohm

```
Voltaje = Corriente × Resistencia
V = I × R

En nuestro caso:
5V = I × Resistencia
Si Resistencia es ALTA → Voltaje en A1 es ALTO (cercano a 5V = 1023)
Si Resistencia es BAJA → Voltaje en A1 es BAJO (cercano a 0V = 0-200)
```

# FLUJO COMPLETO DEL PROYECTO

## Visión General

```
┌──────────────────────────────────────────────────────────────────┐
│                      PLANTWAVE - FLUJO COMPLETO                  │
└──────────────────────────────────────────────────────────────────┘

HARDWARE (MUNDO FÍSICO)
    │
    ├─ Planta (genera voltaje natural)
    │   ↓
    ├─ Jumpers (conducen voltaje)
    │   ↓
    ├─ Arduino (mide voltaje)
    │   ↓ (0-5V)
    ├─ Convertidor ADC (convierte a 0-1023)
    │   ↓
    └─ Cable USB (envía datos)
        ↓
SOFTWARE (COMPUTADORA)
    │
    ├─ Python (recibe números 0-1023)
    │   ↓
    ├─ Invierte valores (1023 - x)
    │   ↓
    ├─ Detecta planta conectada
    │   ↓
    ├─ Suaviza señal
    │   ↓
    ├─ Calcula cambios
    │   ↓
    ├─ Convierte a notas musicales
    │   ↓
    ├─ Genera ondas de sonido
    │   ↓
    └─ Altavoz (reproduce música)
```

# PROCESAMIENTO EN LA COMPUTADORA (PASO A PASO)

Cada 5 milisegundos (200 veces por segundo), esto ocurre:

## Paso 1: Recepción

```
Arduino envía: "512" (número entre 0-1023)
Python recibe: número en variable "raw_value"
```

## Paso 2: Inversión

```
raw_value = 512
inverted_value = 1023 - 512 = 511

¿POR QUÉ?
Sin inversión:
- Sin contacto: 1000+ (arriba en gráfico) - Confuso
- Con contacto: 200 (abajo en gráfico) - Confuso

CON INVERSIÓN:
- Sin contacto: 0-23 (abajo en gráfico) - Lógico
- Con contacto: 800+ (arriba en gráfico) - Lógico
```

## Paso 3: Detección de Conexión

```
¿El valor está entre 10 y 980?
    SÍ → signal_active = VERDADERO (hay planta)
    NO → signal_active = FALSO (sin conexión)

Esto se muestra como:
    Verde: "Señal ACTIVA"
    Rojo: "Señal INACTIVA"
```

## Paso 4: Suavizado (Smoothing)

```
Valores brutos del Arduino: 500, 520, 490, 510, 495, 515, 505, 520, ...

Se promedian los últimos 15 valores:
(500+520+490+510+495+515+505+520+...) / 15 = 507.33

Valor suavizado: 507

BENEFICIO:
- Elimina fluctuaciones de ruido eléctrico
- Música más fluida
- Sin "saltitos" innecesarios
```
## Paso 5: Detección de Cambio (Trigger)
```
Lectura anterior: 507
Lectura actual: 508

¿El valor CAMBIÓ?
    507 ≠ 508?
    SÍ → Generar nota musical inmediatamente
    NO → Mantener sonido anterior o silencio

NOTA IMPORTANTE:
El programa NO usa un umbral de magnitud (como "cambio > 20")
Sino un sistema de TRIGGER: cualquier cambio genera una nota
```

### ¿Cómo funciona el trigger?

```
Sistema de comparación simple:
if (valor_anterior) != (valor_actual):
    generar_nota = VERDADERO
else:
    generar_nota = FALSO
```

### Ejemplo en tiempo real:

```
Lectura 1: 512
Lectura 2: 512 → ¿512 ≠ 512? NO → Sin cambio, sin nota nueva
Lectura 3: 512 → ¿512 ≠ 512? NO → Sin cambio, sin nota nueva
Lectura 4: 513 → ¿512 ≠ 513? SÍ → ¡¡NUEVA NOTA!!
Lectura 5: 513 → ¿513 ≠ 513? NO → Sin cambio, continúa nota anterior
Lectura 6: 514 → ¿513 ≠ 514? SÍ → ¡¡NUEVA NOTA!!
Lectura 7: 513 → ¿514 ≠ 513? SÍ → ¡¡NUEVA NOTA!!
Lectura 8: 512 → ¿513 ≠ 512? SÍ → ¡¡NUEVA NOTA!!
```

## Paso 7: Conversión a Nota Musical

El programa  utiliza MIDI de 0 a 127
```
Valor (0-1023) → Nota MIDI (0-127) → Frecuencia → Sonido

Mapeo:
Valor 0    → Nota 36 (DO muy bajo)
Valor 512  → Nota 66 (FA central)
Valor 1023 → Nota 96 (DO muy alto)

Fórmula:
nota = 36 + (valor / 1023) × (96 - 36)
nota = 36 + (valor / 1023) × 60
```
### ¿Por qué se mapea a MIDI 36 a 96?

- Porque las notas de 0 a 35 son notas extremadamente bajas menores a 8Hz, inaudible para  el oído humano, a ese punto más que nadas son vibraciones.
- Y las notas de 97 a 127 son notas extremadamente altas mayores a 10kHz, lo cuál es un sonido silbante muy desagradable para el oído humano

### Tabla de conversión

| Valor Arduino | Cálculo | Nota MIDI | Nombre | Frecuencia |
| ------------- | ------- | --------- | ------ | ---------- |
| 0             | 36 + 0  | 36        | DO2    | 65.41 Hz   |
| 102           | 36 + 6  | 42        | FA2    | 92.50 Hz   |
| 205           | 36 + 12 | 48        | DO3    | 130.81 Hz  |
| 307           | 36 + 18 | 54        | FA3    | 185.00 Hz  |
| 410           | 36 + 24 | 60        | DO4    | 261.63 Hz  |
| 512           | 36 + 30 | 66        | FA4    | 370.00 Hz  |
| 614           | 36 + 36 | 72        | DO5    | 523.25 Hz  |
| 716           | 36 + 42 | 78        | FA5    | 739.99 Hz  |
| 819           | 36 + 48 | 84        | DO6    | 1046.50 Hz |
| 921           | 36 + 54 | 90        | FA6    | 1479.98 Hz |
| 1023          | 36 + 60 | 96        | DO7    | 2093.00 Hz |

## Paso 8: Actualización del Gráfico

```
Se dibuja un nuevo punto:
├─ Posición horizontal: tiempo actual (segundos)
├─ Posición vertical: valor suavizado (0-1023)
├─ Color: verde si signal_active, gris si no
└─ Se muestra el último 10 segundos

El gráfico se redibuja cada 50ms para verse suave
```
**Nota**: En versiones anteriores el gráfico se dibujaba 200 veces por segundo (cada 5ms o 0.005 segundos), la misma cantidad de veces que el arduino manda datos en un segundo, causando que el procesador de la computadora se saturara, esto se cambió a que el gráfico se dibuje 20 por segundo (cada 50ms 0.050 segundos), 20 veces por segundo no es un cambio perceptible para el ojo humano, eficientando así el programa.
# PARTE 8: ARCHIVOS MIDI

## ¿Qué es MIDI?

**MIDI = Interfaz Digital de Instrumentos Musicales**

Es un estándar internacional.
No es un audio grabado (como .mp3). Es una **"partitura digital"**.

```
Archivo MP3:
├─ Almacena: Ondas de sonido completas
└─ Tamaño: ~5MB por minuto

Archivo MIDI:
├─ Almacena: Instrucciones (qué nota, cuándo, cuánto)
└─ Tamaño: ~10KB por minuto
```

## Estructura de un MIDI

```
plantwave.mid:
├─ BPM: 120 (tempo)
├─ Eventos:
│  ├─ Tiempo: 0.5s → Nota ON (DO, nota 60, intensidad 100)
│  ├─ Tiempo: 0.8s → Nota OFF (DO)
│  ├─ Tiempo: 0.8s → Nota ON (RE, nota 62, intensidad 110)
│  ├─ Tiempo: 1.1s → Nota OFF (RE)
│  └─ ... (más notas)
└─ Fin
```

## Velocidad MIDI

Cada nota tiene una **velocidad** (0-127):

```
Velocidad 0   = Nota muda (silencio)
Velocidad 64  = Volumen normal
Velocidad 127 = Volumen máximo

En PlantWave:
Velocidad = (Valor del Sensor / 1023) × 127
```

# ANALOGÍA FINAL

**PlantWave es como un "traductor automático bilingüe":**

```
Lenguaje de la Planta:
├─ Resistencia eléctrica
├─ Cambios de voltaje
├─ Pulsaciones eléctricas naturales
└─ (La planta no sabe que es música)

Arduino (Oído):
└─ Escucha y mide esos cambios
   └─ Convierte voltaje en números

Python (Cerebro):
└─ Recibe esos números
  └─ Los procesa y entiende
   └─ Traduce a "lenguaje de música"

Altavoz (Voz):
└─ Reproduce la traducción
  └─ El humano escucha música

RESULTADO:
La planta sigue siendo ella misma (pulsando electricidad naturalmente)
Pero nosotros la escuchamos cantar 🎵
```

# CONCLUSIÓN

PlantWave demuestra que **la tecnología puede hacer "hablar" a la naturaleza**.

Cada planta es única:

- Diferentes resistencias eléctricas
- Diferentes patrones de cambio
- Diferentes "canciones"

Es como descubrir que cada planta tiene **su propia voz musical**, esperando a ser escuchada.

# CONCEPTOS CLAVE

|Concepto|Explicación|
|---|---|
|**Arduino**|Computadora pequeña que lee voltaje (0-5V)|
|**Pin A1**|Entrada analógica que mide el voltaje de la planta|
|**Convertidor ADC**|Convierte 0-5V en números 0-1023|
|**Signal_active**|Detecta si hay planta conectada (10-980)|
|**Smoothing**|Promedia valores para suavizar|
|**Threshold**|Cambio mínimo necesario para sonar (20)|
|**MIDI**|Formato de partitura digital|
|**Síntesis**|Creación matemática de sonidos|
|**Varianza**|Medida de cambios (0.01 = muy sensible)|
|**Inversión**|1023 - valor (para lógica intuitiva)|
|**Efectos**|EQ, Reverb, Delay (modifican sonido)|
