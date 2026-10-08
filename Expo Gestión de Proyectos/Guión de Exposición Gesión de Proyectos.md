## ESTRUCTURA Y FLUJO DE LA PRESENTACIÓN

### DIAPOSITIVA 1: Portada / Introducción

**Qué decir:**

- Bienvenida
- Nombre del proyecto: "Gestionar Desarrollo de App de Geolocalización para el Seguimiento de Reportes a Problemas Urbanos"
- Equipo: ClearCode - Desarrollo & Soluciones Digitales
- Estudiantes: (Nombres)
- Profesor: Ing. Alma Delia Verónica López Jarquín
- Fecha y período

**Tiempo:** 30 segundos

---

### DIAPOSITIVA 2: Definición del Proyecto

**Qué decir:** "Este proyecto busca crear una plataforma digital completa que funcione como intermediaria entre los ciudadanos y las autoridades municipales.

Consta de tres componentes:

1. **Una App Móvil** para que los ciudadanos reporten problemas urbanos con foto y ubicación GPS
2. **Un Portal Web** para que las alcaldías gestionen esos reportes en tiempo real
3. **Una Infraestructura Cloud** que sostiene todo el sistema

El objetivo es combatir la desconfianza ciudadana: mientras el 98.2% de la población identifica problemas urbanos, solo el 29.9% confía en que el gobierno los resolverá. Esta app lo hace visible y trazable."

**Tiempo:** 1 minuto

---

### DIAPOSITIVA 3: Introducción - El Problema

**Qué decir:** "Permítanme mostrarles el contexto. Según la ENSU de diciembre 2025:

**Problemas Identificados:**

- 86.4% reporta baches en calles
- 63.9% falla en agua potable
- 60.8% alumbrado insuficiente
- 59.9% coladeras tapadas
- 63.8% se siente inseguro en la ciudad

**El Déficit Principal:** A pesar de que casi el 100% identifica problemas, **solo el 29.9% cree que el gobierno es efectivo resolviéndolos**.

Hay un GAP enorme entre identificación del problema y respuesta institucional. Los canales tradicionales (llamadas, formularios presenciales) son lentos, no tienen seguimiento, y generan desconfianza.

Aquí es donde entra nuestro proyecto: una plataforma que valida reportes, los geolocaliza, y proporciona seguimiento transparente."

**Tiempo:** 1.5 minutos

---

### DIAPOSITIVA 4: Objetivos del Proyecto

**Qué decir:** "Definimos 4 objetivos de gestión para los 12 meses de desarrollo:

**1. Alcance (MVP):** Entregar una App Móvil, Portal Web y Infraestructura Cloud con 6 categorías de reporte prioritarias: Baches, Agua, Iluminación, Coladeras, Basura e Infraestructura General.

**2. Tiempo:** Completar 6 fases en exactamente 12 meses sin retrasos:

- Mes 1: Análisis
- Mes 2: Diseño
- Meses 3-7: Desarrollo
- Meses 8-9: Pruebas
- Meses 10-11: Piloto con 3 alcaldías
- Mes 12: Cierre

**3. Costo:** Presupuesto de **$0 pesos en licencias**. Usamos solo Open Source y planes gratuitos de AWS, Firebase y Google Maps.

**4. Calidad:** Máximo 1% de bugs críticos, cumplimiento 100% de LGPDPPSO, y superación de prueba de estrés con 100,000 usuarios concurrentes."

**Tiempo:** 1.5 minutos

---

### DIAPOSITIVA 5: Enunciado del Alcance - Incluido/Excluido

**Qué decir:** "Para evitar que el proyecto se descontrole (scope creep), definimos claramente qué SÍ y qué NO está en el alcance.

**INCLUIDO:** ✓ App Móvil iOS y Android ✓ Portal Web para alcaldías ✓ Infraestructura Cloud completa ✓ Integración Google Maps + Firebase ✓ Pruebas exhaustivas ✓ Capacitación a 3 alcaldías piloto ✓ Documentación técnica

**EXCLUIDO:** ✗ Mantenimiento post-lanzamiento (eso es Año 1) ✗ Módulos de pago o monetización ✗ Reportes de delincuencia (eso es del Ministerio Público) ✗ Hardware o servidores físicos ✗ Expansión nacional (solo 3 alcaldías piloto) ✗ Gamificación o recompensas

