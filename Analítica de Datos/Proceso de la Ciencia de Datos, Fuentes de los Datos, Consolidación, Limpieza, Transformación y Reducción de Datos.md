# Componentes fundamentales que representan el núcleo del proceso de ciencia de datos

- Conector de Fuentes Heterogeneas
- Motor de Consolidación
- Módulo de Limpieza
- Transformador de Características
- Reductor de Dimensionalidad

# Validación de Cada componente mediante métricas relevantes

- Para Fuentes: Tasa de éxito en extracción y tiempo de respuesta
- Para Consolidación: Porcentaje de registros procesados sin pérdida
- Para limpieza: Reducción en errores detectados en validación posterior
- Para Transformación: Mejora en correlación con variable objetivo
- Para reducción, mantenimiento de varianza explicada > 95% con dimensionalidad reducida > 50%

# El Proceso de Ciencia de Datos se conecta con las siguientes **Disciplinas Fundamentales para Ingenieros**:

- Teoría de la Información: Explica por que la reducción debe preservar entroía crítica
- Teoría de Grafos: Fundamenta la consolidación de entidades cuando múltiples fuentes describen el mismo objetivo del mundo real
- Estadística Robusta: Proporciona herramientas para limpieza que no se ven distorcionadas por valores atípicos legítimos

# **Etapas del Proceso de Ciencia de Datos**
## El Origen del caos: Identificación y Extracción de Fuentes

La diversidad de fuentes es inevitable en contextos reales, y el éxito del pipeline depende de diseñar para la resiliencia ante esta diversidad. Un pipeline robusto no asume fuentes perfectas, incorpora salvaguardas en cada punto de extracción: reintentos con retroceso exponencial para APIs inestables, esquemas de fallback cuando el formato esperado cambia, y mecanismos de cuarentena para datos que no cumplen validaciones básicas son desbloquear todo el flujo.

La trampa más costosa en esta etapa es la ilusión de la fuente única de verdad, generando cuellos de botella y puntos únicos de fallo. La solución moderna es el **data mesh**, donde cada dominio de negocio (ventas, logística, marketing) mantiene sus propias fuentes como productos de datos autónomos, y el pipeline de ciencia de datos consume estas fuentes directamente mediante contratos explícitos de calidad y formato. Esta arquitectura no elimina la complejidad, la distribuye de forma manejable donde cada equipo res responsable de la calidad de sus propias fuentes, en lugar de un equipo central de ingeniería de datos sobrecargado.

**Clasificación de las Fuentes de Datos**

- Fuentes Estructuradas: Bases de Datos Relacionales (SQL), data warehouses con esquemas rígidos y predefinidos.

	- Ventaja→Consistencia garantizada por restricciones de integridad referencial
	- Desafío→Rigidez que dificulta adaptación a nuevos tipos de datos sin migraciones costosas 

- Fuentes Semiestructuradas: Documentos JSON/XML, logs con formato parcialmente definido, APIs REST

	- Ventaja→Flexibilidad para evolucionar sin esquemas rígidos
	- Desafío→Inconsistencia en estructura entre versiones o proveedores distintos

- Fuentes No Estructuradas: Texto libre (emails, anotaciones manuales), imágenes, audio, video

	- Ventaja→Riqueza de información contextual que las estructuras rígidas eliminan
	- Desafío→Necesidad de técnicas avanzadas (NLP, visión por computadora) para extraer señales útiles

- Fuentes en Streaming: Flujos continuos de datos (sensores IoT, clicks en tiempo real, transacciones financieras)

	- Ventaja→Capacidad para reaccionar a eventos en milisegundos
	- Desafío→Manejo de estado sin ventajas fijas y tolerancia a reordenamiento de eventos
## La integración imposible: Consolidación de Datos Heterogéneos

Es un proceso híbrido que combina reglas automáticas con intervención humana guiada.

La consolidación enfrente tres tipos de conflictos que requieren **estrategias** distintas

- **Conflictos de Esquema**: Mismos conceptos representados con tipos de datos incompatibles (ej: fecha como VARCHAR "2024-01-15" en una fuente vs. TIMESTAMP 1705276800 en otra).

	- Solución→Normalización a un tipo canónico mediante tranformaciones idempotentes (ej: convertir todo a ISO 8601)

- **Conflictos de Valor**: Mismos atributos con valores contradictorios para la misma entidad (ej: edad=35 en CRM vs. edad=42 en encuestas).

	- Solución→Mediante reglas de confianza (ej: dar prioridad a fuente actualizada más recientemente) o fusión probabilista (ej: calcular edad promedio ponderada por confianza de cada fuente)

- **Conflictos de Entidad**: Múltiples registros que describen la misma entidad del mundo real sin identificador común (ej: "Juan Pérez" en ventas vs. "J. Pérez" en CRM).

	- Solución→Record linkage mediante técnicas como fuzzy matching (comparación aproximada de strings) o grafos de similitud que conectan entidades basándose en atributos compartidos

## La purificación peligrosa: Limpieza de Datos Sin Destruir Señales

**La limpieza efectiva se estructura en tres fases interdependientes que evitan la trampa de la purificación ciega**

- **Detección con contexto**: Identificar potenciales problemas mediante técnicas estadísticas (IQR para atípicos, patrones regex para formatos inválidos) pero siempre en el contexto del dominio. Un valor de temperatura de 45°C es atípico en un clima templado pero normal en un desierto; la detección debe incorporar metadatos contextuales.

