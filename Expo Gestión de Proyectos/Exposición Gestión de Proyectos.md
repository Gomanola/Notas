# INFORMACIÓN PARA LA PRESENTACIÓN DEL PROYECTO

## App de Geolocalización para Reportes Urbanos

---

## 1. NOMBRE DEL PROYECTO

**Gestionar Desarrollo de App de Geolocalización para el seguimiento de reportes a problemas urbanos**

---

## 2. DEFINICIÓN DEL PROYECTO

La gestión del proyecto consiste en planificar, diseñar, desarrollar, probar e implementar una plataforma digital completa (App Móvil iOS/Android + Portal Web Administrativo + Infraestructura Cloud) que permita a los ciudadanos reportar problemas urbanos mediante geolocalización, fotografías y descripciones, y a las autoridades municipales gestionar estos reportes de forma eficiente, transparente y trazable.

**Empresa responsable:** ClearCode - Desarrollo & Soluciones Digitales

---

## 3. INTRODUCCIÓN

(Información para la diapositiva)

### Contexto del Problema

- Según la ENSU (Encuesta Nacional de Seguridad Pública Urbana) de diciembre 2025:
    - **98.2%** de la población identifica problemáticas en su ciudad (baches, agua, iluminación, etc.)
    - **Solo 29.9%** confía en la efectividad del gobierno para resolver estos problemas
    - Existe una brecha crítica entre la detección de problemas y la capacidad de respuesta

### Problemas Identificados

- Baches en calles: 86.4%
- Fallas en agua: 63.9%
- Alumbrado insuficiente: 60.8%
- Coladeras tapadas: 59.9%
- Inseguridad ciudadana: 63.8%

### Solución Propuesta

Plataforma intermediaria independiente que:

- Valida reportes ciudadanos
- Geolocaliza problemas con precisión
- Proporciona seguimiento trazable
- Combate desconfianza institucional (29.9% efectividad)

---

## 4. OBJETIVOS DEL PROYECTO

### Objetivos de Gestión (Proyecto - 12 meses)

**Objetivo de Alcance (MVP):**

- Finalizar desarrollo de Producto Mínimo Viable incluyendo:
    - App móvil (iOS y Android)
    - Portal Web de consulta
    - Dashboard administrativo
    - 6 categorías de reporte prioritarias: Baches, Agua, Luz, Coladeras, Basura, Infraestructura General

**Objetivo de Tiempo:**

- Completar 6 fases en período estricto de 12 meses:
    1. Análisis y Levantamiento de Requerimientos (Mes 1)
    2. Diseño de la Solución (Mes 2)
    3. Desarrollo (Meses 3-7)
    4. Pruebas e Integración (Meses 8-9)
    5. Implementación y Piloto (Meses 10-11)
    6. Cierre y Entrega (Mes 12)

**Objetivo de Costo:**

- Presupuesto operativo: **$0 pesos en licencias**
- Estrategia: Open Source + Free Tiers de AWS/Firebase/Google Maps

**Objetivo de Calidad y Seguridad:**

- Índice de bugs críticos: menor a 1%
- Cumplimiento 100% LGPDPPSO (protección de datos)

### Objetivos del Producto (Post-lanzamiento)

**Objetivo de Adopción:**

- Procesar mínimo 1,000 reportes validados en primeros 3 meses de operación

**Objetivo de Precisión:**

- Reportes con coordenadas GPS exactas (máximo 10 metros de error)

**Objetivo de Vinculación:**

- Establecer canal técnico con al menos 3 dependencias gubernamentales

**Objetivo de Escalabilidad:**

- Soportar 100,000 usuarios concurrentes
- Transitar a modelo SaaS a partir del año 1

---

## 5. ENUNCIADO DEL ALCANCE DEL PROYECTO

### Línea Base del Alcance

**Incluido en el alcance:**

- Análisis y definición de requisitos
- Diseño técnico completo (diagramas, arquitectura)
- Desarrollo de App Móvil (iOS/Android)
- Desarrollo de Portal Web Administrativo
- Infraestructura Cloud 100% (AWS o Azure)
- 6 categorías de reporte del MVP
- Integración de APIs: Google Maps, Firebase Cloud Messaging
- Pruebas unitarias (80% cobertura mínima)
- Pruebas de estrés (100,000 usuarios concurrentes)
- Capacitación a 3 ayuntamientos piloto
- Documentación completa (técnica, usuario, administrador)

**Excluido del alcance:**

- Mantenimiento post-lanzamiento
- Módulos de pago/suscripción
- Integración con sistemas legados municipales
- Reportes de seguridad pública/delincuencia
- Hardware e infraestructura física
- PWA o versión web escritorio
- Gamificación o recompensas
- Expansión nacional
- Soporte multi-idioma

### Línea Base del Cronograma (Tiempo)

**Duración total:** 12 meses calendario **Fases:** 6 fases secuenciales (predictivo/cascada) **Ruta crítica:** Sin retrasos permitidos

|Fase|Duración|Actividades|
|---|---|---|
|Análisis y Requerimientos|Mes 1|Documentación de requisitos, Historias de Usuario, Casos de Uso, SRS|
|Diseño|Mes 2|Diagramas de clases, ER, flujos, wireframes, prototipos|
|Desarrollo|Meses 3-7|Codificación backend, frontend móvil y web|
|Pruebas|Meses 8-9|Unitarias, integración, seguridad, estrés|
|Piloto|Meses 10-11|Despliegue en 3 alcaldías, capacitación, validación|
|Cierre|Mes 12|Aceptación formal, entrega documentación|

### Línea Base del Costo

**Presupuesto total:** $0 pesos en licencias de software

**Estrategia de costos:**

- Herramientas Open Source (gratuitas)
- Free Tier de AWS/Azure
- Free Tier de Google Maps Platform (dentro de límites)
- Free Tier de Firebase Cloud Messaging

**Recursos necesarios (costos NO incluidos en la línea base pero relevantes para ejecución):**

- Equipo de desarrollo ClearCode
- Infraestructura cloud (cubierta con Free Tiers)
- Servicios externos (mapas, notificaciones)