Esta claridad en el alcance es fundamental para mantener el control del proyecto."

**Tiempo:** 1 minuto

---

### DIAPOSITIVA 6: Línea Base del Alcance

**Qué decir:** "La Línea Base del Alcance está compuesta por tres documentos:

1. **El Enunciado del Alcance:** Describe en detalle qué es lo que entregaremos y qué no.
    
2. **La EDT (Estructura de Desglose del Trabajo):** Es como un organigrama del proyecto. Lo dividimos en paquetes: Gestión, Análisis, Diseño, Desarrollo, Pruebas, Implementación y Cierre. Cada paquete contiene actividades específicas.
    
3. **El Diccionario de la EDT:** Define qué es cada paquete, quién es responsable, y cuáles son los entregables.
    

Esta línea base es sagrada: cualquier cambio debe pasar por un proceso formal de Solicitud de Cambio. El Director aprueba cambios menores; cambios mayores los aprueba el Comité de Control de Cambios."

**Tiempo:** 1 minuto

---

### DIAPOSITIVA 7: Línea Base del Cronograma

**Qué decir:** "El proyecto dura exactamente 12 meses. Esto es una restricción dura del proyecto.

Las 6 fases son secuenciales (cascada):

- **Mes 1:** Análisis y Requerimientos → Entrega: Especificación completa
- **Mes 2:** Diseño → Entrega: Diagramas, arquitectura, wireframes
- **Meses 3-7:** Desarrollo → Entrega: Código funcional, APIs, apps
- **Meses 8-9:** Pruebas → Entrega: Plan de Pruebas, Casos, Reportes. AQUÍ ocurre la prueba de estrés OBLIGATORIA de 100,000 usuarios
- **Meses 10-11:** Piloto → Entrega: Apps publicadas, capacitaciones, 1,000+ reportes validados
- **Mes 12:** Cierre → Entrega: Manuales, Acta de Aceptación, Cierre formal

El camino crítico (ruta crítica) significa que un retraso en cualquier fase hace que todo se retrase. No hay buffer. Por eso es importante monitoreo semanal."

**Tiempo:** 1.5 minutos

---

### DIAPOSITIVA 8: Línea Base del Costo

**Qué decir:** "La restricción de costo es peculiar: **$0 pesos en licencias de software.**

¿Cómo lo logramos?

1. **Desarrollo:** Solo herramientas Open Source
    
    - GitHub (Control de versiones)
    - VS Code, Android Studio, Xcode (IDEs gratuitos)
    - Jest, pytest (Testing frameworks gratuitos)
2. **Infraestructura Cloud:** Free Tiers
    
    - AWS Free Tier cubre bases de datos, almacenamiento, computo
    - Azure Free Tier alternativa
    - Google Maps Free Tier (geolocalización, geocoding)
    - Firebase Free Tier (notificaciones push)
3. **Consumo Estimado:** Durante los 12 meses de desarrollo, nuestro volumen (100-1,000 reportes/mes) se mantiene dentro de los límites free. Post-piloto, ya es problema de operación Año 1.
    

Esto es una inversión estratégica de ClearCode. Los costos de RRHH corren por cuenta de la organización."

**Tiempo:** 1 minuto

---

### DIAPOSITIVA 9: Interesados

**Qué decir:** "Un proyecto siempre tiene múltiples interesados con intereses diferentes. Los identificamos en dos grupos:

**INTERESADOS EXTERNOS:**

- **Ciudadanía:** Quieren una app intuitiva, rápida, con respuestas del gobierno
- **Alcaldías Piloto (3):** Necesitan reportes geolocalizados para gestionar recursos
- **Dependencias Municipales:** Requieren asignaciones de trabajo (Obras Públicas, CFE, etc.)
- **Organismos Reguladores:** Supervisan cumplimiento de LGPDPPSO
- **Personas con discapacidad:** Requieren accesibilidad en la app

**INTERESADOS INTERNOS:**

- **ClearCode:** Desarrollador, busca modelo SaaS post-lanzamiento
- **Director del Proyecto:** Gestión, aprobación de cambios
- **Equipo de Desarrollo:** 17 personas (arquitectos, backend, frontend, QA, DevOps)
- **Comité de Control de Cambios:** Aprueba cambios mayores

