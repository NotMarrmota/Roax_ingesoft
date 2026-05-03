# DOCUMENTO DE ESPECIFICACIÓN DE REQUERIMIENTOS

## ROAX

---

**INTEGRANTES**

- Melisa Gomez Gomez
- Samuel Alejandro Estupiñan Gonzales
- Nicolas Ordoñez Cosio
- Juan Camilo Borrero Flores
- Juan Pablo Urbina Ladino
- Matius Montealegre Padilla

---
# **Tabla de Contenido**
 
1. Especificación de Requerimientos
   1.1 Descripción general
   1.2 Contexto del proyecto
   1.3 Requisitos 
   1.4 Subespecificación por subsistemas
   1.5 Tabla de asignación a subsistemas
2. PESTLE
3. RF1: Agente Conversacional
   3.1 Historias de usuario
   3.2 Casos de uso
   3.3 Formatos Bicolumnares
4. RF2: Recomendaciones Inteligentes
   4.1 Historias de usuario
   4.2 Casos de uso
   4.3 Formatos Bicolumnares
5. RF3: Gestión de Alertas
   5.1 Historias de usuario
   5.2 Casos de uso
   5.3 Formatos Bicolumnares
6. RF4: Retroalimentación y Aprendizaje
   6.1 Historias de usuario
   6.2 Casos de uso
   6.3 Formatos Bicolumnares
7. Backlog
8. MockUp
------

# **1. Especificación de Requerimientos**

## **1.1 Descripción General**

El presente documento describe el análisis, diseño y propuesta de solución para el Reto 4: Confianza Progresiva del proyecto ROAX by Dropi, desarrollado en el marco de la asignatura de Ingeniería de Software.

El reto consiste en diseñar un sistema que permita a la plataforma ROAX pasar de mostrar datos a tomar decisiones concretas por el usuario, construyendo gradualmente la confianza necesaria para que este delegue acciones críticas de su negocio a la inteligencia artificial. Para ello se identificaron requerimientos funcionales y no funcionales, se propuso una arquitectura de solución y se desarrolló un prototipo visual del agente inteligente.

## **1.2 Contexto del Proyecto**

ROAX by Dropi es una plataforma de inteligencia de negocio para e-commerce que integra datos de publicidad digital (Meta Ads, y próximamente TikTok) con datos reales de ventas y logística (Shopify, Tienda Nube, WooCommerce y Dropi), con el objetivo de calcular la rentabilidad real de un negocio digital.

La plataforma actualmente cuenta con más de 5.600 usuarios registrados y opera en dos modalidades: como módulo interno dentro de Dropi, y como plataforma externa independiente en app.roaxai.com, que es el foco del presente proyecto.

Hoy, ROAX funciona principalmente como una plataforma de reportería: conecta fuentes de datos, calcula métricas clave como ROAS, CPA, CTR, CPC y CPM, y genera alertas sobre el rendimiento de las campañas. Sin embargo, el modelo actual presenta una limitación estructural: muestra información pero no ayuda a tomar decisiones. El usuario debe interpretar solo qué significan los números y qué hacer con ellos, lo cual genera una alta fricción en la adopción del producto.

Con el avance de la inteligencia artificial, las plataformas de data enfrentan el reto de evolucionar: pasar de responder "¿qué está pasando?" a responder "¿qué debo hacer para mejorar mi negocio?". En este contexto, ROAX plantea su Refactor 2026, un proceso de rediseño profundo orientado a convertir la IA en el motor central de decisiones de la plataforma.

Dentro de este refactor se definen cuatro retos técnicos. El presente proyecto aborda el Reto 4: Confianza Progresiva, cuyo foco es diseñar el mecanismo mediante el cual un sistema de recomendaciones basado en IA logra que el usuario confíe en él, actúe sobre sus sugerencias, y permita que el sistema aprenda y mejore con el tiempo.