---

## 6. INTERESADOS

### Interesados Externos

|Tipo|Descripción|
|---|---|
|**Ciudadanía**|Usuarios finales que reportan problemas urbanos; esperan app intuitiva con retroalimentación rápida|
|**Ayuntamientos/Alcaldías Piloto (3)**|Receptores de reportes; requieren portal eficiente y datos en tiempo real para gestionar recursos|
|**Dependencias Municipales**|Obras Públicas, CFE, SACMEX; realizan reparaciones; reciben asignaciones de tareas|
|**Organismos Reguladores**|Supervisores de protección de datos (LGPDPPSO)|
|**Población Vulnerable**|Personas con discapacidad; requieren accesibilidad según WCAG|

### Interesados Internos

|Tipo|Rol/Responsabilidad|
|---|---|
|**ClearCode (Organización)**|Desarrollador; gestor del proyecto; responsable del MVP; buscará modelo SaaS post-lanzamiento|
|**Director del Proyecto**|Gestión general, aprobación de cambios menores, coordinación|
|**Equipo de Desarrollo**|Arquitectos, desarrolladores backend/frontend, QA, DevOps|
|**Equipo de Diseño UX/UI**|Interfaz intuitiva, accesibilidad|
|**Equipo de Calidad**|Pruebas (unitarias, integración, seguridad, estrés)|
|**Comité de Control de Cambios**|Evalúa y aprueba cambios mayores que afecten línea base|

---

## 7. ACUERDOS

### Alianzas Estratégicas Documentadas

**1. Memorandos de Entendimiento (MOUs) con Alcaldías**

- Tipo: Documento no vinculante financieramente
- Propósito: Compromiso municipal para recibir reportes y asignar personal operativo
- Entregable: Documento firmado por cada alcaldía piloto

**2. Acuerdos de Nivel de Servicio (SLA) con Proveedores Cloud**

- Proveedor: AWS o Azure
- Disponibilidad garantizada: 99.9% mensual (máximo 43 minutos inactividad/mes)
- DRP (Disaster Recovery Plan): Tiempos de recuperación ante desastres
- Propósito: Garantizar funcionamiento del sistema

**3. Cartas de Intención con Organismos Autónomos**

- Destinatarios: CFE, organismos de agua
- Propósito: Protocolos técnicos para que reportes de infraestructura lleguen directamente a despachadores
- Ejemplo: Reportes de cables sueltos → CFE sin intermediarios

**4. Acuerdos de Confidencialidad y Protección de Datos**

- Regulación: LGPDPPSO (Ley General de Protección de Datos Personales)
- Cláusulas en términos y condiciones
- Garantías: Datos personales protegidos, uso solo para fines de servicio público
- Derechos ARCO: Acceso, Rectificación, Cancelación, Oposición

---

## 8. CICLO DE VIDA DEL PROYECTO

### Tipo: Predictivo (Cascada)

**Justificación:** Alcance, plazos y presupuesto definidos desde inicio. Control estricto sobre cambios.

### Las 6 Fases:

**FASE 1: ANÁLISIS Y LEVANTAMIENTO DE REQUERIMIENTOS (Mes 1)**

- Entrada: Problema definido por ENSU 2025, necesidad municipal
- Actividades:
    - Documentar requisitos funcionales y no funcionales
    - Escribir Historias de Usuario (ciudadano, operador, admin)
    - Definir Casos de Uso con diagramas
    - Crear Especificación de Requisitos de Software (SRS)
    - Matriz de Trazabilidad de Requisitos (inicial)
    - Formalizar acuerdos con alcaldías (MOUs)
    - Protocolo LGPDPPSO
- Salida: SRS firmado, Requisitos priorizados (MoSCoW)

**FASE 2: DISEÑO DE LA SOLUCIÓN (Mes 2)**

- Entrada: SRS aprobado
- Actividades:
    - Diagrama de Clases (estructura del software)
    - Diagrama Entidad-Relación (base de datos)
    - Diagramas de Secuencia (interacciones sistema)
    - Documento de Arquitectura del Sistema
    - Diagrama de Componentes y Despliegue (cloud)
    - Wireframes y Mockups de interfaz
    - Prototipos interactivos (validar con alcaldías)
    - Especificación de APIs (Swagger/OpenAPI)
- Salida: Documentación de diseño aprobada

**FASE 3: DESARROLLO (Meses 3-7)**

- Entrada: Diseño aprobado
- Actividades:
    - Codificación backend (APIs REST)
    - Desarrollo App Móvil iOS (Swift/Objective-C)
    - Desarrollo App Móvil Android (Kotlin/Java)
    - Desarrollo Portal Web Administrativo (React/Vue)
    - Integración Google Maps Platform
    - Integración Firebase Cloud Messaging
    - Configuración infraestructura AWS/Azure
    - Base de datos escalable
    - Almacenamiento de imágenes (S3/Blob Storage)
    - Control de versiones Git
    - Estándares de codificación
- Salida: Código funcional, repositorios organizados

**FASE 4: PRUEBAS E INTEGRACIÓN (Meses 8-9)**

- Entrada: Código desarrollado
- Actividades:
    - Plan de Pruebas (documento formal)
    - Pruebas Unitarias (80% cobertura backend mínimo, herramientas Jest/pytest)
    - Pruebas de Integración (componentes del sistema)
    - Pruebas de Seguridad (OWASP Mobile Top 10, vulnerabilidades críticas)
    - Prueba de Estrés (100,000 usuarios concurrentes simulados - OBLIGATORIA)
    - Pruebas de Aceptación (validación funcional)
    - Casos de Prueba documentados
    - Reportes de Resultados por tipo
    - Corrección de bugs
- Salida: Sistema aprobado técnicamente, bugs críticos < 1%

**FASE 5: IMPLEMENTACIÓN Y PILOTO (Meses 10-11)**

- Entrada: Sistema validado
- Actividades:
    - Publicar en App Store (iOS)
    - Publicar en Google Play Store (Android)
    - Carga inicial datos geográficos (colonias, códigos postales, polígonos)
    - Capacitación a personal municipal (3 alcaldías)
    - Acta de Capacitación firmada por cada dependencia
    - Operación piloto en 3 alcaldías
    - Monitoreo de estabilidad
    - Recolección de retroalimentación
    - Ajustes menores según feedback
    - Validación de 1,000+ reportes procesados