Mantener a estos interesados comunicados y satisfechos es clave para el éxito."

**Tiempo:** 1.5 minutos

---

### DIAPOSITIVA 10: Acuerdos

**Qué decir:** "Para que el proyecto funcione, establecimos 4 tipos de acuerdos formales:

**1. MOUs (Memorandos de Entendimiento) con Alcaldías:** Documentos no vinculantes financieramente que comprometen a las alcaldías a recibir reportes y asignar personal para actualizar estatus. Cada alcaldía firma uno.

**2. SLAs (Acuerdos de Nivel de Servicio) con AWS/Azure:** Garantizan disponibilidad del 99.9% (máximo 43 minutos de inactividad por mes) y tiempos de recuperación ante desastres. Esto es crítico para que los ciudadanos confíen.

**3. Cartas de Intención con CFE y Organismos de Agua:** Establecen que reportes de cables sueltos o fugas de agua lleguen DIRECTAMENTE a los despachadores, sin burocracia.

**4. Acuerdos de Confidencialidad y LGPDPPSO:** Cláusulas legales que obligan al sistema a proteger datos personales, implementar Derechos ARCO, y mantener bitácora de auditoría.

Sin estos acuerdos, el proyecto no avanza. Son nuestro marco de gobernanza legal."

**Tiempo:** 1.5 minutos

---

### DIAPOSITIVA 11: Ciclo de Vida del Proyecto

**Qué decir:** "Usamos ciclo de vida **Predictivo (Cascada)** porque el alcance, plazo y costo están definidos desde el inicio. Permite control estricto.

Veamos rápidamente qué ocurre en cada fase:

**FASE 1 (Mes 1) - Análisis:** Documentamos todos los requisitos, escribimos Historias de Usuario, Casos de Uso, todo compilado en la Especificación de Requisitos de Software (SRS). Firmamos MOUs con alcaldías. Salida: SRS aprobado.

**FASE 2 (Mes 2) - Diseño:** Arquitectos crean diagramas (Clases, Entidad-Relación, Secuencia, Componentes). Diseñadores crean Wireframes y Mockups. Documentamos decisiones técnicas. Salida: Documentación de diseño aprobada.

**FASE 3 (Meses 3-7) - Desarrollo:** Backend developers crean APIs, Frontend developers crean Apps móvil y portal web. DevOps configura infraestructura cloud. Integramos Google Maps y Firebase. Todo en código. Salida: Código funcional listo para pruebas.

**FASE 4 (Meses 8-9) - Pruebas:** QA realiza pruebas unitarias (80% cobertura mínima), integración, seguridad (OWASP). **OBLIGATORIAMENTE**: prueba de estrés con 100,000 usuarios concurrentes. Si falla, volvemos a desarrollo. Salida: Sistema aprobado técnicamente.

**FASE 5 (Meses 10-11) - Piloto:** Publicamos en App Store y Google Play. Cargamos datos geográficos de las 3 alcaldías. Capacitamos al personal municipal. Operamos piloto en vivo. Recolectamos feedback. Meta: Procesar 1,000+ reportes en 2 meses. Salida: Sistema operando en producción, validado.

**FASE 6 (Mes 12) - Cierre:** Entregamos manuales de usuario, de administrador, documentación técnica. Formalizamos Acta de Aceptación. Proyecto cerrado. Salida: Proyecto cerrado, listo para operación Año 1.

Este orden secuencial es importante: cada fase depende de la anterior. No se puede diseñar sin requisitos claros, no se puede desarrollar sin diseño aprobado, etc."

**Tiempo:** 3 minutos

---

### DIAPOSITIVA 12: Matriz de Trazabilidad de Requisitos

**Qué decir:** "La Matriz de Trazabilidad es un documento que vincula cada requisito desde su **origen** hasta su **implementación**, **prueba** y **validación**.

¿Por qué es importante?

1. **Asegura que nada se olvida:** Si definimos un requisito, debe tener su caso de prueba. Si no, algo falta.
    
2. **Justifica todo:** Cada requisito debe venir de una necesidad de negocio real (ENSU, LGPDPPSO, etc.). Si no tiene justificación, no debería estar ahí.
    
3. **Control de cambios:** Si alguien pide un cambio, podemos medir el impacto rastreando qué requisitos, pruebas y código se afectan.
    