Este reto cobra especial relevancia dado el contexto del usuario de ROAX: un emprendedor o marca que invierte en promedio entre 1.500 y 2.000 dólares mensuales en publicidad digital, que opera en múltiples plataformas simultáneamente, y que ya ha desarrollado una desconfianza hacia las recomendaciones automáticas de Meta, debido a que estas priorizan el gasto publicitario por encima de la rentabilidad real del negocio.

## **1.3 Requisitos **

| **RF** | **Descripción** |
| --- | --- |
| **RF13** | El sistema debe permitir la comunicación con el usuario mediante un agente conversacional visual en tiempo real |
| **RF14** | El sistema debe generar y presentar recomendaciones inteligentes sobre campañas publicitarias basadas en análisis de datos y comportamiento histórico |
| **RF15** | El sistema debe gestionar alertas priorizadas sobre indicadores críticos del negocio evitando la saturación de información al usuario |
| **RF16** | El sistema debe gestionar la retroalimentación del usuario y ajustar progresivamente sus recomendaciones para construir confianza progresiva |

**Requerimientos No Funcionales**

| **RNF** | **Descripción** |
| --- | --- |
| **RNF1** | Disponibilidad: el sistema debe estar disponible 24/7 para monitoreo continuo de campañas |
| **RNF2** | Procesamiento en tiempo real: el sistema debe procesar y analizar datos con mínima latencia |
| **RNF3** | Interfaz de usuario: el sistema debe ofrecer una interfaz intuitiva, clara y orientada a la toma de decisiones |
| **RNF4** | Portabilidad: el sistema debe ser accesible desde múltiples dispositivos incluyendo móviles |
| **RNF5** | Interacción por voz: el sistema debe permitir interacción mediante audio procesando comandos en tiempo real |
| **RNF6** | Transparencia IA: el sistema debe hacer visible cuando una recomendación es generada por inteligencia artificial |

## **1.4 Subespecificación por Subsistemas**

**RF13 — Agente Conversacional Visual (ACV)**

| **ID** | **Subrequerimiento** |
| --- | --- |
| **ACV R13.1** | El sistema debe mostrar el avatar visual del agente mediante una ventana fija en la interfaz principal de la plataforma |
| **ACV R13.2** | El sistema debe reproducir la voz del agente mediante síntesis de voz clonada de actriz al momento de emitir una recomendación o alerta |
| **ACV R13.3** | El sistema debe mostrar el texto de la respuesta en un panel de conversación junto al avatar para usuarios que prefieran leer |
| **ACV R13.4** | El sistema debe permitir al usuario enviar mensajes al agente mediante un campo de texto o por entrada de voz |
| **ACV R13.5** | El sistema debe responder al usuario en lenguaje natural evitando tecnicismos innecesarios mediante el procesamiento del LLM |
| **ACV R13.6** | El sistema debe permitir al usuario activar o desactivar la voz del agente mediante un botón de configuración en la interfaz |

**RF14 — Recomendaciones Inteligentes (REC)**

| **ID** | **Subrequerimiento** |
| --- | --- |
| **REC R14.1** | El sistema debe identificar automáticamente campañas con bajo rendimiento mediante el análisis de métricas como ROAS, CPA, CTR y comportamiento histórico |
| **REC R14.2** | El sistema debe presentar cada recomendación en una tarjeta de acción que incluya la acción sugerida, la explicación basada en datos y la estimación de impacto esperado |
| **REC R14.3** | El sistema debe permitir al usuario interactuar con cada recomendación mediante tres opciones: Aplicar, Rechazar o Posponer, mostradas como botones diferenciados en la interfaz |
| **REC R14.4** | El sistema debe permitir al usuario expandir cada recomendación para acceder a una vista detallada con gráficas de evolución temporal y análisis del embudo de conversión |
| **REC R14.5** | El sistema debe solicitar y almacenar información cualitativa del negocio (inventario disponible, costos fijos, perfil del cliente) mediante un formulario de onboarding para mejorar la precisión de las recomendaciones |
| **REC R14.6** | El sistema debe mostrar, posterior a la aplicación de una recomendación, un seguimiento del impacto real versus el impacto estimado en formato antes/después con métricas en valores monetarios y porcentajes |