- Salida: Sistema operando en producción, retroalimentación documen tada

**FASE 6: CIERRE Y ENTREGA (Mes 12)**

- Entrada: Piloto exitoso
- Actividades:
    - Entrega Manual de Usuario (App)
    - Entrega Manual de Administrador (Portal)
    - Documentación técnica completa
    - Documentación LGPDPPSO (Aviso de Privacidad, módulo ARCO)
    - Manual de Despliegue (para futuro mantenimiento)
    - Acta de Aceptación del Proyecto (firmada por interesados)
    - Lecciones Aprendidas
    - Transición a modelo operativo
- Salida: Acta de Cierre firmada, proyecto finalizado

### Documentos Generados por Fase (Entregables)

|Fase|Entregables Principales|
|---|---|
|1|SRS, Historias de Usuario, Casos de Uso, Matriz Trazabilidad, MOUs|
|2|Arquitectura, Diagramas, Wireframes, Prototipos|
|3|Código fuente, APIs documentadas, Infraestructura cloud|
|4|Plan de Pruebas, Casos de Prueba, Reportes de Resultados|
|5|Apps publicadas, Capacitaciones realizadas, Datos cargados|
|6|Manuales, Documentación técnica, Acta de Cierre|

---

## 9. MATRIZ DE TRAZABILIDAD DE REQUISITOS

### Concepto

Documento que vincula cada requisito desde su **origen** (necesidad de negocio) hasta su **implementación** (desarrollo), **pruebas** y **validación**. Asegura que nada se olvida y todo está justificado.

### Estructura Básica

| ID Req | Origen (Necesidad)              | Tipo         | Descripción                                                       | Prioridad (MoSCoW) | Implementación (Código/Módulo) | Prueba Asociada                | Estado       | Línea Base |
| ------ | ------------------------------- | ------------ | ----------------------------------------------------------------- | ------------------ | ------------------------------ | ------------------------------ | ------------ | ---------- |
| RF-01  | Ciudadano necesita ver reportes | Funcional    | Mostrar mapa interactivo con reportes geolocalizados              | Must Have          | App Móvil - Maps SDK           | Caso de Prueba 01              | Implementado | ✓          |
| RF-02  | Necesidad de reporte rápido     | Funcional    | Crear reporte con GPS, foto, descripción                          | Must Have          | App + Backend API              | Caso de Prueba 02              | Implementado | ✓          |
| RF-03  | ENSU 86.4% baches               | Funcional    | Categorías: Baches, Agua, Luz, Coladeras, Basura, Infraestructura | Must Have          | App + Portal                   | Caso de Prueba 03              | Implementado | ✓          |
| RNF-01 | Criticidad operativa            | No Funcional | Disponibilidad 99.9%                                              | Must Have          | Infraestructura Cloud SLA      | Prueba de Estrés               | En prueba    | ✓          |
| RNF-04 | Escalabilidad                   | No Funcional | Soportar 100,000 usuarios concurrentes                            | Must Have          | Auto-scaling AWS/Azure         | Prueba de Estrés (Obligatoria) | En prueba    | ✓          |
| RN-01  | LGPDPPSO                        | Regla Legal  | Aviso de Privacidad obligatorio                                   | Must Have          | App - Módulo Perfil            | Validación Legal               | Implementado | ✓          |
| RN-02  | LGPDPPSO                        | Regla Legal  | Derechos ARCO accesibles                                          | Must Have          | App/Portal - Configuración     | Validación Legal               | Implementado | ✓          |

### Requisitos Principales (Muestra)

**Requisitos Funcionales de App Móvil:**

- RF-01: Mapa interactivo con reportes
- RF-02: Crear reporte (GPS + foto + descripción)
- RF-03: Seleccionar categoría (6 opciones)
- RF-04: Geocodificación automática
- RF-05: Validación de duplicados (50 metros)
- RF-06: Confirmación ciudadana (crowdsourcing)
- RF-07: Ciclo de vida del reporte (5 estados)
- RF-08: Notificaciones push
- RF-09: Filtros por categoría/estado
- RF-10: Historial de reportes del usuario
- RF-11: Autenticación (email/Google/Apple)
- RF-12: Mapa de calor de densidad

**Requisitos Funcionales Portal Web:**

- RF-13: Autenticación 2FA + roles
- RF-14: Mapa de calor en tiempo real
- RF-15: Actualizar estado + comentarios internos
- RF-16: Asignar a área responsable + fecha compromiso
- RF-17: Dashboard KPIs (abiertos, en proceso, resueltos, tiempo promedio)
- RF-18: Exportar reportes PDF/Excel
- RF-19: Alerta automática por email si pasan 72 horas sin cambio

**Requisitos No Funcionales:**

- RNF-01: Disponibilidad 99.9% mensual
- RNF-02: Tiempo de carga <3 segundos (4G), respuesta API <2 segundos
- RNF-03: Precisión GPS <10 metros
- RNF-04: Soporte 100,000 usuarios concurrentes
- RNF-05: Cifrado TLS 1.2 en tránsito, AES-256 en reposo
- RNF-06: Compatible iOS 14+, Android 9+

**Reglas de Negocio (LGPDPPSO, Transición, Calidad):**

- RN-01: Aviso de Privacidad previo a registro
- RN-02: Módulo ARCO funcional
- RN-03: Bitácora de auditoría (audit log)
- RN-04: Capacitación documentada a 3 alcaldías
- RN-05: Carga inicial de datos geográficos
- RN-06: Manuales de usuario y administrador
- RN-07: Cobertura pruebas 80%, bugs críticos <1%
- RN-08: Prueba de estrés 100,000 usuarios (OBLIGATORIA)
- RN-09: Presupuesto $0 en licencias
- RN-10: Plazo máximo 12 meses

---

## 10. EDT (ESTRUCTURA DE DESGLOSE DEL TRABAJO / WBS)