**Ejemplo de estructura:**

- ID: RF-01 (Requisito Funcional 01)
- Origen: "Ciudadano necesita ver reportes en un mapa"
- Descripción: "Mostrar mapa interactivo con reportes geolocalizados"
- Prioridad: Must Have (MVP obligatorio)
- Implementación: "App Móvil - módulo Maps"
- Prueba: "Caso de Prueba 01"
- Estado: Implementado
- Línea Base: ✓

Tenemos ~50 requisitos así en la matriz. Cada uno trazable de principio a fin.

Esta matriz es 'viva': se actualiza cada mes conforme avanzamos el proyecto."

**Tiempo:** 1.5 minutos

---

### DIAPOSITIVA 13: EDT (Estructura de Desglose del Trabajo)

**Qué decir:** "La EDT es como un organigrama del trabajo. Descomponemos el proyecto en paquetes cada vez más pequeños hasta llegar a actividades concretas.

**Nivel 1: Proyecto Raíz** App de Geolocalización para Reportes Urbanos

**Nivel 2: 8 Paquetes Principales**

1. Gestión del Proyecto
2. Análisis y Requerimientos (Mes 1)
3. Diseño (Mes 2)
4. Desarrollo (Meses 3-7)
5. Pruebas (Meses 8-9)
6. Implementación y Piloto (Meses 10-11)
7. Cierre (Mes 12)
8. Control y Monitoreo (Transversal)

**Nivel 3: Subpaquetes y Actividades** Por ejemplo, dentro de 'Desarrollo':

- Desarrollo Backend (APIs, BD)
- Desarrollo App iOS
- Desarrollo App Android
- Desarrollo Portal Web
- Integración de Servicios

Cada paquete tiene un responsable, un cronograma, un presupuesto, y entregables específicos.

Veremos que el cronograma detallado en la siguiente diapositiva se alinea con esta EDT."

**Tiempo:** 1 minuto

---

### DIAPOSITIVA 14: Cronograma de Actividades

**Qué decir:** "El cronograma detalla CUÁNDO ocurre cada actividad, QUIÉN es responsable, y CUÁLES son las dependencias.

**Vista rápida (simplificada):**

- **Semana 1-4 (Mes 1):**
    
    - Constitución del proyecto
    - Recolección de requisitos (2 sem)
    - Documentación SRS (1 sem)
    - Hito: SRS aprobado
- **Semana 5-8 (Mes 2):**
    
    - Diseño Arquitectura (1 sem)
    - Diseño BD y Clases (1 sem)
    - Wireframes y Mockups (1 sem)
    - Especificación APIs (1 sem)
    - Hito: Diseño aprobado
- **Semana 9-28 (Meses 3-7):**
    
    - Desarrollo Backend (paralelo)
    - Desarrollo iOS (paralelo)
    - Desarrollo Android (paralelo)
    - Desarrollo Portal (paralelo)
    - Integraciones de servicios
    - Code review continuo
- **Semana 29-36 (Meses 8-9):**
    
    - Pruebas Unitarias (4 semanas, 80% cobertura)
    - Pruebas de Integración (2 semanas)
    - Pruebas de Seguridad (2 semanas)
    - Prueba de Estrés 100,000 usuarios (OBLIGATORIA)
    - Hito: Sistema aprobado técnicamente
- **Semana 37-44 (Meses 10-11):**
    
    - Publicación App Store y Google Play
    - Carga de datos geográficos
    - Capacitación 3 alcaldías (3 semanas)
    - Operación piloto (8 semanas)
    - Hito: Validación piloto exitosa
- **Semana 45-52 (Mes 12):**
    
    - Documentación final
    - Manual de usuario, administrador, técnico
    - Validación LGPDPPSO
    - Hito: Acta de Cierre

**Recursos por fase:**

- Meses 1-2: ~5 personas (analistas, diseñadores)
- Meses 3-7: ~12 personas (desarrolladores, arquitectos)
- Meses 8-9: ~8 personas (QA, testers, seguridad)
- Meses 10-11: ~6 personas (operaciones, capacitadores)
- Mes 12: ~3 personas (cierre, documentación)

Sin retrasos. Ruta crítica estricta."

**Tiempo:** 2 minutos

---