**RF15 — Gestión de Alertas (ALR)**

| **ID** | **Subrequerimiento** |
| --- | --- |
| **ALR R15.1** | El sistema debe enviar notificaciones inmediatas al usuario cuando detecte una campaña en situación crítica, priorizando aquellas con mayor impacto económico potencial |
| **ALR R15.2** | El sistema debe agrupar y priorizar las alertas según su impacto potencial mediante un sistema de pesos por indicador, mostrando un máximo de alertas críticas por sesión |
| **ALR R15.3** | El sistema debe analizar indicadores en conjunto (CTR + CPA + CBR) en lugar de dispararlos individualmente, para evitar la saturación de alertas al usuario |
| **ALR R15.4** | El sistema debe permitir al usuario configurar sus preferencias de notificación incluyendo canales (in-app, correo, push móvil), horarios de envío y nivel de criticidad mínimo |

**RF16 — Retroalimentación y Aprendizaje (RFA)**

| **ID** | **Subrequerimiento** |
| --- | --- |
| **RFA R16.1** | El sistema debe presentar al usuario un mecanismo de retroalimentación explícita que le permita calificar la utilidad de cada recomendación (útil, incorrecta, irrelevante) con comentario opcional |
| **RFA R16.2** | El sistema debe registrar retroalimentación implícita derivada del comportamiento del usuario: frecuencia de aceptación, tiempo antes de actuar, recomendaciones ignoradas y acciones revertidas |
| **RFA R16.3** | El sistema debe ajustar progresivamente sus recomendaciones en función del historial de comportamiento del usuario, incrementando la precisión de las sugerencias futuras de forma personalizada |
| **RFA R16.4** | El sistema debe permitir al usuario configurar niveles de automatización desde recomendaciones manuales hasta ejecución automática de acciones según su preferencia y nivel de confianza acumulada |
| **RFA R16.5** | El sistema debe mostrar al usuario un indicador de nivel de confianza acumulada con el agente de IA, reflejando el historial de recomendaciones aceptadas y sus resultados medibles |

## **1.5 Tabla de Asignación a Subsistemas**

| **Requerimiento** | **RF13 - ACV** | **RF14 - REC** | **RF15 - ALR** | **RF16 - RFA** |
| --- | --- | --- | --- | --- |
| Agente conversacional visual | **X** |  |  |  |
| Síntesis de voz clonada | **X** |  |  |  |
| Identificación de campañas |  | **X** |  |  |
| Tarjetas de recomendación |  | **X** |  |  |
| Opciones aplicar/rechazar/posponer |  | **X** |  |  |
| Datos cualitativos del negocio |  | **X** |  |  |
| Alertas priorizadas |  |  | **X** |  |
| Sistema de pesos de indicadores |  |  | **X** |  |
| Configuración de notificaciones |  |  | **X** |  |
| Retroalimentación explícita |  |  |  | **X** |
| Aprendizaje por comportamiento |  |  |  | **X** |
| Niveles de automatización |  |  |  | **X** |
| Indicador de confianza acumulada |  |  |  | **X** |

# **2. PESTLE**

El análisis PESTLE se aplica a los requerimientos funcionales que toman decisiones sobre personas, usan datos sensibles o pueden generar impacto negativo. Para cada dimensión se identifica el hallazgo, su impacto y el requerimiento derivado.

**PESTLE — RF13: Agente Conversacional Visual**

