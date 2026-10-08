### 1. ¿Qué es el Arduino?
El Arduino actúa como el **traductor y mensajero** entre el mundo físico (la planta) y el mundo digital (tu computadora). Es el "cuerpo" del proyecto.
**Explicación Técnica**
Es un **microcontrolador** de hardware libre. Su función principal es leer señales eléctricas del entorno a través de sus **pines de entrada analógica** y enviar esa información en tiempo real a la computadora mediante un cable USB.

### 2. ¿Cómo recibe los datos de la planta?
Las plantas están vivas y llenas de agua y sales minerales, por lo que conducen electricidad de forma similar a nuestro cuerpo. Al conectar dos cables a la planta (uno de energía y otro de retorno), la planta actúa como un "regulador" de electricidad. Dependiendo de cómo se mueva el agua en sus células, la planta ofrece más o menos resistencia al paso de la electricidad.
**Explicación Técnica
  * Medimos la **impedancia (o resistencia eléctrica)** de la planta. 
  * Para medirla, usamos la resistencia interna del Arduino llamada **Pull-Up**. Esto crea un **divisor de tensión** (un circuito donde el voltaje se reparte entre la resistencia del Arduino y la de la planta).
  * El Arduino tiene un **Conversor Analógico-Digital (ADC)** de 10 bits. Este componente toma el voltaje físico que detecta en el pin `A1` (que va de 0 a 5 voltios) y lo convierte en un número entero digital entre **0 y 1023**.

### 3. ¿Qué datos recibe la computadora?
La computadora no recibe "música" ni "pensamientos" de la planta; solo recibe una ráfaga constante de números muy rápido.
**Explicación Técnica**
Recibe un flujo de **datos seriales (flujo de enteros de 0 a 1023)** a una tasa de muestreo (**sample rate**) de 200 Hz. Esto significa que el Arduino lee y envía 200 números por segundo a través del puerto USB (usando comunicación **UART/Serial** a una velocidad de **115200 baudios**).

### 4. ¿Qué es el programa en Python y cómo funciona?
El programa en Python es el "cerebro" y el "músico". Recibe esos números del Arduino, los limpia para que no tengan saltos bruscos por estática, detecta si la planta está realmente conectada y los convierte en hermosas notas musicales.
**Explicación Técnica**
El programa es una aplicación escrita en Python que realiza tres tareas en hilos de procesamiento paralelo (**multithreading**):
  1. **Procesamiento de Señal (DSP):** 
     * **Filtrado/Suavizado:** Usa una cola de datos (**deque**) para promediar los últimos valores y suavizar las curvas de la gráfica, eliminando el ruido electromagnético.
     * **Detección de conexión:** Analiza el promedio de los datos. Si está muy cerca de 1023 (sin conexión) o 0 (tierra), apaga el sonido. Si está en el rango medio, activa la música.
  2. **Mapeo a Notas Musicales (Escalado):**
     * Toma el número del sensor (de 0 a 1023) y mediante **interpolación matemática** lo traduce a una nota musical estándar (sistema **MIDI** de 36 a 96, que son las teclas de un piano).
  3. **Síntesis de Audio:**
     * Con la nota MIDI obtenida, calcula la **frecuencia de onda en Hertz (Hz)** y utiliza un sintetizador digital incorporado en Python (un **oscilador** que genera ondas senoidales, cuadradas, etc.) para crear el sonido físico que escuchas por los altavoces.