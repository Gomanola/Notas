# Módulo 1: Gestión de Cumplimiento
## Introducción
Es recomendable completar el curso de Defensa de la Red como requisito previo.
Se crearán documentos de políticas que cubran la gobernanza y el cumplimiento. Se aprenderá sobre el cumplimiento de estándares de ética y marcos legales y regulatorios. Además, aprenderá a evaluar la vulnerabilidad de la red y los sistemas y creará un plan de gestión de riesgos. Finalmente, aprenderá sobre la respuesta posterior a un incidente, incluidas las nvestigaciones forenses, los métodos de recuperación y la planificación de la respuesta a incidentes. Todas estas acciones son aspectos críticos de la seguridad de red.
Estos materiales del curso brindarán el conocimiento y las habilidades que necesita para hacer lo siguiente:
- Evaluar los controles de seguridad de acuerdo con los requisitos de cumplimiento ético, regulatorio y legal.
- Utilizar herramientas para las pruebas de seguridad de la red.
- Evaluar las fuentes de inteligencia de amenazas.
- Explique cómo se evalúan y administran las vulnerabilidades de los terminales.
- Seleccionar controles de seguridad basados en los resultados de la evaluación de riesgos. Utilizar modelos de respuesta a incidentes y técnicas forenses para investigar incidentes de seguridad.
### Descargar e Instalar Packet Tracer
[https://www.netacad.com/resources/lab-downloads](https://www.netacad.com/resources/lab-downloads?courseLang=es-XL)
### Introducción a Cisco Packet Tracer
Packet Tracer es una herramienta que permite simular redes reales. Proporcionar tres menús principales:
- Puede agregar dispositivos y conectarlos a través de cables o inalámbricos.
- Puede seleccionar, eliminar, inspeccionar, etiquetar y agrupar componentes dentro de la red.
- Puede administrar su red abriendo una red existente o de muestra, guardando la red actual y modificando su perfil de usuario o preferencias.
A los modelos más nuevos de dispositivos de red se puede acceder a través de un puerto USB para la configuración de la administración. Esto es necesario porque los portátiles y los PC más recientes normalmente no incluyen un puerto TS232 para las conexiones de cables de consola.
En Packet Tracer, se puede almacenar un inventario de dispositivos en el estante. Estos dispositivos se apagan y se pueden configurar e implementar previamente para reemplazar o agregar a los dispositivos de producción en el rack.
Todas las computadoras requieren de un sistema operativo para funcionar, incluso los dispositivos de red basados en PC, como switches, routers, puntos de acceso y firewalls. Un sistema operativo de red habilita el hardware del dispositivo que funcione y proporciona una interfaz para que los usuarios interactúen.
El Cisco Internetwork Operating System (IOS) es un sistema operativo que se utiliza en los dispositivos de red de Cisco. Permite la creación de configuraciones que personalizan el funcionamiento de los dispositivos de red en diferentes entornos de red. Se puede acceder a la CLI a través del puerto de la consola del dispositivo mediante el software de terminal o de forma remota mediante Secure Shell (SSH). Los administradores de red utilizan una computadora para acceder a la consola del dispositivo con el fin de crear o modificar la configuración del dispositivo.
Los administradores de red suelen asignar un nombre a los dispositivos de red. El nombre de host se usa para identificar un dispositivo cuando se accede a su sistema operativo para la conexión de consola al Backup_Router. Una vez configurado el nombre de host, el nombre de host aparece como parte del símbolo del sistema IOS.
## Gestión y Cumplimiento
La gobernanza es  un tema importante en la ciberseguridad, ya que describir las políticas y los procesos vigentes dentro de una organización que definen las responsabilidades por la aplicación y la rendición de cuentas para mitigar el riesgo cibernético. Estos también deben alinearse con las regulaciones clave.
Como profesional de la ciberseguridad, debe tener conocimiento de las diferentes leyes que regulan la seguridad de la información, la ciberseguridad y la privacidad dentro de su país para garantizar el cumplimiento de la organización. Y no olvidemos su obligación ética de hacer siempre lo correcto.
### Gobernanza
#### Gestión
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
#### Políticas de Ciberseguridad
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
#### Tipos de Políticas de Seguridad
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
### Desarrollando Políticas y Procedimientos de Ciberseguridad
[[1.1.6 Práctica de Laboratorio - Desarrollando Políticas y Procedimientos de Ciberseguridad]]
### Principios Rectores para los Recursos Humanos
El equipo de TI de @Apollo está preocupado. Identificaron algunas amenazas de dominio de usuario y solicitaron asesoramiento sobre qué contramedidas podrían implementar para manejar estas amenazas.
Basado en lo que ha aprendido durante este curso hasta ahora, ¿puede recomendar que control de seguridad deben implementar para abordar cada amenaza?
1. Un alto porcentaje de empleados que trabajan remotamente hacen clic en correos electrónicos de suplantación de identidad
	**Respuesta**: Realice una capacitación de conocimiento sobre seguridad
	Para evitar que los empleados sean víctimas de estafas de suplantación de identidad, debe realizar una capacitación de concientización sobre la seguridad. Esto puede implicar la exhibición de afiches de concientización sobre la seguridad, la educación de los empleados sobre políticas clave y el envío de recordatorios por correo electrónico a los empleados
2. Los gerentes de proyecto pueden acceder a todos los datos de clientes de @Apollo en una unidad compartida, incluso para proyectos en los que no están trabajando
	**Respuesta**: Aplique controles de acceso de usuarios
	El principio de "necesidad de saber" establece que un empleado solo debe tener acceso a la información que necesita para realizar su trabajo. Por lo tanto, cada uno de los gerentes de proyecto de @Apollo solo debe estar autorizado a acceder a los datos del cliente para los proyectos en los que está trabajando. El acceso a todos los demás datos, incluidos datos de otros clientes, debe restringirse mediante controles de acceso de usuario
3. Los empleados del departamento de Diseño Gráfico en particular están descargando versiones no autorizadas de software en sus dispositivos de trabajo
	**Respuesta**: Habilitar monitoreo de IDS/IPS
	La descarga de programas o archivos no autorizados aumenta la probabilidad de infecciones de malware.  @Apollo debe habilitar análisis de virus automáticos para archivos adjuntos y descargas de correo electrónico y habilitar el monitoreo de IDS/IPS para combatir esta amenaza
4. Los empleados que trabajan remotamente están usando VPNs para ver películas en sus dispositivos de trabajo
	**Respuesta**: Realice el seguimiento y monitoree el comportamiento anormal de los empleados
	Una conexión VPN permite a los empleados remotos enrutar su actividad en línea a través de un servidor que los conecta directamente a la red de @Apollo. El desempeño laboral errático y el uso de la infraestructura de TI fuera del horario laboral normal pueden ser señales de que los empleados que trabajan remotamente están usando VPN no autorizadas en sus dispositivos de trabajo, lo que puede mitigarse mediante el seguimiento y la supervisión del comportamiento anormal de los empleados
Las medidas adicionales que las organizaciones pueden implementar para administrar las amenazas de los usuarios incluyen:
- Vincular la concientización de seguridad con los objetivos de revisión de desempeño
- Habilitar el filtrado de contenido para permitir o rechazar nombres de dominio específicos conforme a las políticas de uso aceptable
- Deshabilitar las unidades de CD internas y los puertos USB
- Habilitar el análisis de malware automático para unidades de medios insertas, archivos y archivos adjuntos de correo electrónico
- Asignar permisos de escritura y borrado únicamente al propietario de los datos
### Manejo de Amenazas al Usuario
Es posible que haya aprendido que, como profesional de ciberseguridad, tiene las mismas habilidades que un ciberdelincuente.
De hecho, la ética es el código de comportamiento que lo distingue.
## La Ética de la Ciberseguridad
La ética es la pequeña voz en su cabeza que le dice lo que está bien y lo que está mal, y lo guía para tomar decisiones correctas. Como especialista en ciberseguridad, debe comprender tanto la ley como los intereses de una organización para poder tomar tales decisiones.
La ética puede verse desde muchas perspectivas diferentes.
**Ética utilitarista**
	Durante el siglo diecinueve, los filósofos Jeremy Bentham y John Stuart Mill articularon la teoría de la ética utilitarista. Esto se basa en el principio rector de que la consecuencia de una acción es el factor más importante para determinar si la acción es moral o no. Por ejemplo, una acción que maximice el mayor bien para la mayor cantidad de personas es una opción ética.
**El enfoque de los derechos**
	El enfoque de derechos se guía por el principio que establece que un individuo tiene derecho a tomar sus propias decisiones, que no pueden ser violadas por la decisión de otra persona. Esta decisión debe respetar y considerar los derechos fundamentales del individuo. Estos derechos fundamentales incluyen el derecho a la verdad, la privacidad, la seguridad y que la sociedad aplique las leyes de manera justa a todos los miembros de la sociedad.
**El enfoque del bien común**
	El enfoque del bien común propone que las acciones éticas son las que benefician a toda la comunidad. Desafía a las personas a reconocer y perseguir los valores y objetivos compartidos con otros miembros de una comunidad.
Como especialista en ciberseguridad, a menudo no habrá una respuesta obvia a los problemas éticos con los que se encuentre. El curso de acción correcto dependerá de la situación y la respectiva ética que utilice para guiar su decisión.
### Los Diez Mandamientos de la Ética Informática
Situado en Washington, DC, el Instituto de Ética Informática es un recurso que identifica, evalúa y responde a problemas éticos en el sector de la tecnología de la información.
Crearon lo diez mandamientos de ética informática presentados aquí.
1. No usarás una computadora para dañar a otras personas
2. No interferirás con el trabajo informático de otras personas
3. No husmearás en los archivos informáticos de otras personas
4. No usarás una computadora para robar
5. No usaras una computadora para dar falso testimonio
6. No copiarás ni utilizarás software propietario por el que no hayas pagado
7. No utilizarás los recursos informáticos de otras personas sin autorización o compensación adecuada
8. No te apropiarás de la producción intelectual de otras personas
9. Deberás pensar en las consecuencias sociales del programa que estás escribiendo o del sistema que estás diseñando
10. Siempre usarás una computadora de manera que garantice la consideración y el respeto por tus semejantes
### Explorando la Ética Cibernética
Su ética cibernética se someterá regularmente a prueba.
Echemos un vistazo a algunas situaciones de empleados que usted ha presenciado en @Apollo. En cada caso, ¿puede identificar si el empleado tomó la decisión correcta o incorrecta?
Utilice los diez mandamientos de la ética informática como guía y seleccione "Correcto" si cree que el empleado ha tomado una decisión ética o "Incorrecto" si cree que el empleado ha tomado una decisión poco ética.
- Actualizar el plan de proyecto de un colega después de notar un error (**Incorrecto**)
	'No interferirás con el trabajo de otras personas en la computadora' — por lo tanto, actualizar el plan de proyecto de un colega, incluso si ha notado un error, **no es ético**.
- Publicar un mensaje en el foro interno de @Apollo para agradecer a un colega por su ayuda (**Correcto**)
	'Utilizarás una computadora de manera que garantice la consideración y el respeto por tu prójimo' — por lo tanto, publicar un mensaje de agradecimiento en un foro en línea **es lo correcto**.
- Iniciar sesión en una aplicación de terceros utilizando los detalles de un colega cuando el administrador no está disponible (**Incorrecto**)
	'No utilizarás los recursos informáticos de otras personas sin autorización' — por lo tanto, iniciar sesión en una aplicación de terceros con los datos de un colega, incluso si el administrador no está disponible para otorgarle acceso, **no es ético**.
- Descargar archivos de música con derechos de autor para escuchar en el trabajo (**Incorrecto**)
	'No copiarás ni utilizarás software de propiedad exclusiva por el cual no has pagado' — por lo tanto, **no es ético** descargar archivos de música con derechos de autor.
- Quejarse del trabajo de un colega en un grupo de chat privado (**Incorrecto**)
	'No utilizará una computadora para dañar a otras personas' — por lo tanto, **no es ético** quejarse del trabajo de un colega en un grupo de chat privado.
- Acreditar una fuente en una publicación de blog (**Correcto**)
	'No te apropiarás de la producción intelectual de otras personas' — por lo tanto, atribuir crédito a una fuente en una publicación de blog **es lo correcto**.
- Acceder a los archivos de un cliente para ver cómo un colega está tratando su caso (**Incorrecto**)
	'No espiarás los archivos informáticos de otras personas' — por lo tanto, **no es ético** acceder a los archivos de un cliente para ver cómo un colega se ocupa de su caso.
### Delito Cibernético
El delito cibernético se divide en tres categorías:
1. **El delito informático** es donde una computadora es el blanco de actividades delictivas. Los ejemplos incluyen ataques de malware, el hackeo o ataques de denegación de servicio.
2. **El delito asistido por computadora** ocurre cuando una computadora se utiliza para cometer un delito, como robo o fraude.
3. Un **delito incidental informático** es cuando una computadora proporciona información incidental aun delito real. Por ejemplo, una computadora se utiliza para almacenar videos descargados ilegalmente, no es la herramienta real utilizada para cometer el delito.
Hay muchas herramientas conectadas a internet, muchas de las cuales no requieren mucha experiencia para su uso, que están contribuyendo al conocimiento exponencial del delito cibernético. De hecho, el delito cibernético está creciendo mucho más rápido que la capacidad del sistema legal para crear las leyes y regulaciones que lo prohíben.
Existen varias agencias que trabajan para combatir el delito cibernético, incluido el Centro de Quejas por Delitos en Internet (IC3) de la Oficina Federal de Investigaciones, InfraGard y la Asociación de la Industria de Software e Información (SIIA) en los Estados Unidos.
### Derecho Cibernético
Las leyes existen para prohibir los comportamientos no deseados. En los Estados Unidos, hay tres fuentes principales de leyes y regulaciones, las cuales involucran aspectos de seguridad informática.

> [!NOTE] Ley estatutaria
> El congreso de los Estados unidos ha establecido agencias administrativas federales y un marco de trabajo regulatorio que incluye sanciones civiles y penales para quienes incumplen las reglas.
> Los derechos penales aplican un código moral comúnmente aceptado respaldado por la autoridad gubernamental. Por ejemplo, la Ley de Fraude y Abuso Informático es una ley estatutaria que prohíbe el acceso a una computadora sin autorización o en exceso de autorización. La violación de estas reglas puede dar lugar a una multa o una pena de prisión.

> [!NOTE] Derecho administrativo
> Un marco legal que rige las actividades de las agencias administrativas del gobierno, el derecho administrativo garantiza que los organismos públicos actúen de conformidad con la ley.
> Por ejemplo, la Comisión Federal de Comunicación (FCC) y la Comisión Federal de Comercio (FTC) se ocupan de problemas tales como el fraude y el robo de la propiedad intelectual.

> [!NOTE] Derecho común
> Los casos de derecho común resuelven sus problemas a través del sistema judicial que proporciona precedentes y bases constitucionales para la elaboración de leyes.

### Ley Federal de Administración de Seguridad de la Información (FISMA)
Los sistemas federales de TI contienen y utilizan una gran cantidad de información valiosa y, por lo tanto, se consideran objetivos de alto valor para los ciberdelincuentes.
En 2002, el Congreso de los Estados Unidos creó FISMA para cubrir los sistemas de TI de las agencias federales. Específicamente, FISMA estipula que las agencias federales deben crear un programa de seguridad de la información que incluya:
- Evaluación de riesgos
- Un inventario anual de los sistemas de TI
- Políticas y procedimientos para reducir el riesgo
- Capacitaciones de concientización en seguridad
- Prueba y evaluación de todos los controles del sistema de TI
- Procedimientos de respuesta a incidentes
- Un plan de continuidad de operaciones
### Leyes Específicas de la Industria

> [!NOTE] Finanzas
> La Ley **Gramm-Leach-Bliley (GLBA)** es una ley que afecta principalmente la industria financiera. Sin embargo, una parte de esta legislación también proporciona disposiciones de exclusión voluntaria para las personas, lo que les otorga el control de cómo se utiliza la información que comparten con una organización durante una transacción comercial. La GLBA restringe el intercambio de información con organizaciones de terceros.

> [!NOTE] Contabilidad corporativa
> Luego de varios escándalos contables corporativos de alto perfil en los Estados Unidos, el Congreso aprobó la **Ley Sarbanes-Oxley (SOX)** en 2002 para revisar los estándares contables financieros y corporativos. Específicamente, apuntó a los estándares y prácticas financieras de las empresas que cotizan en bolsa en el país.

> [!NOTE] Tarjeta de crédito
> La industria privada también reconoce la importancia de las normas uniformes y exigibles y, en 2006, un Consejo de Normas de Seguridad compuesto por las principales organizaciones de la industria de las tarjetas de pago diseñó una iniciativa del sector privado para mejorar la confidencialidad de las comunicaciones de red.
> El **Estándar de seguridad de Datos de la Industria de Tarjetas de Pago (PCI DSS)** es un conjunto de reglas contractuales que buscan proteger los datos de pago del titular de la tarjeta de pago durante una transacción y reducir el fraude. En teoría, el PCI DSS es un estándar voluntario. Sin embargo, en la práctica, cualquier organización que almacene, procese o transmita datos de titulares de tarjetas que no cumplan con el estándar PCI DSS puede enfrentar tarifas de transacción significativamente más altas, multas de hasta USD 500 000 y, en circunstancias extremas, perder la capacidad de procesar tarjetas de pago.

> [!NOTE] Criptografía
> Las organizaciones que **importan o exportan productos de cifrado comerciales** están sujetas a regulaciones supervisadas por la Oficina de Industria y Seguridad del Departamento de Comercio.
> Las restricciones a la exportación a estados dudosos y organizaciones terroristas pueden estar vigentes debido a preocupaciones de seguridad nacional.
> Además, algunos países pueden decidir restringir la importación de tecnologías de criptografía debido a preocupaciones que:
> - La tecnología contiene una puerta trasera o una vulnerabilidad de seguridad.
> - Los ciudadanos pueden utilizar esta tecnología para comunicarse de forma anónima y eludir el monitoreo por parte de las autoridades.
> - Los niveles de privacidad podrían aumentar por encima de un nivel aceptable.
### Leyes de Notificación de Infracciones a la Seguridad
Las organizaciones grandes y pequeñas reconocen el valor de recopilar y analizar datos y, como resultado, recopilan una cantidad cada vez mayor de información personal sobre sus clientes. Los ciberdelincuentes siempre están buscando formas de obtener acceso a estos datos valiosos y aprovecharlos para su propio beneficios personal. Por lo tanto, todas las organizaciones que recopilan datos confidenciales deben ser buenos guardianes de estos datos.
Existen varias leyes en los Estados Unidos que exigen que las organizaciones notifiquen a las personas si se produce una violación de sus datos personales.

> [!NOTE] Ley de privacidad de las comunicaciones electrónicas
> El objetivo de la ley ECPA es garantizar la privacidad en el lugar de trabajo y proteger una variedad de comunicaciones electrónicas, como correo electrónico y conversaciones telefónicas, contra la intercepción, el acceso, el uso y la divulgación no autorizados.

> [!NOTE] Fraude informático y abuso
> Promulgada en 1986 como enmienda a la Ley de Control Integral del Delito de 1984, CFAA prohíbe el acceso no autorizado a los sistemas informáticos. A sabiendas, el acceso a una computadora del gobierno sin permiso o el acceso a cualquier computadora utilizada en el comercio interestatal o internacional es un delito penal. La ley también penaliza el tráfico de contraseñas o información de acceso similar y la transmisión intencionada de un programa, un código o un comando que de como resultado un daño.
### Protección de la Privacidad
**Ley de Privacidad de 1974**
	Esta ley establece un código de prácticas de información justa que rigen la recopilación, el mantenimiento, el uso y la transmisión de identificación personal de los individuos conservada