| **Dimensión** | **Hallazgo** | **Impacto** | **Requerimiento derivado** |
| --- | --- | --- | --- |
| **P — Político** | No existen regulaciones específicas sobre agentes de IA conversacionales en Colombia, pero el MINTIC puede establecer lineamientos sobre sistemas automatizados de toma de decisiones comerciales. | Si se regulan los agentes IA en comercio electrónico, el sistema podría quedar fuera de cumplimiento. | RNFP-1-01: El sistema debe documentar y hacer trazable toda acción sugerida o ejecutada por el agente de IA. |
| **E — Económico** | La síntesis de voz clonada y el procesamiento LLM en tiempo real implican costos por token y por llamada a APIs externas (ElevenLabs, OpenAI, etc.). | Si el costo por interacción es alto, la funcionalidad puede volverse inviable económicamente a escala con 5.600 usuarios. | RNFE-1-02: El sistema debe implementar caché de respuestas frecuentes del agente para reducir el costo de llamadas a APIs externas. |
| **S — Social** | Usuarios con menor alfabetización digital o con discapacidad auditiva pueden verse excluidos de la interacción verbal con el agente. | Un agente que solo funciona por voz excluye a usuarios con discapacidad auditiva o en entornos ruidosos. | RNFS-1-03: El sistema debe ofrecer siempre una alternativa textual a la interacción por voz, garantizando accesibilidad completa. |
| **T — Tecnológico** | La síntesis de voz en tiempo real requiere baja latencia. Conexiones lentas o dispositivos de gama baja pueden degradar la experiencia. | Si el agente tarda más de 3 segundos en responder, el usuario pierde confianza en el sistema. | RNFT-1-04: El sistema debe responder las consultas del agente en menos de 3 segundos bajo condiciones normales de red. |
| **L — Legal** | El agente conversa con el usuario y puede acceder a datos financieros del negocio. La Ley 1581 de Colombia (Habeas Data) exige protección de datos personales. | Almacenar conversaciones sin consentimiento o sin cifrado puede constituir una violación legal. | RNFL-1-05: El sistema debe cifrar todas las conversaciones almacenadas y obtener consentimiento explícito del usuario para su almacenamiento. |
| **E — Ético** | El agente usa voz clonada de una actriz real. El usuario puede confundirlo con una persona humana real. | Generar engaño sobre la naturaleza del agente viola principios de transparencia y puede erosionar la confianza del usuario. | RNFE-1-06: El sistema debe identificar al agente como inteligencia artificial al inicio de cada sesión de conversación. |

**PESTLE — RF14: Recomendaciones Inteligentes**

| **Dimensión** | **Hallazgo** | **Impacto** | **Requerimiento derivado** |
| --- | --- | --- | --- |
| **P — Político** | Meta Ads tiene términos de uso que restringen el acceso automatizado y la toma de decisiones sobre campañas vía API. Cambios en su política pueden invalidar funcionalidades. | Si Meta restringe el acceso API, el sistema pierde su fuente principal de datos para generar recomendaciones. | RNFP-2-01: El sistema debe diseñarse con una capa de abstracción de fuentes de datos para soportar cambios en las APIs de Meta sin rediseño mayor. |
| **E — Económico** | Un usuario promedio invierte 1.500-2.000 USD/mes en publicidad. Una recomendación incorrecta de pausar una campaña rentable puede generar pérdidas económicas directas. | Si el sistema genera una recomendación errónea y el usuario la sigue, puede perder ingresos significativos y abandonar la plataforma. | RNFE-2-02: El sistema debe mostrar el nivel de confianza (%) de cada recomendación y advertir cuando la certeza es baja antes de sugerir acciones críticas. |
| **S — Social** | Usuarios con poco conocimiento de métricas (ROAS, CPA) pueden no entender las recomendaciones aunque estén bien explicadas. | Si la explicación usa jerga técnica, el usuario no actúa sobre la recomendación y la plataforma pierde valor. | RNFS-2-03: El sistema debe traducir cada recomendación a lenguaje no técnico con analogías comprensibles para el usuario promedio del sector. |
| **T — Tecnológico** | El cálculo de recomendaciones en tiempo real requiere cruzar datos de Meta, Shopify y Dropi simultáneamente. Inconsistencias entre fuentes pueden generar recomendaciones incorrectas. | Una recomendación basada en datos desactualizados o inconsistentes puede llevar al usuario a tomar una decisión dañina. | RNFT-2-04: El sistema debe indicar en cada recomendación la fecha y hora de la última sincronización de datos de cada fuente. |
| **L — Legal** | Las recomendaciones pueden constituir asesoría financiera o comercial. En Colombia no existe regulación específica para IA en publicidad digital, pero sí para servicios de asesoría. | Si el sistema es considerado un servicio de asesoría financiera, podría requerir habilitación regulatoria. | RNFL-2-05: El sistema debe incluir un aviso claro de que las recomendaciones son sugerencias automatizadas y no constituyen asesoría financiera certificada. |
| **E — Ético** | El sistema aprende del comportamiento del usuario, pero puede reforzar sesgos si el usuario siempre acepta recomendaciones de un tipo y rechaza otras, creando un ciclo de confirmación. | El modelo puede volverse sesgado y dejar de explorar estrategias nuevas que podrían beneficiar al negocio. | RNFE-2-06: El sistema debe diversificar periódicamente el tipo de recomendaciones generadas para evitar sesgos de confirmación en el modelo de aprendizaje. |