### DIAPOSITIVA 15: Hoja de Recursos

**Qué decir:** "Para ejecutar el proyecto, necesitamos un equipo de 17 personas distribuidas así:

**Gestión y Análisis:**

- 1 Director de Proyecto (100% meses 1, 2, 10-12; 50% resto)
- 2 Analistas/Business Analysts (100% mes 1; luego decrece)

**Arquitectura y Infraestructura:**

- 1 Arquitecto del Sistema (50% mes 1; 100% mes 2; 50% resto)
- 1 DevOps/Infrastructure (50% mes 2; 100% meses 3-7, 10-11)

**Desarrollo:**

- 3 Backend Developers (100% meses 3-7; 100% meses 8-9)
- 1 iOS Developer (100% meses 3-7)
- 1 Android Developer (100% meses 3-7)
- 1 Frontend Developer (80% meses 3-6; 100% meses 7-9)

**Diseño:**

- 1 UX/UI Designer (50% mes 1; 100% mes 2; 30% meses 3-7)

**Calidad:**

- 1 QA Lead (20% meses 3-7; 100% meses 8-9)
- 2 QA Testers (10% meses 3-7; 100% meses 8-9)
- 1 Security Tester (100% meses 8-9)

**Documentación:**

- 1 Technical Writer (10% meses 3-7; 50% meses 10-11; 100% mes 12)

**Total:** 17 personas, con picos de carga en meses 3-7 y 8-9.

**Costo:** No presupuestado (inversión interna ClearCode). Licencias: $0 pesos."

**Tiempo:** 1.5 minutos

---

### DIAPOSITIVA 16: Costos de las Actividades

**Qué decir:** "El proyecto tiene un presupuesto oficial de **$0 pesos en licencias.**

**Desglose de costos:**

1. **Software:** $0
    
    - Desarrollo: Open Source (GitHub, VS Code, Android Studio, Xcode, Jest, pytest)
    - Servicios cloud: Free Tiers (AWS, Azure, Firebase, Google Maps)
    - Herramientas: Open Source
2. **Infraestructura:** $0
    
    - Cloud-native 100% (no hay servidores físicos propios)
    - AWS Free Tier / Azure Free Tier cubre almacenamiento, BD, cómputo
    - Durante 12 meses de desarrollo, consumo es bajo
3. **Recursos Humanos:** No presupuestado
    
    - 17 personas × 65-70 persona-mes = ~$130-140k USD equivalente
    - PERO es inversión interna ClearCode, no presupuesto del proyecto
4. **Otros:** Bajo
    
    - Capacitación alcaldías: Realizado por equipo ClearCode
    - Documentación: Digital (PDF)
    - Viajes: Bajo (depende ubicación alcaldías)

**Post-piloto (Año 1 operación):** Aquí SÍ habría costos de infraestructura cloud si el volumen crece, pero eso está fuera del scope de este proyecto."

**Tiempo:** 1 minuto

---

### DIAPOSITIVA 17: Presupuesto

**Qué decir:** "La Línea Base del Costo es **$0 en licencias.**

**Distribución por fase (conceptual):**

- Mes 1 (Análisis): $0 licencias
- Mes 2 (Diseño): $0 licencias
- Meses 3-7 (Desarrollo): $0 licencias
- Meses 8-9 (Pruebas): $0 licencias
- Meses 10-11 (Piloto): $0 licencias
- Mes 12 (Cierre): $0 licencias

**Total oficial: $0 pesos**

**Supuestos:**

1. Free Tiers de AWS, Azure, Google y Firebase cubren nuestro volumen durante 12 meses
2. Equipo de ClearCode asume costos de RRHH como inversión estratégica
3. Infraestructura cloud se contrata post-piloto bajo modelo SaaS

Este presupuesto es una restricción importante: obliga a ser muy eficiente en tecnología."

**Tiempo:** 1 minuto

---

### DIAPOSITIVA 18: Ejemplo de Valor Ganado (EVM) - Contexto

**Qué decir:** "La Gestión del Valor Ganado (EVM) es una técnica que mide el **desempeño del proyecto** combinando **alcance**, **tiempo** y **costo** en un solo indicador.

**Conceptos clave:**