### Nivel 1: Proyecto Raíz

**Gestionar Desarrollo de App de Geolocalización para Reportes Urbanos**

### Nivel 2: Paquetes de Trabajo Principales

```
1. GESTIÓN DEL PROYECTO
   1.1 Planificación del Proyecto
       - Acta de Constitución
       - Plan de Gestión del Alcance
       - Plan de Gestión de Requisitos
       - Matriz de Trazabilidad
   1.2 Ejecución y Control
       - Reuniones de seguimiento semanales
       - Informes de avance quincenales
       - Control de cambios
       - Gestión de riesgos

2. ANÁLISIS Y LEVANTAMIENTO DE REQUERIMIENTOS (Mes 1)
   2.1 Recolección de Requisitos
       - Entrevistas con interesados
       - Workshop con alcaldías piloto
       - Análisis de ENSU 2025
   2.2 Documentación de Requisitos
       - Especificación de Requisitos de Software (SRS)
       - Historias de Usuario (ciudadano, operador, admin)
       - Casos de Uso con diagramas
   2.3 Priorización (MoSCoW)
       - Must Have (MVP obligatorio)
       - Should Have (post-lanzamiento)
       - Could Have (futuro)
   2.4 Requisitos Legales
       - Análisis LGPDPPSO
       - Aviso de Privacidad template
       - Protocolo ARCO
   2.5 Acuerdos Iniciales
       - MOUs con alcaldías
       - SLA con proveedores cloud

3. DISEÑO DE LA SOLUCIÓN (Mes 2)
   3.1 Diseño de Arquitectura
       - Arquitectura del Sistema
       - Diagrama de Componentes
       - Diagrama de Despliegue (cloud)
   3.2 Diseño de Base de Datos
       - Diagrama Entidad-Relación (ER)
       - Diccionario de datos
   3.3 Diseño de Aplicación
       - Diagrama de Clases (OOP)
       - Diagramas de Secuencia
       - Diagramas de Actividad
   3.4 Diseño de Interfaz
       - Wireframes (app móvil y portal web)
       - Mockups visuales
       - Prototipos interactivos
       - Validación de usabilidad
   3.5 Especificaciones Técnicas
       - API Specification (Swagger/OpenAPI)
       - Estándares de Codificación
       - Decisiones técnicas documentadas

4. DESARROLLO (Meses 3-7)
   4.1 Desarrollo Backend
       4.1.1 APIs REST
           - Endpoint reportes (GET, POST, PUT)
           - Endpoint usuarios (registro, autenticación)
           - Endpoint estadísticas/KPIs
       4.1.2 Integración de Servicios Externos
           - Google Maps API (Geocoding, Places)
           - Firebase Cloud Messaging
       4.1.3 Base de Datos
           - Diseño e implementación
           - Scripts de migración
       4.1.4 Infraestructura Cloud
           - Configuración AWS/Azure
           - Base de datos gestionada
           - Storage (S3/Blob)
   4.2 Desarrollo Frontend Móvil
       4.2.1 App iOS (Swift/Objective-C)
           - Mapa interactivo
           - Módulo de creación de reportes
           - Sistema de notificaciones
           - Gestión de sesión
       4.2.2 App Android (Kotlin/Java)
           - Mapa interactivo
           - Módulo de creación de reportes
           - Sistema de notificaciones
           - Gestión de sesión
   4.3 Desarrollo Frontend Web
       4.3.1 Portal Administrativo
           - Dashboard ejecutivo
           - Mapa de calor
           - Gestión de reportes
           - Generador de reportes (PDF/Excel)
   4.4 Integración Completa
       - APIs ↔ Base Datos
       - Apps ↔ Backend
       - Servicios externos ↔ Sistema
   4.5 Documentación de Código
       - Comentarios en código
       - README de cada módulo
       - Guías de contribución

5. PRUEBAS E INTEGRACIÓN (Meses 8-9)
   5.1 Pruebas Unitarias
       - Desarrollo de test cases
       - Ejecución Jest/pytest
       - Reporte de cobertura (objetivo 80%)
   5.2 Pruebas de Integración
       - Test de APIs
       - Test de módulos
       - Test de flujos completos
   5.3 Pruebas de Seguridad
       - Análisis OWASP Mobile Top 10
       - Test de penetración
       - Validación de cifrado (TLS 1.2, AES-256)
       - Reporte de vulnerabilidades
   5.4 Pruebas de Rendimiento
       - Prueba de Estrés (100,000 usuarios) - OBLIGATORIA
       - Test de carga gradual
       - Medición de tiempos de respuesta
   5.5 Pruebas de Aceptación
       - Validación funcional vs. requisitos
       - Validación con alcaldías piloto
       - Acta de aceptación
   5.6 Documentación de Pruebas
       - Plan de Pruebas
       - Casos de Prueba detallados
       - Reportes de Resultados

6. IMPLEMENTACIÓN Y PILOTO (Meses 10-11)
   6.1 Publicación en Tiendas
       - Preparación App Store (iOS)
       - Preparación Google Play (Android)
       - Publicación y aprobación
   6.2 Carga de Datos Iniciales
       - Colonias y códigos postales (3 alcaldías)
       - Polígonos de jurisdicción
       - Zonas geográficas
   6.3 Capacitación a Alcaldías
       - Sesión de capacitación personal (3 alcaldías)
       - Manual de Administrador entregado
       - Acta de Capacitación firmada
   6.4 Operación Piloto
       - Monitoreo de aplicación
       - Seguimiento de reportes
       - Recolección de retroalimentación
       - Ajustes menores
   6.5 Validación de Éxito Piloto
       - Mínimo 1,000 reportes procesados
       - Estabilidad del sistema
       - Retroalimentación documentada

7. CIERRE Y ENTREGA (Mes 12)
   7.1 Documentación Final
       - Manual de Usuario (App Ciudadana)
       - Manual de Administrador (Portal Web)
       - Documentación Técnica Completa
       - Arquitectura y decisiones técnicas
   7.2 Cumplimiento Legal
       - Aviso de Privacidad (LGPDPPSO) publicado
       - Módulo ARCO funcional
       - Bitácora de auditoría operativa
   7.3 Manual de Despliegue
       - Procesos de instalación
       - Configuración cloud
       - Procedimientos de actualización
   7.4 Lecciones Aprendidas
       - Retroalimentación de equipo
       - Identificación de mejoras
       - Documentación para futuros proyectos
   7.5 Aceptación Final
       - Acta de Aceptación del Proyecto
       - Firma de interesados
       - Transición a operación

8. CONTROL Y MONITOREO (Transversal a todas las fases)
   8.1 Gestión de Riesgos
       - Identificación de riesgos
       - Plan de mitigación
       - Monitoreo continuo
   8.2 Gestión de Cambios
       - Solicitudes de Cambio
       - Análisis de impacto
       - Aprobación (Director o Comité)
   8.3 Gestión de Calidad
       - Auditorías de proceso
       - Validación de estándares
       - Métricas de desempeño
   8.4 Comunicación
       - Reportes semanales
       - Reuniones de avance quincenales
       - Escalamientos según necesidad
```