**PESTLE — RF15: Gestión de Alertas**

| **Dimensión** | **Hallazgo** | **Impacto** | **Requerimiento derivado** |
| --- | --- | --- | --- |
| **P — Político** | No aplica directamente a la gestión de alertas internas. | — | — |
| **E — Económico** | El envío masivo de alertas por correo o push puede implicar costos por notificación según el proveedor (SendGrid, Firebase, etc.). | Con 5.600 usuarios y múltiples alertas diarias, los costos de notificación pueden escalar significativamente. | RNFE-3-01: El sistema debe implementar agrupación de alertas por sesión para reducir el volumen de notificaciones enviadas por usuario. |
| **S — Social** | El exceso de alertas genera fatiga en el usuario y puede llevar al abandono de la plataforma. Laura mencionó que llegaron a 250 alertas diarias. | Si el usuario desactiva todas las notificaciones por saturación, pierde el valor central de monitoreo del sistema. | RNFS-3-02: El sistema debe limitar las alertas críticas a un máximo configurable por el usuario por período de tiempo. |
| **T — Tecnológico** | El sistema de alertas debe operar 24/7 monitoreando campañas en tiempo real. Una falla del motor de alertas de madrugada puede dejar campañas sin monitoreo. | Un usuario que se acuesta con campañas activas puede amanece con pérdidas si el sistema de alertas falló. | RNFT-3-03: El sistema debe implementar redundancia en el motor de alertas y notificar al usuario si el monitoreo estuvo inactivo por más de 15 minutos. |
| **L — Legal** | Las alertas pueden contener información financiera sensible del negocio del usuario enviada por canales externos (correo, push). | El envío de datos financieros por canales no cifrados puede violar la Ley 1581 de protección de datos. | RNFL-3-04: El sistema debe cifrar el contenido de las notificaciones que incluyan métricas financieras del usuario. |
| **E — Ético** | El sistema prioriza alertas por impacto económico, lo que puede llevar a ignorar alertas de menor valor monetario pero alto impacto operacional para el negocio. | Un usuario pequeño puede no recibir alertas relevantes para su escala porque el sistema las considera de bajo impacto. | RNFE-3-05: El sistema debe permitir al usuario definir qué tipo de alertas considera críticas independientemente del impacto económico calculado. |

**PESTLE — RF16: Retroalimentación y Aprendizaje**