- **BAC (Budget at Completion):** Presupuesto total del proyecto = 100 unidades
- **PV (Planned Value):** Valor planificado a una fecha específica = trabajo que DEBERÍA estar listo
- **EV (Earned Value):** Valor ganado = trabajo que REALMENTE está listo
- **AC (Actual Cost):** Costo real que hemos gastado

**Variaciones:**

- **CV (Cost Variance) = EV - AC**
    - CV > 0: Gastamos menos (favorable)
    - CV < 0: Gastamos más (desfavorable)
- **SV (Schedule Variance) = EV - PV**
    - SV > 0: Adelantados (favorable)
    - SV < 0: Atrasados (desfavorable)

**Índices de Desempeño:**

- **CPI (Cost Performance Index) = EV / AC**
    - CPI > 1: Eficiente
    - CPI < 1: Ineficiente
- **SPI (Schedule Performance Index) = EV / PV**
    - SPI > 1: Adelantado
    - SPI < 1: Atrasado
- **CSI (Combined Schedule Index) = CPI × SPI**
    - CSI > 0.9: Proyecto en buen estado
    - CSI 0.8-0.9: Requiere atención
    - CSI < 0.8: Crítico

El EVM se calcula cada mes para monitorear desviaciones temprano."

**Tiempo:** 2 minutos

---

### DIAPOSITIVA 19: Ejemplo de Valor Ganado - Escenario Mes 6

**Qué decir:** "Imaginemos que estamos al final del Mes 6 (mitad del proyecto).

**Distribución de valor planificada:**

- Meses 1-2 (Análisis + Diseño): 20 unidades
- Meses 3-6 (Desarrollo ½): 32 unidades (de 50 totales)
- Meses 7-9 (Desarrollo ½ + Pruebas): 30 unidades
- Meses 10-11 (Piloto): 14 unidades
- Mes 12 (Cierre): 4 unidades
- **Total BAC: 100 unidades**

**Lo que DEBERÍA estar listo al Mes 6 (PV):**

- Análisis: completado = 10 unidades
- Diseño: completado = 10 unidades
- Desarrollo parcial (4 de 5 meses): 32 unidades
- **Total PV: 52 unidades**

**Lo que REALMENTE está listo (EV):**

- Análisis: completado = 10 unidades
- Diseño: completado = 10 unidades
- Desarrollo parcial: SOLO 28 unidades (atrasado)
- **Total EV: 48 unidades**

**Lo que REALMENTE gastamos (AC):**

- Consumo de infraestructura: más alto de lo esperado
- Equipo requirió horas extra para resolver problemas técnicos
- **Total AC: 50 unidades**

**Cálculos:**"

**Tiempo:** 1.5 minutos

---

### DIAPOSITIVA 20: Ejemplo de Valor Ganado - Cálculos

**Qué decir:** "Con los datos anteriores, calculamos:

**Variación de Costo (CV):** CV = EV - AC = 48 - 50 = **-2 unidades** → Interpretación: Gastamos 2 unidades MÁS de lo planificado. **DESFAVORABLE.**

**Variación de Cronograma (SV):** SV = EV - PV = 48 - 52 = **-4 unidades** → Interpretación: Completamos 4 unidades MENOS de lo planificado. Estamos **ATRASADOS** en cronograma. **DESFAVORABLE.**

**Índice de Desempeño de Costo (CPI):** CPI = EV / AC = 48 / 50 = **0.96** → Interpretación: Por cada peso gastado, solo generamos 0.96 pesos de valor. Ineficiencia del 4% en costo.

**Índice de Desempeño de Cronograma (SPI):** SPI = EV / PV = 48 / 52 = **0.923** → Interpretación: Solo completamos el 92.3% del trabajo planificado. Hemos perdido ~8% de velocidad.

**Índice Combinado (CSI):** CSI = CPI × SPI = 0.96 × 0.923 = **0.886** → Interpretación: **CSI = 0.886 está en rango 0.8-0.9.** → El proyecto **REQUIERE ATENCIÓN INMEDIATA**, pero no es crítico aún."

**Tiempo:** 1.5 minutos

---

### DIAPOSITIVA 21: Ejemplo de Valor Ganado - Diagnóstico

**Qué decir:** "¿Qué está pasando?

**Resumen de problemas:**

1. Estamos 4 unidades atrasados en cronograma (8% de retraso)
2. Gastamos 2 unidades de más (sobregasto del 4%)
3. CSI = 0.886 → requiere intervención