### Relación EDT-Cronograma

Cada paquete de trabajo se asigna a una o más fases y tiene actividades específicas con duración y recursos asignados.

---

## 11. CRONOGRAMA DE ACTIVIDADES

### Formato: Tabla de Actividades (para Gantt)

| ID  | Actividad                        | Fase | Duración (semanas) | Mes  | Predecesora | Recurso                 |
| --- | -------------------------------- | ---- | ------------------ | ---- | ----------- | ----------------------- |
| 1.1 | Acta de Constitución             | 1    | 1                  | 1    | -           | Director                |
| 1.2 | Análisis de Interesados          | 1    | 1                  | 1    | 1.1         | PM + Stakeholders       |
| 2.1 | Recolección de Requisitos        | 1    | 2                  | 1    | 1.2         | Analista + Alcaldías    |
| 2.2 | Documentar SRS                   | 1    | 1                  | 1    | 2.1         | Analista                |
| 2.3 | Historias de Usuario             | 1    | 1                  | 1    | 2.1         | Analista + UX           |
| 2.4 | Casos de Uso                     | 1    | 1                  | 1    | 2.3         | Analista                |
| 2.5 | Matriz de Trazabilidad           | 1    | 1                  | 1    | 2.4         | Analista                |
| 3.1 | Diseño Arquitectura              | 2    | 1                  | 2    | 2.5         | Arquitecto              |
| 3.2 | Diseño Base de Datos (ER)        | 2    | 1                  | 2    | 3.1         | Arquitecto DB           |
| 3.3 | Diseño de Clases                 | 2    | 1                  | 2    | 3.1         | Diseñador OOP           |
| 3.4 | Wireframes y Mockups             | 2    | 1                  | 2    | 2.3         | UX/UI Designer          |
| 3.5 | Especificación APIs              | 2    | 1                  | 2    | 3.1         | Arquitecto API          |
| 4.1 | Configurar Infraestructura Cloud | 3    | 1                  | 3    | 3.5         | DevOps                  |
| 4.2 | Desarrollar APIs Backend         | 3-4  | 4                  | 3-4  | 3.5         | Backend Dev Team        |
| 4.3 | Desarrollar App iOS              | 3-5  | 6                  | 3-5  | 3.4         | iOS Developer           |
| 4.4 | Desarrollar App Android          | 3-5  | 6                  | 3-5  | 3.4         | Android Developer       |
| 4.5 | Desarrollar Portal Web           | 3-6  | 7                  | 3-6  | 3.4         | Frontend Developer      |
| 4.6 | Integrar Google Maps API         | 4    | 2                  | 4    | 4.2         | Backend Dev             |
| 4.7 | Integrar Firebase Messaging      | 4    | 2                  | 4    | 4.2         | Backend Dev             |
| 4.8 | Código Review y Estándares       | 3-6  | 12                 | 3-6  | 4.2-4.5     | Lead Developer          |
| 5.1 | Plan de Pruebas                  | 5    | 1                  | 5    | 4.8         | QA Lead                 |
| 5.2 | Pruebas Unitarias                | 5-6  | 4                  | 5-6  | 5.1         | QA Testers              |
| 5.3 | Pruebas de Integración           | 6    | 2                  | 6    | 5.2         | QA Testers              |
| 5.4 | Pruebas de Seguridad             | 6    | 2                  | 6    | 5.2         | Security Tester         |
| 5.5 | Prueba de Estrés (100k users)    | 6    | 1                  | 6    | 5.3         | Performance Tester      |
| 5.6 | Pruebas de Aceptación            | 7    | 1                  | 7    | 5.5         | QA + Alcaldías          |
| 6.1 | Publicar App Store               | 7    | 1                  | 7    | 5.6         | DevOps                  |
| 6.2 | Publicar Google Play             | 7    | 1                  | 7    | 5.6         | DevOps                  |
| 6.3 | Carga de Datos Geográficos       | 7    | 1                  | 7    | 4.1         | Data Manager            |
| 6.4 | Capacitación Alcaldía 1          | 8    | 1                  | 8    | 6.3         | Trainer                 |
| 6.5 | Capacitación Alcaldía 2          | 8    | 1                  | 8    | 6.3         | Trainer                 |
| 6.6 | Capacitación Alcaldía 3          | 8    | 1                  | 8    | 6.3         | Trainer                 |
| 6.7 | Operación Piloto                 | 8-9  | 8                  | 8-9  | 6.4-6.6     | Operations Team         |
| 6.8 | Monitoreo y Ajustes Piloto       | 8-9  | 8                  | 8-9  | 6.7         | Tech Support            |
| 7.1 | Documentación Técnica Final      | 9-10 | 2                  | 9-10 | 4.8         | Technical Writer        |
| 7.2 | Manual de Usuario                | 10   | 1                  | 10   | 3.4         | Technical Writer        |
| 7.3 | Manual de Administrador          | 10   | 1                  | 10   | 3.4         | Technical Writer        |
| 7.4 | Manual de Despliegue             | 10   | 1                  | 10   | 4.1         | DevOps                  |
| 7.5 | Validación LGPDPPSO              | 10   | 1                  | 10   | 7.1         | Compliance              |
| 7.6 | Lecciones Aprendidas             | 11   | 1                  | 11   | 6.8         | Project Manager         |
| 7.7 | Acta de Cierre                   | 12   | 1                  | 12   | 7.1-7.6     | Director + Stakeholders |