| **Dimensión** | **Hallazgo** | **Impacto** | **Requerimiento derivado** |
| --- | --- | --- | --- |
| **P — Político** | No existen regulaciones específicas sobre sistemas de aprendizaje automático en Colombia actualmente, pero la UE ya regula la IA de alto riesgo. ROAX opera en Latinoamérica pero puede expandirse. | Si ROAX expande a Europa o se regulan los sistemas de IA en Colombia, el motor de aprendizaje podría requerir auditoría. | RNFP-4-01: El sistema debe mantener logs auditables de cómo la retroalimentación del usuario modifica el modelo de recomendaciones. |
| **E — Económico** | El reentrenamiento del modelo con datos de retroalimentación puede requerir recursos computacionales significativos si se hace en tiempo real. | Si el costo de reentrenamiento es alto, el sistema puede limitarse a actualizaciones periódicas, reduciendo la personalización. | RNFE-4-02: El sistema debe implementar actualizaciones del modelo por lotes nocturnos para optimizar el costo computacional del aprendizaje. |
| **S — Social** | Usuarios que rechazan todas las recomendaciones por desconfianza inicial pueden impedir que el sistema aprenda correctamente de su comportamiento. | El sistema no puede personalizar si el usuario nunca interactúa, generando un ciclo de baja confianza. | RNFS-4-03: El sistema debe ofrecer un modo de observación donde el usuario pueda ver el impacto hipotético de recomendaciones sin necesidad de aplicarlas. |
| **T — Tecnológico** | El nivel de automatización configurable requiere integración directa con la API de Meta para ejecutar acciones (pausar, escalar). Cambios en permisos API pueden bloquear esta funcionalidad. | Si Meta revoca permisos de escritura, el modo de automatización completa deja de funcionar sin aviso al usuario. | RNFT-4-04: El sistema debe verificar el estado de los permisos de escritura de Meta antes de permitir al usuario activar el modo de automatización completa. |
| **L — Legal** | El historial de retroalimentación y comportamiento del usuario constituye un dato personal que requiere protección bajo la Ley 1581. | Almacenar patrones de comportamiento sin consentimiento explícito puede generar sanciones legales. | RNFL-4-05: El sistema debe informar al usuario que su historial de interacciones con el agente es almacenado y utilizado para personalizar recomendaciones, con opción de eliminarlo. |
| **E — Ético** | El sistema aprende a recomendar lo que el usuario acepta, no necesariamente lo que es mejor para su negocio. Puede reforzar malas prácticas si el usuario las valida repetidamente. | Un usuario que sistemáticamente escala presupuesto sin evaluar logística puede recibir más recomendaciones de ese tipo, agravando el problema. | RNFE-4-06: El sistema debe balancear el aprendizaje por preferencia del usuario con parámetros de rentabilidad objetiva para evitar reforzar decisiones dañinas. |

# **3. RF13 — Agente Conversacional Visual (ACV)**

## **3.1 Historias de Usuario**

| **Título de la Historia de Usuario** | **Interacción con el agente de IA** |
| --- | --- |
| **Yo, como** | usuario de ROAX (emprendedor o gestor de e-commerce) |
| **Quiero** | comunicarme con un agente de IA mediante voz o texto que me muestre su avatar en pantalla |
| **Para** | entender mis métricas y recomendaciones sin necesidad de interpretar dashboards complejos |
| **Criterios de Aceptación (Gherkin)** | |
| **Scenario 1** | Given el usuario accede a la plataforma ROAX When el agente se carga en la interfaz Then el sistema muestra el avatar visual del agente en una ventana fija y reproduce un saludo por voz |
| **Scenario 2** | Given el usuario envía un mensaje de texto al agente When el LLM procesa la consulta Then el agente responde en lenguaje natural en menos de 3 segundos con texto y voz simultáneos |
| **Scenario 3** | Given el usuario desea desactivar el audio When hace clic en el botón de configuración de voz Then el agente continúa respondiendo solo con texto sin reproducir audio |
| **Prioridad** | Alta |
| **Dependencias** | Integración con API de Meta, Shopify y Dropi (RF2) |


# **4. RF14 — Recomendaciones Inteligentes (REC)**

## **4.1 Historias de Usuario**