**Causas probables:**

- Problemas técnicos integrando Google Maps API o Firebase
- Cambios no previstos en requisitos de alcaldías
- Equipo de desarrollo subestimó complejidad de módulo de notificaciones
- Pruebas de integración más largas de lo esperado

**¿A dónde vamos si no intervenimos?** Si continúa esta tendencia:

- Ritmo actual: 48 unidades en 6 meses = 8 unidades/mes
- Trabajo restante: 100 - 48 = 52 unidades
- Tiempo requerido: 52 / 8 = 6.5 meses
- **Terminaríamos a mitad de mes 12.5 (FUERA DE PLAZO)**
- **Costo final estimado: 104.17 unidades (sobrepresupuesto)**

**¿Qué hacemos?**"

**Tiempo:** 1 minuto

---

### DIAPOSITIVA 22: Ejemplo de Valor Ganado - Acciones Correctivas

**Qué decir:** "El Director del Proyecto debe intervenir INMEDIATAMENTE con acciones correctivas:

**1. Acelerar Desarrollo (para recuperar 4 unidades de cronograma):**

- Reasignar +1 backend developer de otro proyecto
- Reducir scope temporal: pausar feature de "mapa de calor" (menor prioridad)
- Aumentar horas del equipo (cuidando burnout)
- Objetivo: Recuperar 1 unidad/semana en próximas 4 semanas

**2. Analizar Sobregasto (para recuperar 2 unidades de costo):**

- Auditar consumo de infraestructura cloud ¿salimos del free tier?
- Revisar horas extras de equipo ¿están documentadas?
- Buscar optimizaciones en código (reduce latencia = menos instancias cloud)

**3. Replanificación:**

- Reunión con Comité de Control de Cambios
- Evaluar si es posible recuperar atraso en Meses 7-9
- Ajustar duración de pruebas si es necesario
- Establecer hito de 'vuelta a línea base' en Mes 7

**4. Comunicación y Monitoreo:**

- Reportar situación a Director General y stakeholders
- Establecer monitoreo SEMANAL de CV y SV (no esperar mes completo)
- Presentar plan de recuperación detallado
- Seguimiento diario de métricas críticas

**Si no actúa rápido, el proyecto termina fuera de plazo y presupuesto. EVM sirve para detectar esto a tiempo.**"

**Tiempo:** 1.5 minutos

---

### DIAPOSITIVA 23: Ejemplo de Valor Ganado - Tabla Resumen

**Qué decir:** "Aquí está el resumen en una tabla:

|Métrica|Valor|Interpretación|
|---|---|---|
|**BAC**|100|Presupuesto total autorizado|
|**PV (Planificado)**|52|Trabajo que debería estar listo|
|**EV (Realizado)**|48|Trabajo realmente completado|
|**AC (Gastado)**|50|Costo real incurrido|
|**CV**|-2|Sobregasto de 2 unidades|
|**SV**|-4|Atraso de 4 unidades|
|**CPI**|0.96|Ineficiencia en costo|
|**SPI**|0.923|Solo 92.3% de cronograma|
|**CSI**|0.886|**Estado: REQUIERE ATENCIÓN**|
|**EAC (Proyección)**|104.17|Costo final estimado (si no cambia)|
|**VAC (Proyección)**|-4.17|Sobrepresupuesto estimado|

Esta tabla se actualiza CADA MES durante el proyecto para monitoreo continuo."

**Tiempo:** 1 minuto

---

### DIAPOSITIVA 24: Conclusiones Personales

**Qué decir:** "Reflexionando sobre este proyecto y lo aprendido en la clase:

**1. Importancia de la Gestión Estructurada:** Este proyecto demostró cómo PMBOK proporciona un marco riguroso. Sin líneas base claras, sin EDT, sin Valor Ganado, estaríamos trabajando a ciegas. La estructura es lo que permite detectar problemas TEMPRANO, no a final de proyecto.

**2. Relevancia Social:** Un proyecto no es solo números. Esto tiene impacto real: el 98.2% de los ciudadanos identifica problemas urbanos pero solo el 29.9% confía en que el gobierno los resuelva. Esta app **cierra esa brecha de confianza**. Es gobernanza digital en acción.