**Hitos Críticos (Ruta Crítica):**

- Mes 1: Requisitos completos
- Mes 2: Diseño aprobado
- Mes 3-7: Desarrollo sin retrasos
- Mes 8-9: Prueba de estrés OBLIGATORIA aprobada
- Mes 10-11: Piloto exitoso con 1,000 reportes
- Mes 12: Acta de Cierre firmada

---

## 12. HOJA DE RECURSOS

### Equipo ClearCode (Recursos Internos)

|Rol|Cantidad|Mes 1|Mes 2|Mes 3-7|Mes 8-9|Mes 10-11|Mes 12|Especialidad|
|---|---|---|---|---|---|---|---|---|
|Director de Proyecto|1|100%|100%|50%|50%|100%|100%|PMBOK, gestión|
|Analista/BA|2|100%|50%|20%|10%|-|20%|Requisitos, casos de uso|
|Arquitecto del Sistema|1|50%|100%|50%|30%|-|-|Diseño, cloud|
|Backend Developer|3|-|20%|100%|100%|50%|10%|APIs, bases datos|
|iOS Developer|1|-|-|100%|100%|50%|-|Swift, integración mapas|
|Android Developer|1|-|-|100%|100%|50%|-|Kotlin, integración mapas|
|Frontend Developer|1|-|-|80%|100%|50%|-|React/Vue, portal web|
|UX/UI Designer|1|50%|100%|30%|20%|10%|-|Wireframes, usabilidad|
|QA Lead|1|-|-|20%|100%|50%|10%|Plan pruebas, estrategia|
|QA Testers|2|-|-|10%|100%|50%|10%|Casos de prueba, ejecución|
|Security Tester|1|-|-|-|100%|30%|-|Seguridad, OWASP|
|DevOps/Infrastructure|1|-|50%|100%|50%|100%|50%|Cloud, deployment|
|Technical Writer|1|-|20%|10%|20%|50%|100%|Documentación, manuales|
|**TOTAL Personas**|**17**|-|-|-|-|-|-|-|

### Recursos Externos

|Recurso|Cantidad|Propósito|Costo|
|---|---|---|---|
|Google Maps Platform (Free Tier)|-|Geocoding, Maps SDK|$0|
|Firebase Cloud Messaging|-|Notificaciones push|$0 (Free Tier)|
|AWS o Azure (Free Tier)|-|Infraestructura cloud|$0 (durante 12 meses)|
|Alcaldías Piloto|3|Validación, capacitación, piloto|Colaborativo|
|Herramientas Open Source|-|Desarrollo, testing|$0|

### Distribución de Carga Trabajo (Esfuerzo Total)

- **Persona-Meses Totales:** ~65-70 PM (personas-mes)
- **Costo Estimado (solo para referencia, no presupuestado):** Depende de salarios internos
- **Presupuesto de Licencias:** **$0 pesos**

---

## 13. COSTOS DE LAS ACTIVIDADES

### Estructura de Costos

|Categoría|Subcategoría|Costo Estimado|Justificación|
|---|---|---|---|
|**SOFTWARE**||||
||Licencias desarrollo|$0|Open Source (GitHub, VS Code, Android Studio)|
||Servicios cloud|$0|AWS/Azure Free Tier durante desarrollo|
||APIs externas|$0|Google Maps, Firebase en Free Tier|
||**Subtotal Software**|**$0**||
|**INFRAESTRUCTURA**||||
||Servidores (cloud)|$0|AWS/Azure managed services|
||Almacenamiento BD|$0|Free Tier incluido|
||Almacenamiento imágenes|$0|S3/Blob Free Tier|
||**Subtotal Infraestructura**|**$0**||
|**RECURSOS HUMANOS**||||
||Equipo ClearCode (17 personas)|No presupuestado|Costo interno de la organización|
||Capacitadores externos|Bajo/Nulo|Personal ClearCode realiza capacitación|
||**Subtotal RRHH**|**No presupuestado**||
|**OTROS GASTOS**||||
||Capacitación alcaldías|$0-Bajo|Realizado por equipo ClearCode|
||Documentación/impresión|Bajo|Manuales en digital (PDF)|
||Viajes para capacitación piloto|Bajo|Depende ubicación alcaldías|
||**Subtotal Otros**|**Bajo**||
|**PRESUPUESTO TOTAL**||**$0 en licencias**|Cumple objetivo proyecto|

**Nota:** El proyecto define presupuesto $0 en licencias de software. Costos de RRHH son absorbidos por ClearCode como inversión estratégica.

---

## 14. PRESUPUESTO

### Línea Base del Costo: $0 en Licencias

**Estrategia de Presupuesto:**

- 100% Open Source para desarrollo
- Free Tier para todos los servicios cloud (AWS, Azure, Google, Firebase)
- Dentro de 12 meses, consumo bajo permite permanecer en Free Tiers

**Estimación de Costos Reales (Para Contexto - No Presupuestado):**

|Rubro|Estimación|Observación|
|---|---|---|
|Recurso Humano (17 personas × 65-70 PM)|$130,000 - $140,000 USD*|No presupuestado (inversión ClearCode)|
|Infraestructura Cloud (después Free Tier)|$0 durante Año 1|Posible escalamiento post-piloto|
|Google Maps (después free usage)|$0 - $200/mes (post-piloto)|Dependerá de volumen reportes|
|Firebase (después free messaging)|$0 durante Año 1|Monitoreo necesario|
|AWS/Azure (post free tier)|$0 durante Año 1|Plan escalamiento Año 2|
|**TOTAL LÍNEA BASE (Oficial)**|**$0**|**Cumple restricción presupuestal**|

*Estimación ilustrativa; costo real depende de salarios internos ClearCode.

### Presupuesto por Fase

