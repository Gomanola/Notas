# Introducción

Es recomendable completar el curso de Defensa de la Red como requisito previo.
Se crearán documentos de políticas que cubran la gobernanza y el cumplimiento. Se aprenderá sobre el cumplimiento de estándares de ética y marcos legales y regulatorios. Además, aprenderá a evaluar la vulnerabilidad de la red y los sistemas y creará un plan de gestión de riesgos. Finalmente, aprenderá sobre la respuesta posterior a un incidente, incluidas las nvestigaciones forenses, los métodos de recuperación y la planificación de la respuesta a incidentes. Todas estas acciones son aspectos críticos de la seguridad de red.

Estos materiales del curso brindarán el conocimiento y las habilidades que necesita para hacer lo siguiente:
- Evaluar los controles de seguridad de acuerdo con los requisitos de cumplimiento ético, regulatorio y legal.
- Utilizar herramientas para las pruebas de seguridad de la red.
- Evaluar las fuentes de inteligencia de amenazas.
- Explique cómo se evalúan y administran las vulnerabilidades de los terminales.
- Seleccionar controles de seguridad basados en los resultados de la evaluación de riesgos. Utilizar modelos de respuesta a incidentes y técnicas forenses para investigar incidentes de seguridad.

## Descargar e Instalar Packet Tracer
[https://www.netacad.com/resources/lab-downloads](https://www.netacad.com/resources/lab-downloads?courseLang=es-XL)

## Introducción a Cisco Packet Tracer
Packet Tracer es una herramienta que permite simular redes reales. Proporcionar tres menús principales:
- Puede agregar dispositivos y conectarlos a través de cables o inalámbricos.
- Puede seleccionar, eliminar, inspeccionar, etiquetar y agrupar componentes dentro de la red.
- Puede administrar su red abriendo una red existente o de muestra, guardando la red actual y modificando su perfil de usuario o preferencias.

A los modelos más nuevos de dispositivos de red se puede acceder a través de un puerto USB para la configuración de la administración. Esto es necesario porque los portátiles y los PC más recientes normalmente no incluyen un puerto TS232 para las conexiones de cables de consola.
En Packet Tracer, se puede almacenar un inventario de dispositivos en el estante. Estos dispositivos se apagan y se pueden configurar e implementar previamente para reemplazar o agregar a los dispositivos de producción en el rack.
Todas las computadoras requieren de un sistema operativo para funcionar, incluso los dispositivos de red basados en PC, como switches, routers, puntos de acceso y firewalls. Un sistema operativo de red habilita el hardware del dispositivo que funcione y proporciona una interfaz para que los usuarios interactúen.
El Cisco Internetwork Operating System (IOS) es un sistema operativo que se utiliza en los dispositivos de red de Cisco. Permite la creación de configuraciones que personalizan el funcionamiento de los dispositivos de red en diferentes entornos de red. Se puede acceder a la CLI a través del puerto de la consola del dispositivo mediante el software de terminal o de forma remota mediante Secure Shell (SSH). Los administradores de red utilizan una computadora para acceder a la consola del dispositivo con el fin de crear o modificar la configuración del dispositivo.
Los administradores de red suelen asignar un nombre a los dispositivos de red. El nombre de host se usa para identificar un dispositivo cuando se accede a su sistema operativo para la conexión de consola al Backup_Router. Una vez configurado el nombre de host, el nombre de host aparece como parte del símbolo del sistema IOS.

# Gestión y Cumplimiento

La gobernanza es  un tema importante en la ciberseguridad, ya que describir las políticas y los procesos vigentes dentro de una organización que definen las responsabilidades por la aplicación y la rendición de cuentas para mitigar el riesgo cibernético. Estos también deben alinearse con las regulaciones clave.
Como profesional de la ciberseguridad, debe tener conocimiento de las diferentes leyes que regulan la seguridad de la información, la ciberseguridad y la privacidad dentro de su país para garantizar el cumplimiento de la organización. Y no olvidemos su obligación ética de hacer siempre lo correcto.

## Gobernanza

### Gestión

La gobernanza de seguridad de TI determina quién está autorizado a tomar decisiones sobre los riesgos de ciberseguridad dentro de una organización. Demuestra responsabilidad y proporciona supervisión para garantizar que cualquier riesgo se mitigue adecuadamente y que las estrategias de seguridad estén alineadas con los objetivos comerciales de la organización y cumplan con las regulaciones.
La gobernanza de la seguridad de TI no debe confundirse con la administración de la seguridad de TI, la cual define e implementa los controles que una organización necesita para mitigar los riesgos. De manera similar, la gobernanza de datos en particular determina quién está autorizado a tomar decisiones sobre los datos dentro de una organización.
Hay varios roles clave en los buenos programas de gobernanza de datos.

| Sujeto                             | Descripción                                                                                                                                                                                                                                                |
| ---------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Propietario de datos               | Una persona que garantiza el cumplimiento de políticas y procedimientos, asigna la clasificación adecuada a los recursos de información y determina los criterios para acceder a los recursos de información.                                              |
| Controlador de datos               | Una persona que determina los fines para los cuales, y la manera en la cual, son procesados los datos personales.                                                                                                                                          |
| Procesador de datos                | Una persona u organización que procesa datos personales en nombre del controlador de datos.                                                                                                                                                                |
| Custodio de datos                  | Una persona que implementa la clasificación y los controles de seguridad de los datos de acuerdo con las reglas establecidas por el propietario de los datos. En otras palabras, los custodios de datos son responsables del control técnico de los datos. |
| Administrador de datos             | Una persona que garantiza que los datos cumplan las necesidades empresariales de una organización y cumplan con los requisitos reglamentarios.                                                                                                             |
| Funcionario de protección de datos | Una persona que supervisa la estrategia de protección de los datos de una organización.                                                                                                                                                                    |

### Políticas de Ciberseguridad

Una política de ciberseguridad es un documento de alto nivel que describe la visión de una organización para la ciberseguridad, incluidos sus objetivos, necesidades, alcance y responsabilidades. Específicamente:
- Demuestra el compromiso de una organización con la seguridad.
- Establece los estándares de comportamiento y requisitos de seguridad para llevar a cabo actividades, procesos y operaciones, y proteger los activos de tecnología e información dentro de una organización.
- Garantiza que la adquisición, el uso, el mantenimiento de la operación del sistema, software y hardware sean consistentes dentro de la organización.
- Definir las consecuencias legales de las violaciones a la políticas.
- Brinda al equipo de seguridad el soporte que necesitan de la alta gerencia.

| Política                           | Descripción                                                                                                                                                                                                                                                                                   |
| ---------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Política Maestra de Ciberseguridad | Como modelo para el programa de ciberseguridad de una organización, esta política sirve como plan estratégico para implementar controles de ciberseguridad.                                                                                                                                   |
| Política Específica del Sistema    | Este tipo de política se desarrolla para dispositivos o sistemas informáticos específicos y tiene como objetivo establecer la estandarización para aplicaciones aprobadas, software, configuraciones de sistemas operativos, hardware y contramedidas de refuerzo dentro de una organización. |
| Política de Problemas Específicos  | Este tipo de política se desarrolla para ciertos problemas operativos, circunstancias o condiciones que pueden requerir requisitos o instrucciones más detallados.                                                                                                                            |

### Tipos de Políticas de Seguridad

Una organización debe establecer políticas de seguridad claras y detalladas que todos los empleados conozcan. Es fundamental que estas políticas también cuenten con el respaldo del equipo de alta gerencia.

| Politica                                   | Descripción                                                                                                                                                                                                                                           |
| ------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Política de Identificación y Autenticación | Especifica quién debe tener acceso a los recursos de red y qué procedimientos de verificación existen para facilitar esto.                                                                                                                            |
| Política de Contraseñas                    | Definir los requisitos mínimos de contraseña, como la cantidad y el tipo de caracteres utilizados y la frecuencia con la que deben cambiarse.                                                                                                         |
| Política de Uso Aceptable                  | Destaca un conjunto de reglas que determinan el acceso y el uso de los recursos de red. También puede definir las consecuencias de infringir las políticas.                                                                                           |
| Política de Acceso Remoto                  | Establece cómo conectarse de forma remota a la red interna de una organización y explica qué información es accesible de forma remota.                                                                                                                |
| Política de Mantenimiento de la Red        | Describir los procedimientos para actualizar los sistemas operativos y las aplicaciones de usuario final de una organización.                                                                                                                         |
| Política de Manejo de Incidentes           | Proporciona orientación sobre cómo reportar y responder a incidentes relacionados con la seguridad dentro de una organización.                                                                                                                        |
| Política de Datos                          | Establece reglas mensurables para procesar datos dentro de una organización, como especificar dónde se almacenan los datos, cómo se clasifican los datos (alto, medio, bajo, confidencial, público o privado) y cómo se manejan y eliminan los datos. |
| Política de Credenciales                   | Aplica las reglas para crear credenciales, como la longitud mínima y máxima de una contraseña.                                                                                                                                                        |
| Política Organizacional                    | Proporciona orientación sobre cómo se debe realizar el trabajo en una organización. Los ejemplos pueden incluir políticas de administración de cambios, control de cambios o administración de activos.                                               |