- **Diagnóstico causal**: antes de corregir, investigar la causa raíz del problema. Un valor faltante en "ingresos mensuales" podría ser:

	1. Error de Sistema (campo no guardado)
	2. Omisión deliberada por privacidad
	3. Cliente sin ingresos formales (trabajador informal)

	Cada causa requiere estrategia de tratamiento distinta

- **Tratamiento proporcional**: Aplicar la corrección mínima necesaria para preservar información. Para valores faltantes: imputación por media si es error aleatorio, marcador especial "desconocido" si es omisión deliberada, imputación por modo si es categoría faltante. Nunca eliminar registros sin evaluar el sesgo introducido.

## El enriquecimiento estratégico: transformación que revela patrones ocultos

Mientras la limpieza elimina ruido sin destruir señal, la transformación enriquece los datos para hacer explícitos patrones que están implícitos en las representaciones originales.

La transformación se categoriza en **cuatro tipos complementarios**

- **Derivación de Características**: Crear nuevas variables a partir de existentes mediante operaciones matemáticas o lógicas (ej: calcular "hora del día" a partir de timestamp, derivar "días desde última compra" a partir de fecha de última transacción)
- **Codificación Categórica**: Convertir variables categóricas en representaciones numéricas apropiadas para algoritmos (one-hot para categorías sin orden, label encoding para ordinales, target encoding para alta cardinalidad)
- **Escalado y Normalización**: Ajustar rangos de variables numéricas para que algoritmos sensibles a escala (SVM, k-NN) funcionen correctamente (standard scaling para distribuciones gaussianas, min-max para rangos acotados)
- **Agregación temporal/espacial**: Resumir datos a niveles superiores de granularidad para análisis de tendencias (ventas diarias ⇒ semanales, coordenadas GPS ⇒ zonas geográficas)

La trampa crítica que separa transformación efectiva de transformación destructiva es el data leakage - la filtración inadvertida de información del futuro o del conjunto de prueba al de entrenamiento. Un ejemplo clásico: calcular la media global de ingresos usando todo el dataset (train + test) y usarla para imputar valores faltantes en train. Esto introduce información del conjunto de prueba en train. Esto introduce información en producción. La solución es la transformación con aislamiento estricto: todo ajuste de parámetros (medias, escaladores, codificadores) debe calcularse exclusivamente con el conjunto de entrenamiento y aplicarse sin modificación al de prueba.

## La esencia sin el ruido: reducción de dimensionalidad inteligente

Tras la consolidación, limpieza y transformación, es común enfrentar conjuntos con cientos o miles de características donde muchas son redundantes o irrelevantes. La reducción de dimensionalidad elimina esta redundancia preservando la esencia informativa del conjunto, pero su aplicación requiere juicio crítico para evitar eliminar señales críticas disfrazadas de ruido.

La reducción se implementa mediante **dos enfoques complementarios**

- **Selección de Características**: Identificar y conservar solo las variables más informativas mediante métricas como correlación con variable objetivo, importancia según arboles de decisión, o pruebas estadísticas de significancia.

	- Ventaja: Interpretabilidad preservada (sabes qué variables originales influyen)
	- Desafío: Puede perder interacciones complejas entre variables que individualmente tienen baja correlación

- **Extracción de Características**: Crear nuevas variables que capturen la esencia de múltiples originales mediante técnicas como PCA (Principal Component Analysis) o autoencoders.

	- Ventaja: Captura interacciones complejas y reduce dimensionalidad drásticamente
	- Desafío: Pérdida de interpretabilidad (los componentes principales son combinaciones lineales abstractas sin significado de negocio)

La trampa más costosa es la **reducción ciega sin validación de impacto**. Aplicar PCA para reducir 100 variables a 10 componentes que explican el 95% de la varianza parece óptimo estadísticamente, pero si los componentes eliminados contenían señales críticas para eventos raros (fraudes, fallos catastróficos), el modelo perderá capacidad para detectar estos eventos. La solución es **reducción guiada por el objetivo del análisis:** si el objetivo es detección de fraudes (eventos raros), prioriza preservar dimensionalidad en regiones del espacio de características donde ocurren fraudes, aunque signifique mantener más dimensionalidad.

## El ciclo iterativo: por qué el proceso nunca es lineal

En contextos reales, el proceso es inherentemente iterativo y adaptativo, donde cada etapa informa y modifica las anteriores en un ciclo continuo de refinamiento.

Este carácter iterativo no es un defecto del proceso, es su fortaleza fundamental. Los datos del mundo real son demasiado complejos y cambiantes para ser procesados correctamente en un solo paso lineal. La iteración permite incorporar aprendizajes progresivos:

- En la primera iteración aplicas limpieza básica eliminando valores obviamente imposibles (-263°C en temperatura)
- En la segunda, investigas patrones de valores faltantes y descubres que ciertos sensores fallan sistemáticamente en condiciones de humedad >90%, permitiendo limpieza más inteligente
- En la tercera, incorporas datos meteorológicos externos para predecir y compensar estos fallos antes de que ocurran.

Cada iteración refina no solo los datos, sino también el entendimiento del dominio que guía decisiones de procesamiento.