|Fase|Licencias|Infraestructura|RRHH*|Total Oficial|
|---|---|---|---|---|
|1. Análisis (Mes 1)|$0|$0|~$20k|$0|
|2. Diseño (Mes 2)|$0|$0|~$18k|$0|
|3. Desarrollo (Meses 3-7)|$0|$0|~$45k|$0|
|4. Pruebas (Meses 8-9)|$0|$0|~$20k|$0|
|5. Piloto (Meses 10-11)|$0|$0|~$12k|$0|
|6. Cierre (Mes 12)|$0|$0|~$8k|$0|
|**TOTAL**|**$0**|**$0**|**~$123k***|**$0**|

*Costo RRHH es estimado y no se presupuesta en el proyecto; es absorción interna ClearCode.

### Cash Flow (Desembolsos Reales)

**Durante Desarrollo:** Prácticamente nulos (costos RRHH internos no desembolsados como proyecto)

**Cuándo Podrían Surgir Costos:**

- Después del piloto (Año 1 de operación)
- Si se requiere escalar más allá de Free Tiers
- Si se necesitan herramientas premium post-lanzamiento

---

## 15. EJEMPLO DE VALOR GANADO (EVM - EARNED VALUE MANAGEMENT)

### Introducción al Método

El Valor Ganado es una técnica de gestión de proyectos que mide el desempeño combinando **alcance**, **tiempo** y **costo** en un solo indicador.

**Conceptos Clave:**

- **BAC (Presupuesto Total):** Presupuesto total autorizado para el proyecto
- **PV (Valor Planificado):** Presupuesto para el trabajo planificado a cierta fecha
- **EV (Valor Ganado):** Valor del trabajo REALMENTE realizado a cierta fecha
- **AC (Costo Real):** Costo REAL incurrido a cierta fecha

**Variaciones:**

- **CV (Variación de Costo) = EV - AC**
    - CV > 0: Gastamos menos (favorable)
    - CV < 0: Gastamos más (desfavorable)
- **SV (Variación de Cronograma) = EV - PV**
    - SV > 0: Adelantado (favorable)
    - SV < 0: Atrasado (desfavorable)

**Índices:**

- **CPI (Índice Desempeño Costo) = EV / AC**
    - CPI > 1: Eficiente en costo
    - CPI < 1: Ineficiente
- **SPI (Índice Desempeño Cronograma) = EV / PV**
    - SPI > 1: Adelantado
    - SPI < 1: Atrasado
- **CSI (Índice Combinado) = CPI × SPI**
    - CSI > 0.9: Proyecto en buen estado
    - CSI 0.8-0.9: Requiere atención
    - CSI < 0.8: Crítico

---

### EJEMPLO: PROYECTO APP GEOLOCALIZACIÓN - ANÁLISIS AL MES 6

#### Escenario de Proyecto

- **Duración Total:** 12 meses
- **BAC (Presupuesto Total Oficial):** $0 pesos en licencias
- **Para Fines del Ejemplo:** Convertimos a "puntos de valor" o "unidades de trabajo" equivalentes

**Asumimos un presupuesto conceptual de 100 "unidades de valor" distribuidas:**

- Análisis (Mes 1): 10 unidades
- Diseño (Mes 2): 10 unidades
- Desarrollo (Meses 3-7): 50 unidades
- Pruebas (Meses 8-9): 20 unidades
- Piloto (Meses 10-11): 7 unidades
- Cierre (Mes 12): 3 unidades **Total BAC = 100 unidades**

#### Punto de Corte: Fin de Mes 6 (Mitad del Desarrollo)

|Fase|Duración Planificada|Valor Planificado (PV)|Valor Ganado (EV)|Gasto Real (AC)|
|---|---|---|---|---|
|Análisis (Mes 1)|1 mes|10|10|10|
|Diseño (Mes 2)|1 mes|10|10|10|
|Desarrollo (Meses 3-6)|4 meses|32 (de 50)|28|30|
|**Total Acumulado Mes 6**||**52**|**48**|**50**|

**Interpretación:**

- PV = 52: Debería haberse completado 52 unidades de valor al mes 6
- EV = 48: Realmente se completó 48 unidades de valor
- AC = 50: Se gastaron 50 unidades en recursos/costo

---

#### Cálculos de Variaciones e Índices

**Variación de Costos (CV):**

```
CV = EV - AC = 48 - 50 = -2 unidades
Interpretación: Hemos gastado MÁS de lo planificado. Desfavorable.
```

**Variación de Cronograma (SV):**

```
SV = EV - PV = 48 - 52 = -4 unidades
Interpretación: Vamos ATRASADOS respecto al plan. Hemos completado menos trabajo del planificado.
```

**Índice de Desempeño de Costo (CPI):**

```
CPI = EV / AC = 48 / 50 = 0.96
Interpretación: Por cada peso gastado, solo ganamos 0.96 pesos de valor. Ineficiente en costo.
Regla: CPI < 1 significa sobregasto.
```

**Índice de Desempeño de Cronograma (SPI):**

```
SPI = EV / PV = 48 / 52 = 0.923
Interpretación: Estamos al 92.3% del cronograma planificado. Hemos perdido ~8% de velocidad.
Regla: SPI < 1 significa atraso.
```

**Índice Combinado de Desempeño (CSI):**

```
CSI = CPI × SPI = 0.96 × 0.923 = 0.886
Interpretación: CSI = 0.886 está en rango 0.8-0.9 → Proyecto REQUIERE ATENCIÓN.
- No es crítico (CSI > 0.8)
- Pero se están acumulando desviaciones que podrían escalar
```

---

#### Diagnóstico y Acciones

**¿Qué está pasando?**

1. **Atraso en cronograma:** 4 unidades atrasadas = 8% de retraso
2. **Sobregasto:** 2 unidades gastadas de más
3. **Combinado:** CSI = 0.886 requiere intervención

**¿Por qué podría estar sucediendo?**

- Problemas técnicos en integración de APIs (Google Maps, Firebase)
- Cambios no previstos en requisitos
- Capacidad insuficiente del equipo de desarrollo
- Estimaciones optimistas en la planificación