| **Título de la Historia de Usuario** | **Recibir y actuar sobre recomendaciones de campañas** |
| --- | --- |
| **Yo, como** | usuario de ROAX con campañas activas en Meta Ads |
| **Quiero** | recibir recomendaciones claras sobre qué hacer con mis campañas, con su justificación y estimación de impacto |
| **Para** | tomar decisiones informadas sin necesidad de ser experto en métricas publicitarias |
| **Criterios de Aceptación (Gherkin)** | |
| **Scenario 1** | Given el sistema detecta una campaña con CPA superior al umbral rentable When genera la recomendación Then muestra una tarjeta con la acción sugerida, la explicación en lenguaje simple y la estimación de impacto en pesos |
| **Scenario 2** | Given el usuario revisa una recomendación When hace clic en Aplicar Then el sistema ejecuta la acción, registra el timestamp y comienza el seguimiento de impacto real |
| **Scenario 3** | Given el usuario hace clic en Rechazar When selecciona un motivo opcional Then el sistema registra el rechazo y ajusta el modelo para no repetir ese tipo de recomendación en contextos similares |
| **Prioridad** | Alta |
| **Dependencias** | RF1 (Agente Conversacional), RF4 (Retroalimentación) |


# **5. RF15 — Gestión de Alertas (ALR)**

## **5.1 Historias de Usuario**

| **Título de la Historia de Usuario** | **Recibir alertas críticas sin saturación** |
| --- | --- |
| **Yo, como** | usuario de ROAX que tiene campañas activas mientras duerme o está fuera del computador |
| **Quiero** | recibir alertas inteligentes y priorizadas sobre situaciones críticas de mis campañas en tiempo real |
| **Para** | actuar rápido ante problemas sin ahogarme en notificaciones irrelevantes |
| **Criterios de Aceptación (Gherkin)** | |
| **Scenario 1** | Given el sistema detecta que una campaña gastó el 80% del presupuesto diario sin generar conversiones When evalúa el impacto económico Then envía una alerta crítica al usuario con la situación, el impacto estimado y las opciones de acción |
| **Scenario 2** | Given el usuario tiene múltiples campañas con indicadores fuera de rango simultáneamente When el sistema evalúa el conjunto Then agrupa las alertas por nivel de criticidad y presenta máximo 3 alertas críticas en la sesión |
| **Scenario 3** | Given el usuario quiere configurar sus preferencias When accede a la sección de notificaciones Then puede definir canales, horarios y nivel mínimo de criticidad para ser alertado |
| **Prioridad** | Alta |
| **Dependencias** | RF2 (Recomendaciones), RF1 (Agente) |


# **6. RF16 — Retroalimentación y Aprendizaje (RFA)**

## **6.1 Historias de Usuario**

| **Título de la Historia de Usuario** | **Construir confianza progresiva con el agente** |
| --- | --- |
| **Yo, como** | usuario de ROAX que ha comenzado a usar las recomendaciones del sistema |
| **Quiero** | ver cómo el sistema aprende de mis decisiones y mejora sus sugerencias con el tiempo, y poder delegar gradualmente más autonomía al agente |
| **Para** | confiar en el sistema lo suficiente para permitirle actuar automáticamente en mi nombre cuando esté fuera |
| **Criterios de Aceptación (Gherkin)** | |
| **Scenario 1** | Given el usuario aplicó 5 recomendaciones consecutivas con resultados positivos When el sistema calcula el nivel de confianza Then muestra al usuario un indicador de confianza acumulada y le sugiere activar el modo semi-automatizado |
| **Scenario 2** | Given el usuario rechaza repetidamente recomendaciones de un tipo específico When el modelo de aprendizaje procesa el patrón Then el sistema deja de generar ese tipo de recomendación y ajusta su estrategia |
| **Scenario 3** | Given el usuario activa el modo de automatización completa When el sistema ejecuta una acción automáticamente Then notifica al usuario qué acción tomó, por qué, y le ofrece la opción de revertirla en las próximas 24 horas |
| **Prioridad** | Alta |
| **Dependencias** | RF1, RF2, RF3 |