**3. Restricciones Productivas:** Paradójicamente, restricciones como presupuesto $0 y plazo de 12 meses FUERZAN innovación. No hay dinero para licencias caras → descubrimos open source. Plazo estricto → priorización rigurosa del MVP.

**4. Gestión de Riesgos:** Un proyecto de 12 meses sin retrasos permitidos es de alto riesgo. Por eso:

- Monitoreo semanal de progreso
- Método Cascada permite control estricto
- EVM detecta desviaciones temprano
- Plan de contingencia documentado

**5. Desafíos Observados:**

- **Integración de APIs:** Google Maps + Firebase + custom backend, todo en paralelo
- **Cumplimiento legal:** LGPDPPSO mientras desarrollamos (no después)
- **Adopción ciudadana:** lograr 1,000 reportes en piloto requiere confianza ciudadana
- **Escalabilidad:** 100,000 usuarios concurrentes es un reto con presupuesto $0

**6. Fortaleza del Proyecto:**

- MVP bien definido (no es feature creep)
- 3 líneas base claras
- Documentación exhaustiva
- Gobernanza clara (roles, responsabilidades, aprobaciones)
- Énfasis en calidad (prueba de estrés obligatoria)

**7. Recomendaciones para Ejecución:**

- Implementar monitoreo de Valor Ganado MENSUALMENTE (como mostré)
- Mantener buffers de tiempo en actividades críticas
- Comunicación SEMANAL con alcaldías (no solo al cierre)
- Plan de mitigación de riesgos vivo (actualizado cada mes)
- Decisiones rápidas en Comité de Cambios (1-2 días máximo)

**8. Aprendizaje Personal:** PMBOK no es 'burocracia por burocracia'. Cada documento, cada proceso, existe porque resuelve un problema real. La Matriz de Trazabilidad, el EVM, la EDT: todas son herramientas que permitieron identificar temprano (en mes 6) que el proyecto estaba desviándose. Sin ellas, seguiríamos desarrollando sin saber que estábamos en problemas.

Este proyecto me mostró que **la gestión disciplinada es lo que transforma visiones en realidad.** No es glamoroso, pero es absolutamente necesario."

**Tiempo:** 3 minutos

---

## RESUMEN DE TIEMPOS

|Sección|Tiempo|
|---|---|
|Portada|0:30|
|Definición|1:00|
|Introducción|1:30|
|Objetivos|1:30|
|Enunciado Alcance|1:00|
|Línea Base Alcance|1:00|
|Línea Base Cronograma|1:30|
|Línea Base Costo|1:00|
|Interesados|1:30|
|Acuerdos|1:30|
|Ciclo de Vida|3:00|
|Matriz Trazabilidad|1:30|
|EDT|1:00|
|Cronograma|2:00|
|Hoja Recursos|1:30|
|Costos Actividades|1:00|
|Presupuesto|1:00|
|EVM Contexto|2:00|
|EVM Escenario|1:30|
|EVM Cálculos|1:30|
|EVM Diagnóstico|1:00|
|EVM Acciones|1:30|
|EVM Tabla|1:00|
|Conclusiones|3:00|
|**TOTAL**|**~38 minutos**|

_(Aproximadamente 38 minutos sin preguntas. Deja 5-7 minutos para preguntas del profesor/compañeros)_

---

## NOTAS IMPORTANTES PARA LA PRESENTACIÓN

1. **Empieza en tiempo:** Los profesores valoran la puntualidad
2. **Habla con confianza:** Tú conoces este proyecto mejor que nadie
3. **Haz contacto visual:** No leas directamente de las diapositivas
4. **Usa ejemplos reales:** "El 98.2% de la población..." es más impactante que números genéricos
5. **Anticipa preguntas comunes:**
    - "¿Por qué cascada y no ágil?" → Porque alcance, plazo y costo están fijos desde inicio
    - "¿Cómo logran $0 en licencias?" → Open Source + Free Tiers
    - "¿Qué pasa si sale del Free Tier?" → Parte del Año 1 de operación, fuera del MVP
6. **Maneja el nerviosismo:** Respira, pausa entre ideas, toma agua
7. **Cierra fuerte:** Las conclusiones personales son lo que te diferencia. Haz que cuente.

---

¡Mucho éxito en tu presentación! 