**Acciones Correctivas Recomendadas:**

1. **Acelerar Desarrollo:**
    
    - Reasignar recursos: +1 programador backend
    - Reducir scope de features menos críticas temporalmente
    - Extender horas equipo (cuidar burnout)
2. **Analizar Sobregasto:**
    
    - Revisar consumo de infraestructura cloud (¿salió del free tier?)
    - Auditar gastos de recursos de RRHH
    - Buscar optimizaciones
3. **Replanificación:**
    
    - Evaluar si es posible recuperar los 4 días de atraso en Meses 7-9
    - Ajustar buffer de tiempo si es necesario
    - Monitoreo semanal de CV y SV
4. **Comunicación:**
    
    - Reportar a director y stakeholders
    - Presentar plan de recuperación
    - Establecer hito de "vuelta a la línea base"

---

#### Proyección a Finalización (Forecast)

**Si la tendencia continúa:**

```
Trabajo restante = BAC - EV = 100 - 48 = 52 unidades
Tiempo restante = 12 - 6 = 6 meses

Ritmo actual = 48 unidades / 6 meses = 8 unidades/mes
Tiempo para completar = 52 / 8 = 6.5 meses

PROYECCIÓN: Terminaríamos a mitad de mes 12.5 (fuera del plazo)
```

**Costo Estimado Final (EAC - Estimate at Completion):**

```
Tasa de costo actual = AC / EV = 50 / 48 = 1.042
Costo estimado para trabajo restante = (52 / 0.96) = 54.17 unidades
EAC = AC + ETC = 50 + 54.17 = 104.17 unidades (versus BAC = 100)

Variación final estimada (VAC) = BAC - EAC = 100 - 104.17 = -4.17 unidades
```

**Conclusión:** El proyecto estaría **0.5 meses atrasado y 4.17 unidades sobrepresupuestado** si no hay intervención.

---

#### Tabla Resumen del Ejemplo (Mes 6)

|Métrica|Valor|Interpretación|
|---|---|---|
|**BAC**|100|Presupuesto total autorizado|
|**PV (Planificado)**|52|Trabajo que debería estar listo|
|**EV (Realizado)**|48|Trabajo REALMENTE completado|
|**AC (Gastado)**|50|Costo REAL incurrido|
|**CV**|-2|Sobregasto de 2 unidades|
|**SV**|-4|Atraso de 4 unidades|
|**CPI**|0.96|Ineficiencia: solo 0.96 por peso gastado|
|**SPI**|0.923|Retraso: 92.3% del cronograma|
|**CSI**|0.886|Estado: REQUIERE ATENCIÓN (0.8-0.9)|
|**EAC (Proyección)**|104.17|Costo estimado final|
|**VAC (Proyección)**|-4.17|Varianza final estimada|

---

#### Gráfico Conceptual (Descripción para Diapositiva)

```
Línea Base del Alcance (BAC = 100)
│
100 ├─────────────────────────────────── BAC
    │
    │     Mes 6
    │     ↓
  50 ├─────●─────────────────────────── AC (Costo Real)
    │    /
    │   / PV (Valor Planificado)
 48 ├──────● ↑ Brecha SV = -4 (ATRASO)
    │    /  │
    │   /   ↓ EV (Valor Ganado)
    │  /
    │ /
    └──────────────────────────────────
      1   6    12 meses
    
Variación de Costo (CV) = EV - AC = 48 - 50 = -2 (SOBREGASTO)
Variación de Cronograma (SV) = EV - PV = 48 - 52 = -4 (ATRASO)
```

---

#### Aplicación Práctica al Proyecto Real

**En un proyecto real, cada mes se:**

1. Recolectaría PV de las actividades planificadas
2. Evaluaría EV de trabajo COMPLETADO (no iniciado ni en progreso)
3. Registraría AC de costos reales incurridos
4. Calcularía CV, SV, CPI, SPI, CSI
5. Tomaría decisiones correctivas si algún índice se desviaba

**Ejemplo real en App Geolocalización:**

- Mes 1: ✓ Análisis completado (PV=10, EV=10, AC=10) → Sin variación
- Mes 2: ✓ Diseño completado (PV=10, EV=10, AC=10) → Sin variación
- Mes 3: Desarrollo iniciado (PV=8, EV=6, AC=8) → CV=-2, SV=-2 (empieza el atraso)
- Mes 4-6: Atraso acumula...
- **Mes 6:** Como en el ejemplo (estado requiere atención)
- **Meses 7-9:** Plan de recuperación en ejecución
- **Mes 12:** Esperar haber cerrado la varianza

---

## 16. CONCLUSIONES PERSONALES

_(Esta sección será completada por el estudiante con reflexiones propias, pero aquí menciono qué debería incluir)_

**Puntos a Desarrollar:**

1. **Aprendizajes principales sobre gestión de proyectos**
    
    - Importancia de la línea base (alcance, tiempo, costo)
    - Rol del PMBOK en estructurar el proyecto
    - Valor del análisis de interesados
2. **Reflexión sobre el proyecto específico**
    
    - Relevancia social: Soluciona problema real (98.2% población con problemas urbanos)
    - Desafíos identificados: Presupuesto $0, plazo estricto, adopción ciudadana
    - Oportunidades: Modelo escalable SaaS, impacto en ciudades inteligentes
3. **Desafíos observados**
    
    - Integración de APIs externas (Google, Firebase)
    - Cumplimiento LGPDPPSO simultáneamente con desarrollo
    - Validación en piloto (lograr 1,000 reportes en 2 meses)
    - Capacitación y adopción municipal
4. **Fortalezas del proyecto**
    
    - Metodología cascada clara para MVP
    - Gobernanza definida (3 líneas base)
    - Énfasis en calidad (prueba de estrés obligatoria)
    - Documentación exhaustiva
5. **Recomendaciones para ejecución**
    
    - Mantener monitoreo de Valor Ganado mensualmente
    - Buffers de tiempo en actividades críticas
    - Comunicación semanal con alcaldías
    - Plan de mitigación de riesgos activo

[[Guión de Exposición Gesión de Proyectos]]