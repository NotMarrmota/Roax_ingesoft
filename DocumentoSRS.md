# DOCUMENTO DE ESPECIFICACIÓN DE REQUERIMIENTOS

## ROAX

---

### Equipo Reto 1 — Datos y Decisiones

- Daniel Felipe Herrera Parra — A00413908
- Juan Rikardo Ramírez — A00414615
- Juan José González Chavez — A00415940
- Joshua Vera Hoyos — A00414279
- Juan Pablo Ceballos — A00415570
- Alejandro Sandoval — A00418631
- Juan Esteban Otero — A00414905

### Equipo Reto 2 — Alertas que Razonan

- David Altaminaro Altamirano
- Mariana Carmona Galvez
- Santiago Campo
- David Santiago García
- Mario Andrés Romero Rivera
- Andrés Vinasco

### Equipo Reto 3 — Creatividades desde el Rendimiento

- Maria Jose Sanchez
- Mariana Lucia Galeano
- Esteban Bernal
- Juan Jose Motato
- Samuel Palma
- Santiago Millan

### Equipo Reto 4 — Confianza Progresiva

- Melisa Gomez Gomez
- Samuel Alejandro Estupiñan Gonzales
- Jorge Humberto Garcia Leon
- Juan Camilo Borrero Florez
- Juan Pablo Urbina Ladino
- Matius Montealegre Padilla

---

# Tabla de Contenido

1. Especificación de Requerimientos
   - 1.1 Descripción General
   - 1.2 Contexto del Proyecto
   - 1.3 Requisitos
     - 1.3.1 Subsistema de Datos y Decisiones
     - 1.3.2 Subsistema de Alertas que Razonan
     - 1.3.3 Subsistema de Creatividades desde el Rendimiento
     - 1.3.4 Subsistema de Confianza Progresiva
   - 1.4 Subespecificación por Subsistemas
     - 1.4.1 RF1: Datos y Decisiones
     - 1.4.2 RF2: Alertas que Razonan
     - 1.4.3 RF3: Creatividades desde el Rendimiento
     - 1.4.4 RF4: Confianza Progresiva
   - 1.5 Tabla de Asignación a Subsistemas

2. PESTLE
   - 2.1 RF1: Datos y Decisiones
   - 2.2 RF2: Alertas que Razonan
   - 2.3 RF3: Creatividades desde el Rendimiento
   - 2.4 RF4: Confianza Progresiva

3. RF1: Datos y Decisiones
   - 3.1 Historias de Usuario
   - 3.2 Casos de Uso
     - 3.2.1 Diagramas de Casos de Uso
     - 3.2.2 Formatos Bicolumnares

4. RF2: Alertas que Razonan
   - 4.1 Historias de Usuario
   - 4.2 Casos de Uso
     - 4.2.1 Diagramas de Casos de Uso
     - 4.2.2 Formatos Bicolumnares

5. RF3: Creatividades desde el Rendimiento
   - 5.1 Historias de Usuario
   - 5.2 Casos de Uso
     - 5.2.1 Diagramas de Casos de Uso
     - 5.2.2 Formatos Bicolumnares

6. RF4: Confianza Progresiva
   - 6.1 Historias de Usuario
   - 6.2 Casos de Uso
     - 6.2.1 Diagramas de Casos de Uso
     - 6.2.2 Formatos Bicolumnares

7. Backlog

8. MockUp
   - 8.1 Descripción General
   - 8.2 Enlace MockUp

---

# 1. Especificación de Requerimientos

## 1.1 Descripción General

En esta sección se describen y analizan los requerimientos del proyecto ROAX Refactor 2026, una plataforma de inteligencia de negocio orientada a e-commerce que busca transformar la manera en que los usuarios interpretan, analizan y ejecutan decisiones relacionadas con sus campañas de marketing digital y desempeño comercial.

Actualmente, ROAX integra múltiples fuentes de datos provenientes de plataformas como Meta Ads, Shopify, Dropi y otros entornos de comercio electrónico, permitiendo visualizar métricas relacionadas con rentabilidad, conversión y rendimiento publicitario. Sin embargo, el sistema actual se centra principalmente en la visualización de información, dejando en manos del usuario la interpretación de los datos y la toma de decisiones estratégicas.

El objetivo de este proyecto es rediseñar la plataforma para convertir la inteligencia artificial en el núcleo operativo del sistema, permitiendo no solo visualizar datos, sino también analizar comportamientos, generar recomendaciones, contextualizar alertas, sugerir acciones concretas y fortalecer progresivamente la confianza del usuario en las decisiones automatizadas.

La solución propuesta se divide en cuatro subsistemas principales: Datos y Decisiones, Alertas que Razonan, Creatividades desde el Rendimiento y Confianza Progresiva. Cada uno de estos componentes busca abordar distintos retos relacionados con automatización, interpretación de datos, generación de recomendaciones y aprendizaje continuo del comportamiento del negocio.

El sistema está orientado a usuarios de e-commerce que requieren herramientas más inteligentes, proactivas y accionables para optimizar sus campañas publicitarias, mejorar su rentabilidad y facilitar la toma de decisiones basada en datos.

---

## 1.2 Contexto del Proyecto

ROAX es una plataforma de data e inteligencia de negocio enfocada en e-commerce que actualmente permite conectar información proveniente de campañas publicitarias y canales de venta digitales para calcular métricas de rendimiento y rentabilidad de un negocio.

La plataforma cuenta con integración de múltiples fuentes de datos, dashboards de métricas publicitarias, sistemas de alertas y herramientas de generación de anuncios mediante inteligencia artificial. Además, dispone de una base de usuarios reales que interactúan constantemente con el sistema y generan comportamientos medibles dentro de la plataforma.

A pesar de contar con una infraestructura sólida de visualización y análisis de datos, el sistema presenta una limitación importante: actualmente la plataforma informa qué está ocurriendo, pero no participa activamente en la toma de decisiones del usuario.

Los usuarios deben interpretar manualmente métricas como ROAS, CTR o CPA para determinar qué campañas están funcionando, cuáles están generando pérdidas y qué acciones deberían ejecutarse para mejorar el rendimiento del negocio. Esto genera dependencia del criterio humano, tiempos de análisis más largos y dificultad para reaccionar rápidamente ante cambios en el comportamiento de las campañas.

El proyecto ROAX Refactor 2026 surge como respuesta a esta necesidad, proponiendo una evolución de la plataforma hacia un sistema más inteligente, proactivo y automatizado, donde la inteligencia artificial no funcione como una característica adicional, sino como el motor principal de análisis, recomendación y aprendizaje continuo.

Para abordar este reto, el proyecto se enfoca en cuatro áreas fundamentales: la generación de decisiones basadas en datos, la construcción de alertas inteligentes capaces de contextualizar recomendaciones, el uso de inteligencia artificial aplicada a creatividades publicitarias y la construcción progresiva de confianza entre el usuario y las decisiones automatizadas del sistema.

Con este rediseño, ROAX busca evolucionar de una plataforma de visualización de datos hacia un ecosistema inteligente capaz de observar, interpretar, recomendar y aprender continuamente del comportamiento de cada negocio.

---

## 1.3 Requisitos

### 1.3.1 Subsistema de Datos y Decisiones

#### Requisitos de Usuario

**RU1 — Visibilidad de rentabilidad real**
El usuario necesita saber en tiempo real cuánto está ganando o perdiendo por cada campaña activa, cruzando automáticamente su inversión en publicidad con las ventas y entregas reales, sin tener que hacer los cálculos manualmente ni entrar a múltiples plataformas.

**RU2 — Alertas comprensibles**
El usuario necesita recibir alertas que no solo le avisen que algo está mal, sino que le expliquen en lenguaje sencillo por qué está pasando y qué parte del proceso está fallando, ya sea el anuncio, la página de venta o la logística.

**RU3 — Control sobre la automatización**
El usuario necesita poder definir sus propias reglas de automatización y aprobar las acciones que la IA propone antes de que se ejecuten, manteniendo siempre el control sobre su presupuesto y sus campañas si lo prefiere; sino, puede configurar las automatizaciones que no requieran su aprobación o considere oportunas.

**RU4 — Monitoreo sin intervención**
El usuario necesita que el sistema vigile sus campañas las 24 horas del día los 7 días de la semana, actuando de forma autónoma dentro de los límites que él mismo configuró, para evitar pérdidas mientras no está disponible.

**RU5 — Privacidad y acceso seguro**
El usuario necesita que los datos de sus clientes y pedidos estén protegidos, y que cada miembro de su equipo solo pueda ver la información que le corresponde según su rol.

**RU6 — Transparencia y acceso móvil**
El usuario necesita conocer cualquier costo adicional antes de aplicar cambios en su presupuesto, y poder gestionar todo desde su teléfono —ya sea en app, portal web o chatbot de WhatsApp— sin perder funcionalidades.

**RU7 — Decisiones con contexto real**
El usuario puede preferir que la IA tenga en cuenta factores reales de su negocio como el inventario disponible, sus restricciones financieras y el perfil de su cliente ideal, para que las recomendaciones sean útiles y no genéricas; o puede usar las recomendaciones de Meta Advantage.

#### Requisitos del Sistema

**RF1 — Rentabilidad real integrada**
El sistema debe calcular la rentabilidad real del negocio integrando fuentes de pauta y ventas.

- **RF1.1** El sistema debe cruzar automáticamente los datos de Meta Ads (Inversión, ROAS, CPA) con los de las plataformas de venta como Shopify o Dropi, para saber cuánto está ganando o perdiendo el negocio por cada campaña activa.
- **RF1.2** El sistema debe detectar de forma proactiva las campañas que no están siendo rentables, comparando el ROAS actual contra el punto de equilibrio real del producto.

**RF2 — IA explicativa**
El sistema debe explicar el porqué de cada métrica de rentabilidad.

- **RF2.1** Las alertas del sistema no deben limitarse a mostrar datos. Deben explicar qué está pasando y por qué — por ejemplo: "La campaña X está quemando dinero porque el CPA superó el margen de ganancia en un 15%".
- **RF2.2** El sistema aprenderá de las decisiones del usuario (aprobaciones, rechazos y modificaciones) para ajustar progresivamente su nivel de autonomía. El usuario puede configurar en cualquier momento qué tipo de acciones puede ejecutar la IA sin pedir permiso. El nivel de autonomía activado siempre es reversible.

**RF3 — Automatización y reglas**
El sistema debe ejecutar acciones correctivas de forma autónoma sobre la publicidad digital.

- **RF3.1** Cada usuario debe poder configurar sus propias reglas de automatización, como pausar campañas o ajustar presupuestos, basándose en la rentabilidad real del negocio y no solo en las métricas de pauta.
- **RF3.2** Cada acción automática debe quedar registrada con la fecha, lo que se hizo y la razón por la que se tomó esa decisión.

**RF4 — Monitor 24/7**
El sistema debe monitorear el negocio de forma autónoma las 24 horas, los 7 días de la semana.

- **RF4.1** El sistema debe revisar continuamente los datos de Meta Ads para detectar, incluso fuera del horario de trabajo del usuario, cuando el CPA o el ROAS estén fallando de forma crítica y poniendo en riesgo la rentabilidad. La evaluación debe considerar el tiempo de madurez de cada campaña y clasificar el rendimiento según la fase activa: Testeo, Optimización o Escalado.

**RF5 — Seguridad y privacidad**
El sistema debe proteger la integridad y privacidad de los datos del e-commerce.

- **RF5.1** El sistema debe cumplir con la Ley de Habeas Data y cifrar los datos de clientes y pedidos de Shopify o Dropi usando protocolos TLS 1.3.
- **RF5.2** El acceso a los datos financieros debe estar dividido por roles (Administrador y Vendedor) para que la información sensible solo la vea quien debe verla.

**RF6 — Transparencia de costos y movilidad**
El sistema debe ser transparente con los costos y funcionar bien en dispositivos móviles.

- **RF6.1** Antes de ejecutar cualquier cambio de presupuesto o activar una integración que pueda generar costos adicionales, el sistema debe informar al usuario sobre el monto estimado, la frecuencia y el servicio involucrado. Esto aplica tanto desde la plataforma web como desde el chatbot de WhatsApp, y el sistema siempre debe esperar confirmación explícita antes de proceder.
- **RF6.2** El sistema debe funcionar correctamente en navegadores móviles de Android e iOS, ya que la mayoría de los dropshippers manejan su negocio desde el celular.

**RF7 — Contexto operativo real**
El sistema debe tomar decisiones considerando el contexto operativo real del negocio, más allá de los datos de las APIs de publicidad, integrando el inventario, las restricciones financieras y el perfil cualitativo del cliente ideal.

- **RF7.1** El sistema debe sincronizarse de forma automática con el inventario real de cada producto (Shopify, Dropi, WooCommerce, Tienda Nube). Cuando un producto se quede sin stock o caiga por debajo del umbral mínimo definido, el sistema debe pausar automáticamente las campañas asociadas y reactivarlas cuando el inventario sea repuesto.
- **RF7.2** El sistema debe identificar campañas ganadoras y sugerir proactivamente un aumento de presupuesto cuando haya margen financiero disponible. La sugerencia debe incluir el monto recomendado, la proyección de gasto en las próximas 24 horas y el resultado esperado, antes de que el usuario confirme.
- **RF7.3** El sistema debe conectarse con la API de Meta Advantage para analizar la configuración de los públicos en las campañas activas, detectar errores o inconsistencias en la segmentación actual y sugerir ajustes concretos. El usuario siempre puede aceptar, modificar o descartar cada sugerencia. El sistema no aplica cambios de segmentación de forma automática.
- **RF7.4** El sistema debe integrar fuentes de datos externos del mercado (tendencias estacionales, picos de demanda en Google Trends, comportamiento publicitario de la competencia accesible vía APIs públicas de Meta) para que sus recomendaciones de pauta consideren el contexto externo.

#### Requisitos de Proceso

**RP1** El desarrollo del módulo se llevará a cabo bajo metodología Scrum, con sprints de 2 semanas y reuniones de revisión al final de cada sprint con el Product Owner de ROAX.

**RP2** El código fuente del sistema debe gestionarse mediante control de versiones usando Git, con ramas separadas para desarrollo, pruebas y producción.

**RP3** Toda integración con APIs externas (Meta Ads, Shopify, Dropi) debe realizarse respetando los permisos y condiciones de uso vigentes de cada plataforma.

**RP4** El sistema debe ser diseñado para operar sobre la infraestructura existente de ROAX en `app.roaxai.com` sin requerir cambios en la arquitectura base de la plataforma externa.

---

### 1.3.2 Subsistema de Alertas que Razonan

**RF1** El sistema debe generar alertas predictivas y diagnósticos contextuales mediante IA.

**RF2** El sistema debe emitir recomendaciones inteligentes basadas en el rendimiento del negocio.

**RF3** El sistema debe permitir la automatización y toma de decisiones autónomas delegadas.

**RF4** El sistema debe construir confianza progresiva y aprender del impacto de las recomendaciones.

---

### 1.3.3 Subsistema de Creatividades desde el Rendimiento

| RF | Requerimiento de alto nivel |
| --- | --- |
| RF1 | El sistema debe capturar la información básica del usuario. |
| RF1.1 | El sistema debe permitir la identificación única de cada cliente. |
| RF1.1.1 | El sistema debe clasificar a los usuarios según su perfil dentro de la organización. |
| RF2 | El sistema debe gestionar el perfil detallado del cliente. |
| RF2.1 | El sistema debe centralizar la información detallada del consumidor. |
| RF2.1.1 | El sistema debe consolidar datos demográficos, históricos y preferencias en un solo perfil. |
| RF3 | El sistema debe generar reportes de estado de negocio. |
| RF3.1 | El sistema debe emitir informes sobre situación financiera y operativa. |
| RF3.1.1 | El sistema debe integrar indicadores de deuda, impuestos y costos fijos en el balance general. |
| RF3.1.2 | El sistema debe notificar el estado del inventario y flujo de procesos actuales. |
| RF4 | El sistema debe gestionar estrategias de marketing basadas en datos. |
| RF4.1 | El sistema debe analizar el rendimiento de campañas publicitarias. |
| RF4.1.1 | El sistema debe generar propuestas de mejora basadas en comparación de resultados históricos. |

---

### 1.3.4 Subsistema de Confianza Progresiva

#### Requerimientos Funcionales

| RF | Descripción |
| --- | --- |
| **RF13** | El sistema debe permitir la comunicación con el usuario mediante un agente conversacional visual en tiempo real. |
| **RF14** | El sistema debe generar y presentar recomendaciones inteligentes sobre campañas publicitarias basadas en análisis de datos y comportamiento histórico. |
| **RF15** | El sistema debe gestionar alertas priorizadas sobre indicadores críticos del negocio evitando la saturación de información al usuario. |
| **RF16** | El sistema debe gestionar la retroalimentación del usuario y ajustar progresivamente sus recomendaciones para construir confianza progresiva. |

#### Requerimientos No Funcionales

| RNF | Descripción |
| --- | --- |
| **RNF1** | **Disponibilidad:** el sistema debe estar disponible 24/7 para monitoreo continuo de campañas. |
| **RNF2** | **Procesamiento en tiempo real:** el sistema debe procesar y analizar datos con mínima latencia. |
| **RNF3** | **Interfaz de usuario:** el sistema debe ofrecer una interfaz intuitiva, clara y orientada a la toma de decisiones. |
| **RNF4** | **Portabilidad:** el sistema debe ser accesible desde múltiples dispositivos incluyendo móviles. |
| **RNF5** | **Interacción por voz:** el sistema debe permitir interacción mediante audio procesando comandos en tiempo real. |
| **RNF6** | **Transparencia IA:** el sistema debe hacer visible cuando una recomendación es generada por inteligencia artificial. |
| **RNF7** | **Escalabilidad:** el sistema debe gestionar el consumo de recursos según el plan de suscripción del usuario. |

---

## 1.4 Subespecificación por Subsistemas

### 1.4.1 RF1: Datos y Decisiones

**SS1 — Motor de Rentabilidad**

- **RF1.1** El sistema debe cruzar automáticamente los datos de Meta Ads (Inversión, ROAS, CPA) con los de las plataformas de venta como Shopify o Dropi, para saber cuánto está ganando o perdiendo el negocio por cada campaña activa.
- **RF1.2** El sistema debe detectar de forma proactiva las campañas que no están siendo rentables, comparando el ROAS actual contra el punto de equilibrio real del producto.

**SS2 — Motor de IA Explicativa**

- **RF2.1** Las alertas del sistema no deben limitarse a mostrar datos. Deben explicar qué está pasando y por qué — por ejemplo: "La campaña X está quemando dinero porque el CPA superó el margen de ganancia en un 15%".
- **RF2.2** El sistema aprenderá de las decisiones del usuario (aprobaciones, rechazos, modificaciones) antes de ejecutar cualquier acción automática y ajustará progresivamente el nivel de autonomía de la IA, permitiendo que el usuario lo revise y modifique en cualquier momento.

**SS3 — Motor de Automatización y Reglas**

- **RF3.1** Cada usuario debe poder configurar sus propias reglas de automatización, como pausar campañas o ajustar presupuestos, basándose en la rentabilidad real del negocio y no solo en las métricas de pauta.
- **RF3.2** Cada acción automática debe quedar registrada con la fecha, lo que se hizo y la razón por la que se tomó esa decisión. El usuario siempre debe poder saber qué hizo el sistema y por qué.

**SS4 — Monitor 24/7 y Detección de Anomalías**

- **RF4.1** El sistema debe revisar continuamente los datos de Meta Ads para detectar, incluso fuera del horario de trabajo del usuario, cuando el CPA o el ROAS estén fallando de forma crítica. Para hacer esta evaluación correctamente, el sistema debe reconocer el tiempo de madurez de la campaña y el delay de 24 horas propio de Meta Ads, usando indicadores diferenciados según la fase activa: Hook rate, Retention rate, Click rate y Tasas de retención en Testeo; Tasas de conversión en Optimización; y CPA y ROAS neto en Escalado.

**SS5 — Seguridad, Privacidad y Control de Acceso**

- **RF5.1** El sistema debe cumplir con la Ley de Habeas Data y cifrar los datos de clientes y pedidos de Shopify o Dropi usando protocolos TLS 1.3. Proteger la información de los compradores no es opcional.
- **RF5.2** El acceso a los datos financieros debe estar dividido por roles (Administrador y Vendedor) para que la información privada solo la vea quien debe verla.

**SS6 — Interfaz Conversacional y Movilidad**

- **RF6.1** Transparencia de costos antes de ejecutar cambios (web y WhatsApp).
- **RF6.2** Conversación con bot inteligente vía WhatsApp.

**SS7 — Integraciones y Contexto Operativo**

- **RF7.1** Sincronización automática con inventario.
- **RF7.2** Restricciones financieras y sugerencia de escalar en campañas ganadoras.
- **RF7.3** API Meta Advantage — segmentación y auditoría de públicos.
- **RF7.4** Fuentes externas del mercado (Google Trends, competencia).

---

### 1.4.2 RF2: Alertas que Razonan

**RF1** El sistema debe generar alertas predictivas y diagnósticos contextuales mediante IA.

- **RF1.1** El sistema debe analizar de forma continua las desviaciones de métricas clave (como caídas de ROAS o incrementos de CPA) cruzando datos de pauta digital (Meta Ads) con datos de ventas reales (Shopify, Dropi).
- **RF1.2** El sistema debe procesar las anomalías detectadas a través de un Modelo de Lenguaje (LLM) para redactar un diagnóstico automatizado en lenguaje natural.
- **RF1.3** El sistema debe estructurar el diagnóstico indicando de forma explícita la causa raíz de la alerta (por ejemplo: identificar qué campaña específica está perdiendo rentabilidad y los motivos asociados).

**RF2** El sistema debe emitir recomendaciones inteligentes basadas en el rendimiento del negocio.

- **RF2.1** El sistema debe sugerir de forma proactiva ajustes específicos en los presupuestos diarios o el estado (pausar/activar) de las campañas publicitarias analizando la rentabilidad real en e-commerce.
- **RF2.2** El sistema debe proponer la sustitución de piezas gráficas o videos de bajo rendimiento por creativos nuevos generados con la inteligencia artificial de ROAX Ads, priorizando aquellos con mayor probabilidad de conversión según los datos históricos de la marca.
- **RF2.3** La interfaz de la alerta debe incluir componentes interactivos (botones de acción directa) que permitan al usuario aplicar e implementar las mejoras sugeridas al instante.

**RF3** El sistema debe permitir la automatización y toma de decisiones autónomas delegadas.

- **RF3.1** El sistema debe proveer un panel de configuración para que el usuario defina y delimite las reglas bajo las cuales la IA puede tomar decisiones autónomas (por ejemplo: umbrales críticos de ROAS o límites de presupuesto permitidos).
- **RF3.2** El sistema debe conectarse y ejecutar los cambios aprobados automáticamente en las plataformas de publicidad externas (Meta Ads API) sin requerir intervención humana una vez se cumplan los criterios de automatización.
- **RF3.3** El sistema debe despachar una notificación de confirmación inmediata al usuario cada vez que la IA realice una acción autónoma en sus cuentas asociadas.

**RF4** El sistema debe construir confianza progresiva y aprender del impacto de las recomendaciones.

- **RF4.1** El sistema debe registrar minuciosamente cada interacción del usuario con las alertas (si la recomendación fue aceptada, rechazada o ignorada) junto con la marca de tiempo para modelar perfiles de adopción.
- **RF4.2** El sistema debe evaluar de forma continua el impacto post-ejecución, comparando las métricas del negocio antes y después de aplicar la recomendación, cerrando el ciclo de confianza con evidencia del resultado.
- **RF4.3** El sistema debe retroalimentar el motor de IA con los resultados históricos medidos para ajustar, optimizar y refinar la precisión de las futuras recomendaciones de la marca con el tiempo.

---

### 1.4.3 RF3: Creatividades desde el Rendimiento

**Subsistema A — Gestión de Usuarios**

| Código | Subrequerimiento |
| --- | --- |
| USU_RF1.1 | Registrar usuarios con identificador único, correo y contraseña. |
| USU_RF1.1.1 | Asignar roles organizacionales a usuarios. |
| USU_RF1.1.2 | Permitir inicio de sesión seguro. |
| USU_RF1.1.3 | Permitir recuperación de contraseña mediante correo. |

**Subsistema B — Perfilamiento del Cliente**

| Código | Subrequerimiento |
| --- | --- |
| PER_RF2.1 | Centralizar información del consumidor desde múltiples fuentes. |
| PER_RF2.1.1 | Consolidar datos históricos y demográficos en un perfil único. |
| PER_RF2.1.2 | Consultar perfil 360° por ID o correo. |
| PER_RF2.1.3 | Guardar trazabilidad de la fuente de cada dato. |
| PER_RF2.1.4 | Fusionar registros duplicados automáticamente. |
| PER_RF2.1.5 | Registrar consentimiento para tratamiento de datos. |

**Subsistema C — Reportes de Inteligencia de Negocio**

| Código | Subrequerimiento |
| --- | --- |
| REP_RF3.1 | Generar reportes financieros y operativos. |
| REP_RF3.1.1 | Integrar costos fijos, impuestos y deudas. |
| REP_RF3.1.2 | Integrar métricas de inventario y flujo de productos. |
| REP_RF3.1.3 | Exportar reportes en PDF y Excel. |
| REP_RF3.1.4 | Generar reportes periódicos automáticos. |

**Subsistema D — Optimización de Campañas con IA**

| Código | Subrequerimiento |
| --- | --- |
| OPT_RF4.1 | Analizar el rendimiento de campañas activas. |
| OPT_RF4.1.1 | Asociar creatividades con métricas reales de conversión. |
| OPT_RF4.1.2 | Clasificar creatividades por estilo, copy y formato. |
| OPT_RF4.1.3 | Identificar patrones comunes en creatividades exitosas. |
| OPT_RF4.1.4 | Generar propuestas automáticas de mejora para nuevas creatividades. |
| OPT_RF4.1.5 | Predecir rendimiento esperado antes de lanzar una creatividad. |

**Subsistema E — Integración de APIs Externas**

| Código | Subrequerimiento |
| --- | --- |
| API_INT1 | Integrarse con Meta Ads API. |
| API_INT2 | Integrarse con Shopify API. |
| API_INT3 | Integrarse con Dropi API. |
| API_INT4 | Integrarse con TikTok Ads API. |
| API_INT5 | Implementar OAuth 2.0 y manejo de rate limits. |

---

### 1.4.4 RF4: Confianza Progresiva

**RF13 — Agente Conversacional Visual (ACV)**

| ID | Subrequerimiento |
| --- | --- |
| ACV R13.1 | El sistema debe mostrar el avatar visual del agente mediante una ventana fija en la interfaz principal de la plataforma. |
| ACV R13.2 | El sistema debe reproducir la voz del agente mediante síntesis de voz clonada de actriz al momento de emitir una recomendación o alerta. |
| ACV R13.3 | El sistema debe mostrar el texto de la respuesta en un panel de conversación junto al avatar para usuarios que prefieran leer. |
| ACV R13.4 | El sistema debe permitir al usuario enviar mensajes al agente mediante un campo de texto o por entrada de voz. |
| ACV R13.5 | El sistema debe responder al usuario en lenguaje natural evitando tecnicismos innecesarios mediante el procesamiento del LLM. |
| ACV R13.6 | El sistema debe permitir al usuario activar o desactivar la voz del agente mediante un botón de configuración en la interfaz. |

**RF14 — Recomendaciones Inteligentes (REC)**

| ID | Subrequerimiento |
| --- | --- |
| REC R14.1 | El sistema debe identificar automáticamente campañas con bajo rendimiento mediante el análisis de métricas como ROAS, CPA, CTR y comportamiento histórico. |
| REC R14.2 | El sistema debe presentar cada recomendación en una tarjeta de acción que incluya la acción sugerida, la explicación basada en datos y la estimación de impacto esperado. |
| REC R14.3 | El sistema debe permitir al usuario interactuar con cada recomendación mediante tres opciones: Aplicar, Rechazar o Posponer, mostradas como botones diferenciados en la interfaz. |
| REC R14.4 | El sistema debe permitir al usuario expandir cada recomendación para acceder a una vista detallada con gráficas de evolución temporal y análisis del embudo de conversión. |
| REC R14.5 | El sistema debe solicitar y almacenar información cualitativa del negocio (inventario disponible, costos fijos, perfil del cliente) mediante un formulario de onboarding para mejorar la precisión de las recomendaciones. |
| REC R14.6 | El sistema debe mostrar, posterior a la aplicación de una recomendación, un seguimiento del impacto real versus el impacto estimado en formato antes/después con métricas en valores monetarios y porcentajes. |

**RF15 — Gestión de Alertas (ALR)**

| ID | Subrequerimiento |
| --- | --- |
| ALR R15.1 | El sistema debe enviar notificaciones inmediatas al usuario cuando detecte una campaña en situación crítica, priorizando aquellas con mayor impacto económico potencial. |
| ALR R15.2 | El sistema debe agrupar y priorizar las alertas según su impacto potencial mediante un sistema de pesos por indicador, mostrando un máximo de alertas críticas por sesión. |
| ALR R15.3 | El sistema debe analizar indicadores en conjunto (CTR + CPA + CBR) en lugar de dispararlos individualmente, para evitar la saturación de alertas al usuario. |
| ALR R15.4 | El sistema debe permitir al usuario configurar sus preferencias de notificación incluyendo canales (in-app, correo, WhatsApp, push móvil), horarios de envío y nivel de criticidad mínimo. |

**RF16 — Retroalimentación y Aprendizaje (RFA)**

| ID | Subrequerimiento |
| --- | --- |
| RFA R16.1 | El sistema debe presentar al usuario un mecanismo de retroalimentación explícita que le permita calificar la utilidad de cada recomendación (útil, incorrecta, irrelevante) con comentario opcional. |
| RFA R16.2 | El sistema debe registrar retroalimentación implícita derivada del comportamiento del usuario: frecuencia de aceptación, tiempo antes de actuar, recomendaciones ignoradas y acciones revertidas. |
| RFA R16.3 | El sistema debe continuar generando recomendaciones aunque el usuario las rechace de forma repetida, ajustando el tipo y enfoque de las sugerencias según el patrón detectado. |
| RFA R16.4 | El sistema debe permitir al usuario configurar niveles de automatización desde recomendaciones manuales hasta ejecución automática de acciones según su preferencia y nivel de confianza acumulada. |
| RFA R16.5 | El sistema debe mostrar al usuario un indicador de nivel de confianza acumulada con el agente de IA, reflejando el historial de recomendaciones aceptadas y sus resultados medibles. |

---

## 1.5 Tabla de Asignación a Subsistemas

### RF1 y RF2

| Requerimiento | Motor de Datos y Análisis | Motor de Alertas Inteligentes | Motor de Creatividades | Motor de Confianza y Aprendizaje | Integraciones y APIs | Sistema Conversacional | Monitor de Rendimiento y Riesgos |
| --- | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| RF1 | X | | | | X | | |
| RF1.1 | X | | | | X | | |
| RF1.1.1 | X | | | | X | | |
| RF1.1.2 | X | | | | X | | |
| RF1.1.3 | X | | | | X | | |
| RF1.2 | X | X | | | X | | X |
| RF1.2.1 | X | X | | | X | | X |
| RF1.2.2 | X | X | | | X | | X |
| RF1.3 | X | | | X | X | | |
| RF1.3.1 | X | | | X | X | | |
| RF1.4 | X | X | | | X | | X |
| RF1.4.1 | X | X | | | X | | X |
| RF1.4.2 | X | X | | | X | | X |
| RF2.1 | X | X | | | X | | X |
| RF2.1.1 | X | X | | | | | X |
| RF2.1.2 | X | X | | | | | |
| RF2.1.3 | X | X | | | | | |
| RF2.2 | | X | X | | X | | |
| RF2.2.1 | X | X | | | X | | |
| RF2.2.2 | | X | X | | X | | |
| RF2.2.3 | | X | | X | X | | |
| RF2.3 | X | X | | X | X | | X |
| RF2.3.1 | X | X | | X | | | |
| RF2.3.2 | X | X | | X | | | X |
| RF2.3.3 | X | | | X | | | |
| RF2.3.4 | X | X | | | X | | X |
| RF2.3.5 | X | X | | | X | | X |
| RF2.3.6 | X | X | | | X | | |
| RF2.3.7 | X | X | | | X | | X |
| RF2.3.8 | X | X | | | X | | X |
| RF2.3.9 | X | X | | | X | | X |
| RF2.3.10 | X | X | | | X | | X |
| RF2.3.11 | X | X | | X | | | |
| RF2.3.12 | X | X | | X | | X | |
| RF2.3.13 | X | X | | X | | | |
| RF2.3.14 | X | X | | X | X | | X |
| RF2.3.15 | X | | | X | | | |

### RF3 y RF4

| Requerimiento | Motor de Datos y Análisis | Motor de Alertas Inteligentes | Motor de Creatividades | Motor de Confianza y Aprendizaje | Integraciones y APIs | Sistema Conversacional | Monitor de Rendimiento y Riesgos |
| --- | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| RF3 | | | X | | X | X | |
| RF3.1 | | | X | | X | X | |
| RF3.1.1 | | | X | | X | X | |
| RF3.1.2 | | X | X | | X | X | |
| RF3.1.3 | | | X | | X | X | |
| RF3.2 | | X | X | | X | X | |
| RF3.2.1 | | X | X | | X | X | |
| RF3.2.2 | | X | X | | X | X | |
| RF3.2.3 | | X | X | | X | X | |
| RF3.3 | | | X | | X | X | |
| RF3.3.1 | | | X | | X | X | |
| RF4.1 | | X | | X | | | |
| RF4.1.1 | | X | | X | | | |
| RF4.1.2 | X | X | | X | | | |
| RF4.2 | | X | | X | | | X |
| RF4.2.1 | | X | | X | | | X |
| RF4.2.2 | X | X | | X | | | |
| RF4.3 | | | | X | | X | |
| RF4.3.1 | | | | X | | X | |
| RF4.3.2 | X | | | X | | | |
| RF4.4 | | X | | X | | | |
| RF4.4.1 | X | X | | X | | | |
| RF4.4.2 | | X | | X | | | |
| RF4.5 | | | | X | | X | |
| RF4.5.1 | | | | X | | X | |
| RF4.5.2 | X | | | X | | | |

---

# 2. PESTLE

> El análisis PESTLE se aplica a los requerimientos funcionales que toman decisiones sobre personas, usan datos sensibles o pueden generar impacto negativo. Para cada dimensión se identifica el hallazgo verificado, su impacto real y el requerimiento derivado.

---

## 2.1 RF1: Datos y Decisiones

| Dimensión | Hallazgo | Impacto | Requerimiento derivado |
| --- | --- | --- | --- |
| **P — Político** | La autonomía configurable de la IA y la posibilidad de delegar decisiones según el historial de confianza están en una zona gris legal en Colombia. No queda claro quién responde si algo sale mal. | Si la IA ejecuta una acción financiera sin que el usuario la haya aprobado manualmente, hay que definir de antemano quién asume la responsabilidad. | **RNFP-7-01:** Antes de activar el "Modo Autónomo", el sistema debe mostrar una cláusula de aceptación de riesgos vinculada al historial de confianza del usuario. **RNFP-7-02:** Cuando el sistema sugiera un cambio de segmentación vía Meta Advantage, debe advertir que la decisión y sus consecuencias son responsabilidad del usuario, y registrar su aceptación explícita antes de aplicar cualquier cambio. |
| **E — Económico** | Las sugerencias de escalado de presupuesto en campañas ganadoras, combinadas con el delay de 24 h de Meta, pueden afectar el flujo de caja antes de ver si el dinero valió la pena. | Escalar sin considerar el delay puede generar sobrecostos antes de ver resultados. | **RNFE-7-02:** Antes de sugerir escalar el presupuesto de una campaña en etapa de "madurez temprana", el sistema debe proyectar cuánto se va a gastar en las próximas 24 horas. **RNFE-7-03:** Antes de sugerir un ajuste de segmentación vía Meta Advantage, el sistema debe estimar el impacto en alcance y CPM proyectado. **RNFE-7-04:** Cuando una recomendación se base en tendencias externas, el sistema debe aclarar que es contextual y no garantiza conversiones. |
| **S — Social** | Pasar de tableros visuales a un chatbot por WhatsApp cambia radicalmente cómo el usuario consume los datos de su negocio. Con respuestas puntuales por chat es fácil perder la visión completa del negocio. | Ver una métrica suelta no es lo mismo que ver cómo se comporta frente al mes anterior. | **RNFS-7-03:** El chatbot debe permitir que el usuario solicite resúmenes ejecutivos en PDF o imagen, para que pueda revisar métricas de forma visual fuera del hilo de conversación. |
| **T — Tecnológico** | El sistema depende de tres APIs externas críticas: WhatsApp Business, Meta Ads y Meta Advantage, además de Google Trends y APIs públicas de Meta, todas fuera del control del proyecto. | Si Meta cambia permisos o WhatsApp Business se cae, el usuario queda sin gestión operativa móvil y sin sugerencias de audiencia. | **RNFT-7-04:** El sistema debe tener un mecanismo de "Heartbeat" que avise al usuario por SMS o correo cuando falle cualquiera de estas conexiones: WhatsApp Business API, Meta Ads API, Meta Advantage Segmentation API o las fuentes de datos externos. |
| **L — Legal** | Manejar datos de ventas por WhatsApp, acceder a audiencias de Meta Advantage y almacenar información financiera del negocio genera obligaciones adicionales bajo la Ley 1581. | Datos de clientes en chat, datos de comportamiento de audiencias y datos financieros requieren consentimiento explícito, cifrado y acceso restringido. | **RNFL-7-05:** Cualquier mensaje del chatbot que contenga datos sensibles de clientes debe ir precedido de una confirmación de identidad del usuario. **RNFL-7-06:** Antes de activar la integración con Meta Advantage, el sistema debe informar al usuario que se accederá a datos de audiencias bajo las políticas de Meta y la Ley 1581, y registrar su aceptación. **RNFL-7-07:** Los datos financieros registrados deben tratarse con cifrado TLS 1.3 y acceso restringido al rol Administrador. |
| **É — Ético** | La IA aprende los hábitos del usuario y puede reforzarlos aunque no sean los mejores. Además, las sugerencias de segmentación pueden introducir sesgos en la audiencia publicitaria. | Una IA que valida hábitos malos, sugiere públicos sesgados o empuja a gastar más sin verificar la salud financiera real del negocio termina siendo un problema. | **RNFE-7-06:** Cuando las automatizaciones basadas en hábitos del usuario vayan en contra de los KPIs de rentabilidad neta, el sistema debe emitir una "Alerta de Salud de Negocio". **RNFE-7-07:** El sistema debe auditar periódicamente los públicos sugeridos para detectar si las recomendaciones excluyen sistemáticamente grupos demográficos sin justificación de rendimiento. **RNFE-7-08:** Cuando sugiera escalar el presupuesto de una campaña ganadora, el sistema debe verificar primero que las métricas de rentabilidad neta soporten ese crecimiento. |

---

## 2.2 RF2: Alertas que Razonan

### PESTLE — RF1: Alertas predictivas y diagnósticos contextuales mediante IA

| Dimensión | Hallazgo | Impacto | Requerimiento derivado |
| --- | --- | --- | --- |
| P — Político | No existen lineamientos específicos en Colombia sobre transparencia en algoritmos que evalúan desempeño de campañas. | El sistema podría ser cuestionado si no justifica cómo clasifica una campaña como de bajo desempeño. | **RNFP-1-01:** El sistema debe permitir consultar las métricas, umbrales y reglas utilizadas para clasificar una campaña como de bajo desempeño, mostrando al menos: nombre de la métrica, valor calculado, umbral aplicado y resultado de la evaluación. |
| E — Económico | El cálculo frecuente de métricas sobre grandes volúmenes de campañas implica alto costo computacional. | Puede afectar la escalabilidad y costos operativos del sistema. | **RNFE-1-02:** El sistema debe calcular métricas de desempeño mediante procesamiento incremental o por lotes, reduciendo en al menos un 30% el tiempo de procesamiento respecto a un cálculo completo sobre todos los datos históricos. |
| S — Social | Usuarios no expertos pueden no comprender métricas como CTR, ROI o tasa de conversión. | Riesgo de mala interpretación del desempeño de campañas. | **RNFS-1-03:** El sistema debe mostrar una descripción textual comprensible (máximo 100 palabras) para cada métrica utilizada, accesible desde la interfaz de evaluación de campañas. |
| T — Tecnológico | La evaluación depende de la actualización oportuna de datos de campañas. | Datos desactualizados generan clasificaciones incorrectas. | **RNFT-1-04:** El sistema debe actualizar las métricas de desempeño de campañas con una latencia máxima de 5 minutos desde la recepción de nuevos datos, garantizando que al menos el 95% de las actualizaciones cumplan este límite. |
| L — Legal | El sistema maneja datos sensibles de negocio asociados a campañas. | Riesgo de incumplimiento de normativas de protección de datos. | **RNFL-1-05:** El sistema debe restringir el acceso a la información de desempeño de campañas mediante control de roles, garantizando que solo usuarios autorizados puedan visualizar o modificar dichos datos. |
| É — Ético | La clasificación automática influye en decisiones comerciales del usuario. | Clasificaciones poco transparentes pueden inducir decisiones erróneas. | **RNFEt-1-06:** El sistema debe indicar explícitamente si la clasificación de bajo desempeño fue generada por reglas del sistema o configuraciones del usuario. |

### PESTLE — RF2: Recomendaciones inteligentes basadas en el rendimiento del negocio

| Dimensión | Hallazgo | Impacto | Requerimiento derivado |
| --- | --- | --- | --- |
| **P — Político** | Las plataformas como Meta y TikTok pueden cambiar sus reglas sobre cómo se permite ajustar presupuestos o publicar anuncios automáticamente. | Si Meta decide restringir la automatización, ROAX perdería la capacidad de aplicar cambios instantáneos (RF2.3), y el usuario tendría que volver a hacer todo manualmente. | El sistema debe anticipar estos cambios mostrando una alerta al usuario del tipo "Meta cambió sus reglas, por ahora solo podemos sugerir, no aplicar automáticamente". |
| **E — Económico** | Analizar si cada campaña está quemando dinero o generando ventas reales (RF2.1) requiere procesar muchos datos históricos. | La plataforma sería cara de mantener y el precio para el usuario final tendría que aumentar. | El sistema debe priorizar el análisis solo en campañas que más invierten y ajustar cada 4 horas, no en tiempo real, para reducir costo sin perder efectividad. |
| **S — Social** | Muchos usuarios de ROAX son dropshippers o pequeños empresarios, no expertos en marketing. Si ven una recomendación de "cambiar inversión" sin entender el porqué, pueden ignorarla o aplicarla mal. | El usuario termina tomando malas decisiones o no usa la función por miedo. | El sistema debe explicar cada recomendación en una frase simple, como: "Esta campaña gastó 100.000 $ y solo vendió 30.000 $. Te sugiero bajar la inversión a 50.000 $ diarios". |
| **T — Tecnológico** | ROAX ya genera anuncios con IA, pero conectarlos con datos reales de venta para que aprenda de lo que ya convierte (RF2.2) es complejo. | Si la IA propone creatividades bonitas pero que no venden, el usuario pierde confianza rápidamente y deja de usar la función. | El sistema debe etiquetar cada creatividad generada con una predicción simple: "Alta probabilidad de venta", "Media", "Baja", basada en anuncios anteriores que sí funcionaron. |
| **L — Legal** | El sistema puede llegar a pausar campañas o redistribuir presupuesto automáticamente (RF2.3) basado en rentabilidad. Si lo hace mal, el usuario pierde ventas reales. | ROAX podría ser demandado o perder muchos usuarios por mala publicidad. | La plataforma debe pedir un consentimiento explícito al inicio: "Autorizo a ROAX a hacer cambios automáticos hasta por un límite de $X diarios". Además, cada acción debe poder deshacerse con un botón "Reversar cambio". |
| **É — Ético** | El sistema decide que algunas recomendaciones "no están funcionando" (RF2.2) basándose en ventas pasadas. Eso puede dejar fuera a nuevos diseños que con más tiempo sí funcionarían. | El usuario puede terminar viendo siempre el mismo tipo de anuncio, saturando a su audiencia y sin explorar nuevas ideas. | El sistema debe reservar un pequeño porcentaje del presupuesto para probar creatividades nuevas sin que la IA las descarte de entrada. |

### PESTLE — RF3: Automatización y toma de decisiones autónomas delegadas

| Dimensión | Hallazgo | Impacto | Requerimiento derivado |
| --- | --- | --- | --- |
| **P — Político** | Las plataformas publicitarias (Meta Ads, TikTok Ads, Google Ads) pueden cambiar políticas o restricciones sobre acceso y uso de datos analíticos. | Cambios externos podrían afectar la continuidad del análisis y aprendizaje del sistema. | **RNFP-3-01:** El sistema debe registrar y notificar cambios en la disponibilidad de datos provenientes de plataformas publicitarias integradas, indicando el servicio afectado y el impacto sobre los análisis generados. |
| **E — Económico** | El procesamiento continuo de métricas históricas implica alto consumo computacional y almacenamiento. | Incremento de costos operativos y riesgo de baja escalabilidad. | **RNFE-3-02:** El sistema debe optimizar el almacenamiento y procesamiento histórico utilizando consolidación incremental de datos diarios y mensuales, reduciendo en al menos un 25% el consumo de recursos. |
| **S — Social** | Usuarios con distintos niveles de experiencia pueden interpretar incorrectamente métricas complejas como ROAS, conversion rate o calidad de tráfico. | Riesgo de tomar decisiones comerciales equivocadas. | **RNFS-3-03:** El sistema debe proporcionar explicaciones contextuales y descripciones comprensibles para cada métrica y recomendación mostrada, utilizando textos de máximo 120 palabras. |
| **T — Tecnológico** | El sistema depende de integración constante con múltiples plataformas externas (Shopify, WooCommerce, Meta Ads, TikTok Ads, etc.). | Fallas de sincronización pueden generar análisis incorrectos o incompletos. | **RNFT-3-04:** El sistema debe sincronizar datos provenientes de plataformas integradas con una disponibilidad mínima del 99% mensual y una latencia máxima de 10 minutos para actualizaciones críticas. |
| **L — Legal** | El sistema maneja información sensible relacionada con ventas, comportamiento de usuarios y datos comerciales. | Riesgo de incumplimiento de normativas de protección de datos y privacidad. | **RNFL-3-05:** El sistema debe proteger la información histórica y analítica mediante autenticación, control de acceso basado en roles y cifrado de datos sensibles almacenados y transmitidos. |
| **É — Ético** | Las recomendaciones inteligentes y decisiones automatizadas pueden influir directamente en inversiones publicitarias y estrategias de negocio. | Recomendaciones poco transparentes o sesgadas podrían afectar negativamente a los usuarios. | **RNFEt-3-06:** El sistema debe mostrar la justificación de cada recomendación o decisión automatizada indicando las métricas, tendencias históricas y reglas utilizadas para generarla. |

### PESTLE — RF4: Confianza progresiva y aprendizaje del impacto de las recomendaciones

| Dimensión | Hallazgo | Impacto | Requerimiento derivado |
| --- | --- | --- | --- |
| **P — Político** | No existen lineamientos específicos en Colombia sobre el nivel de autonomía que puede tener un sistema de IA para tomar decisiones sobre campañas publicitarias sin aprobación del usuario. | Si la IA ejecuta acciones sin supervisión explícita, el sistema puede generar conflictos de responsabilidad legal. | El sistema debe mantener logs auditables de cada interacción con las recomendaciones, indicando claramente qué decisiones tomó el usuario y cuáles ejecutó la IA de forma autónoma. |
| **E — Económico** | El ciclo de medición de impacto post-ejecución requiere almacenamiento histórico de métricas antes y después de cada recomendación aplicada. | Almacenar y comparar grandes volúmenes de datos puede incrementar costos operativos. | El sistema debe implementar un esquema de almacenamiento eficiente que consolide datos de impacto con resolución diaria, evitando duplicación de registros históricos. |
| **S — Social** | Los usuarios con baja experiencia en publicidad digital pueden no comprender el valor de un sistema que aprende de sus decisiones. | La percepción de "caja negra" puede generar desconfianza y abandono del sistema. | El sistema debe mostrar al usuario de forma visual y comprensible cómo sus interacciones anteriores han influido en la mejora de las recomendaciones recientes. |
| **T — Tecnológico** | La medición del impacto real de una recomendación depende de la sincronización oportuna de datos desde Meta Ads, Shopify y Dropi, que tienen latencias variables. | Datos desactualizados pueden generar evaluaciones de impacto incorrectas que alimenten el modelo con información errónea. | El sistema debe validar la frescura de los datos antes de calcular el impacto de una recomendación, marcando el resultado como "preliminar" hasta contar con datos completos del período evaluado. |
| **L — Legal** | El historial de interacciones del usuario con las recomendaciones constituye un perfil de comportamiento que cae bajo la Ley 1581 de Habeas Data en Colombia. | Almacenar este historial sin consentimiento explícito o sin permitir su eliminación puede ser una infracción legal. | El sistema debe informar al usuario que se registrará su comportamiento de adopción de recomendaciones para personalizar el sistema, y debe permitir la eliminación de ese historial a petición del usuario. |
| **É — Ético** | El sistema puede reforzar patrones de decisión del usuario aunque esos patrones no sean óptimos para la rentabilidad del negocio, si simplemente aprende a adaptar las recomendaciones a las preferencias del usuario. | Un sistema que aprende a recomendar solo lo que el usuario acepta puede volverse complaciente y dejar de ofrecer valor real. | El sistema debe balancear el aprendizaje basado en preferencias del usuario con parámetros objetivos de rentabilidad del negocio, priorizando el beneficio económico real sobre la aceptabilidad de las recomendaciones. |

---

## 2.3 RF3: Creatividades desde el Rendimiento

| Factor | Situación | Requerimiento derivado |
| --- | --- | --- |
| Político | Regulación futura de IA generativa en publicidad | P1: El sistema debe etiquetar anuncios generados por IA en la metadata. |
| Político | Transparencia en publicidad dirigida | P2: El sistema debe generar reportes auditables sobre creación de anuncios. |
| Económico | Presupuestos en USD y ventas en COP | E1: El sistema debe normalizar métricas usando tasa de cambio vigente. |
| Económico | CPM creciente obliga optimización | E2: El sistema debe mostrar impacto del CPM en rentabilidad. |
| Social | Preferencia por anuncios auténticos (UGC) | S1: El sistema debe clasificar creatividades por estilo y correlacionar con rendimiento. |
| Social | Fatiga publicitaria | S2: El sistema debe medir fatiga mediante caída progresiva del CTR. |
| Tecnológico | Uso de Meta Ads API y Shopify | T1: El sistema debe integrarse con APIs externas para campañas y ventas reales. |
| Tecnológico | Restricciones de tracking (cookies/iOS) | T2: El sistema debe manejar atribución con datos disponibles. |
| Legal | Habeas Data (Ley 1581) | L1: El sistema debe registrar consentimiento antes de consolidar datos personales. |
| Legal | Derecho al olvido y portabilidad | L2: El sistema debe permitir eliminación y exportación de datos personales. |
| Ambiental | Alto consumo energético de IA | A1: El sistema debe optimizar análisis con caché y modelos eficientes. |

---

## 2.4 RF4: Confianza Progresiva

### PESTLE — RF13: Agente Conversacional Visual

| Dimensión | Hallazgo | Impacto | Requerimiento derivado |
| --- | --- | --- | --- |
| **P — Político** | Colombia tiene en trámite el Proyecto de Ley 043 de 2025 de Inteligencia Artificial, radicado ante el Congreso por MinCiencias y MinTIC, que clasifica los sistemas de IA por nivel de riesgo. Los agentes conversacionales que toman decisiones comerciales podrían clasificarse como riesgo limitado o alto según este marco. | Si el proyecto es aprobado, los agentes de IA conversacionales deberán cumplir con requisitos de trazabilidad, transparencia y gobernanza. | El sistema debe documentar y hacer trazable toda acción sugerida o ejecutada por el agente de IA. |
| **E — Económico** | La síntesis de voz clonada y el procesamiento LLM en tiempo real implican costos por token y por llamada a APIs externas. Con más de 5.600 usuarios activos, el costo por interacción puede escalar rápidamente. | Sin control de consumo, el servicio puede volverse inviable a escala. | El sistema debe gestionar el consumo por niveles de suscripción e implementar caché de respuestas frecuentes para reducir costos. |
| **S — Social** | Usuarios con discapacidad auditiva pueden verse excluidos de la interacción verbal. | Un agente que solo funciona por voz excluye a usuarios con discapacidad auditiva o en entornos ruidosos. | El sistema debe mostrar siempre el texto de las respuestas de forma simultánea a la voz. |
| **T — Tecnológico** | La síntesis de voz en tiempo real con más de 5.600 usuarios puede desbordarse bajo alta concurrencia. | Si el motor de voz se satura, el agente pierde respuesta en tiempo real destruyendo la experiencia del usuario. | El sistema debe degradar al modo texto cuando el procesamiento de voz supere la capacidad disponible. |
| **L — Legal** | El agente accede a datos financieros del negocio. En Colombia aplica la Ley 1581 de Habeas Data. Dado que Dropi opera en Europa con más de 180.000 usuarios, el EU AI Act exige que los usuarios sean informados de que interactúan con una máquina. | No identificar el agente como IA ante usuarios europeos viola el EU AI Act, con multas de hasta 35 millones de euros. | El sistema debe identificar al agente como IA al inicio de cada sesión y cifrar las conversaciones almacenadas. |
| **É — Ético** | La voz clonada puede ofrecerse como una opción elegible por el usuario junto a otras alternativas como voz sintética estándar o solo texto. | Si el usuario no sabe que interactúa con una IA, la confianza puede erosionarse cuando lo descubra. | El sistema debe ofrecer la voz clonada como una opción entre varias e identificar siempre al agente como IA independientemente de la modalidad elegida. |

### PESTLE — RF14: Recomendaciones Inteligentes

| Dimensión | Hallazgo | Impacto | Requerimiento derivado |
| --- | --- | --- | --- |
| **P — Político** | Meta Ads ya está implementando en 2025-2026 restricciones en el acceso a datos para categorías sensibles (salud, finanzas, política). | El sistema puede perder datos clave para generar recomendaciones en categorías restringidas. | El sistema debe adaptarse cuando una fuente de datos esté parcialmente restringida sin interrumpir el servicio. |
| **E — Económico** | Un usuario promedio invierte entre 1.500 y 2.000 USD/mes en publicidad digital. | Una recomendación incorrecta puede generar pérdidas significativas y abandono de la plataforma. | El sistema debe mostrar el nivel de confianza de cada recomendación y advertir cuando los datos sean insuficientes. |
| **S — Social** | Entendimiento de las métricas dentro de ROAX. | Si las recomendaciones usan jerga técnica el usuario no actúa sobre ellas. | El sistema debe presentar las recomendaciones en lenguaje no técnico. |
| **T — Tecnológico** | El cruce de datos entre Meta, Shopify y Dropi hoy es manual porque son bases de datos distintas. | Datos inconsistentes pueden generar recomendaciones incorrectas y dañinas. | El sistema debe indicar la última sincronización de cada fuente y marcar recomendaciones de baja confianza si los datos están desactualizados. |
| **L — Legal** | El EU AI Act exige transparencia sobre decisiones generadas por IA. | El sistema puede generar expectativas incorrectas si no aclara la naturaleza de sus sugerencias. | El sistema debe avisar que las recomendaciones son sugerencias automatizadas y que el usuario conserva la decisión final. |
| **É — Ético** | Usar datos agregados de todos los usuarios para mejorar recomendaciones individuales es válido y valioso. | El modelo puede volverse sesgado y perjudicial si no contrasta con parámetros objetivos de rentabilidad. | El sistema debe combinar el aprendizaje individual con benchmarks de industria y alertar cuando los patrones del usuario afecten negativamente su ROAS. |

### PESTLE — RF15: Gestión de Alertas

| Dimensión | Hallazgo | Impacto | Requerimiento derivado |
| --- | --- | --- | --- |
| **P — Político** | Dado que Dropi opera en Europa, el envío de alertas con datos financieros a usuarios europeos está sujeto al GDPR y al EU AI Act. | Sin cumplimiento del GDPR, ROAX puede recibir sanciones regulatorias europeas. | El sistema debe diferenciar los perfiles de notificación según la región del usuario. |
| **E — Económico** | El envío masivo de alertas por correo o push implica costos por notificación que escalan con la base de usuarios. | Sin control, los costos de notificación pueden volverse inviables económicamente. | El sistema debe agrupar alertas para reducir el volumen de notificaciones sin perder cobertura crítica. |
| **S — Social** | Laura mencionó que el sistema anterior generaba hasta 250 alertas diarias causando fatiga total. | La saturación de alertas lleva al usuario a desactivarlas todas, perdiendo el valor del monitoreo 24/7. | El sistema debe limitar las alertas críticas y ofrecer canales menos invasivos configurables por el usuario. |
| **T — Tecnológico** | El motor de alertas debe operar 24/7. | Una falla nocturna puede generar pérdidas significativas y destruir la confianza en el sistema. | El sistema debe implementar redundancia en el motor de alertas y notificar al usuario ante cualquier interrupción. |
| **L — Legal** | Las alertas con métricas financieras enviadas por canales externos deben estar cifradas según la Ley 1581 y el GDPR. | El envío de datos financieros sin cifrado constituye una violación de datos personales. | El sistema debe cifrar el contenido de las notificaciones que incluyan métricas financieras del usuario. |
| **É — Ético** | El sistema prioriza alertas por impacto económico absoluto, lo que puede perjudicar a usuarios con menor volumen de inversión. | Un usuario pequeño puede perder el 100% de su presupuesto sin recibir alertas críticas. | El sistema debe calcular el impacto de las alertas de forma relativa al presupuesto de cada usuario. |

### PESTLE — RF16: Retroalimentación y Aprendizaje

| Dimensión | Hallazgo | Impacto | Requerimiento derivado |
| --- | --- | --- | --- |
| **P — Político** | ROAX opera actualmente en Latinoamérica y Europa a través de Dropi, que tiene más de 180.000 usuarios en esa región. El EU AI Act ya está en vigor desde agosto 2024 con alcance extraterritorial y multas de hasta 35 millones de euros. | Si el motor de aprendizaje no es auditable, ROAX puede enfrentar sanciones europeas. | El sistema debe mantener logs auditables de cómo la retroalimentación del usuario modifica el modelo de recomendaciones. |
| **E — Económico** | El reentrenamiento del modelo con retroalimentación de más de 5.600 usuarios puede crecer en costos computacionales de forma no lineal. | Costos insostenibles pueden limitar la frecuencia de actualización reduciendo la personalización percibida. | El sistema debe actualizar el modelo por lotes con un ciclo máximo de 24 horas para optimizar costos. |
| **S — Social** | Usuarios con alta desconfianza inicial rechazan todas las recomendaciones sin probarlas. | Sin interacciones iniciales el sistema no puede personalizar, generando el ciclo de baja confianza. | El sistema debe ofrecer un modo de observación donde el usuario vea el impacto hipotético de recomendaciones sin necesidad de aplicarlas. |
| **T — Tecnológico** | La automatización completa requiere integración con la API de Meta, que ya ha cambiado políticas de forma abrupta y está restringiendo categorías en 2025-2026. | Si Meta revoca permisos sin aviso, la automatización falla en el momento más crítico. | El sistema debe verificar los permisos de escritura de Meta antes de cada acción automatizada. |
| **L — Legal** | El historial de comportamiento del usuario es un dato personal bajo la Ley 1581 y el GDPR, que incluye el derecho al olvido para usuarios europeos. | Almacenar datos de comportamiento sin mecanismo de eliminación viola ambas regulaciones. | El sistema debe permitir al usuario eliminar su historial de interacciones y reiniciar su modelo personalizado. |
| **É — Ético** | La IA debe usar datos de toda la base de usuarios para enriquecer recomendaciones, pero también debe proteger al usuario de reforzar sus propias malas prácticas. | El sistema puede volverse cómplice de pérdidas si refuerza decisiones que el usuario acepta pero que son objetivamente perjudiciales. | El sistema debe balancear el aprendizaje individual con parámetros objetivos de rentabilidad de la industria. |

---

# 3. RF1: Datos y Decisiones

## 3.1 Historias de Usuario

### HU RF1.1 — Visualización de rentabilidad real por campaña

| Historia N° | RF1.1 |
| --- | --- |
| **Yo como** | dropshipper |
| **Quiero** | que el sistema cruce automáticamente mis datos de inversión en Meta Ads con las ventas reales de mi tienda |
| **Para** | saber en tiempo real cuánto estoy ganando o perdiendo por cada campaña activa, sin tener que hacer los cálculos yo mismo |

**Escenario RF1.1.1 — Cálculo del margen neto real por campaña**

| | |
| --- | --- |
| **Given** | el dropshipper tiene sesión iniciada y ha integrado su cuenta de Meta Ads y su tienda en ROAX |
| **When** | accede al dashboard de rentabilidad |
| **Then** | el sistema muestra el margen neto real por campaña usando órdenes efectivamente entregadas, no solo las vendidas |
| **And** | el dashboard distingue entre órdenes entregadas, pendientes y devueltas |

**Escenario RF1.1.2 — Actualización de datos con retraso máximo de 15 minutos**

| | |
| --- | --- |
| **Given** | el dropshipper tiene campañas activas con datos en Meta Ads y Shopify/Dropi |
| **When** | consulta el dashboard de rentabilidad |
| **Then** | el sistema muestra información actualizada con un máximo de 15 minutos de retraso respecto a las fuentes de datos |
| **And** | se indica la hora de la última actualización |

---

### HU RF1.2 — Detección proactiva de campañas deficitarias

| Historia N° | RF1.2 |
| --- | --- |
| **Yo como** | dropshipper |
| **Quiero** | recibir una alerta automática cuando alguna campaña activa esté por debajo del punto de equilibrio real de mi producto |
| **Para** | poder actuar antes de perder más dinero del necesario |

**Escenario RF1.2.1 — Alerta por campaña bajo el punto de equilibrio**

| | |
| --- | --- |
| **Given** | el dropshipper tiene una campaña activa con el margen del producto registrado en ROAX |
| **When** | el ROAS de la campaña cae por debajo del umbral de equilibrio durante más de 2 horas continuas |
| **Then** | el sistema genera una alerta automática indicando qué campaña está afectada |
| **And** | la alerta muestra cuánto dinero se está perdiendo por hora y desde cuándo ocurre la caída |

**Escenario RF1.2.2 — Cálculo automático del ROAS de equilibrio**

| | |
| --- | --- |
| **Given** | el dropshipper ha registrado el margen del producto en ROAX |
| **When** | el sistema analiza el rendimiento de la campaña |
| **Then** | calcula automáticamente el ROAS de equilibrio a partir del margen del producto registrado |
| **And** | usa ese umbral como referencia para activar alertas de déficit |

---

### HU RF3.1 — Configuración de reglas de automatización personalizadas

| Historia N° | RF3.1 |
| --- | --- |
| **Yo como** | dropshipper |
| **Quiero** | poder configurar mis propias reglas de automatización, como pausar campañas o ajustar presupuestos, basadas en la rentabilidad real de mi negocio |
| **Para** | tener control sobre las acciones automáticas del sistema sin depender solo de las métricas de Meta |

**Escenario RF3.1.1 — Configuración exitosa de una regla**

| | |
| --- | --- |
| **Given** | el dropshipper tiene sesión iniciada y campañas activas conectadas en ROAX |
| **When** | accede al módulo de automatización y crea una nueva regla definiendo la condición, la acción y los límites de actuación |
| **Then** | el sistema guarda la regla y la activa de inmediato para monitorear las campañas según los parámetros definidos |
| **And** | la regla aparece listada en el panel de automatización con su estado activo |

---

### HU RF3.2 — Registro auditado de acciones automáticas

| Historia N° | RF3.2 |
| --- | --- |
| **Yo como** | dropshipper |
| **Quiero** | que el sistema registre cada acción automática que ejecute, indicando qué hizo, cuándo y por qué |
| **Para** | poder revisar el historial de decisiones del sistema y entender si está actuando correctamente sobre mis campañas |

**Escenario RF3.2.1 — Consulta del historial de acciones automáticas**

| | |
| --- | --- |
| **Given** | el dropshipper tiene sesión iniciada y el sistema ha ejecutado al menos una acción automática |
| **When** | accede al módulo de historial de automatización |
| **Then** | el sistema muestra una lista cronológica de todas las acciones ejecutadas, con la fecha, la campaña afectada, la acción tomada y la regla o condición que la disparó |
| **And** | cada entrada incluye el estado anterior y posterior de la campaña para que el usuario pueda comparar |

**Escenario RF3.2.2 — Detalle de una acción automática específica**

| | |
| --- | --- |
| **Given** | el dropshipper está consultando el historial de acciones automáticas |
| **When** | selecciona una acción específica de la lista |
| **Then** | el sistema muestra el detalle completo: hora exacta, métricas que activaron la regla, la decisión tomada y si el usuario la revirtió manualmente después |
| **And** | ofrece la opción de deshacer la acción si aún es posible hacerlo |

---

### HU RF4.1 — Monitoreo continuo del negocio

| Historia N° | RF4.1 |
| --- | --- |
| **Yo como** | dropshipper |
| **Quiero** | que el sistema monitoree continuamente mis campañas en Meta Ads evaluando su rendimiento según la fase en que se encuentran (Testeo, Optimización o Escalado) y considerando el delay de 24 horas propio de la plataforma |
| **Para** | recibir alertas precisas que no confundan una campaña inmadura con una campaña fallida, y poder tomar decisiones correctas en el momento adecuado |

**Escenario RF4.1.1 — Evaluación de campaña en fase de Testeo con indicadores correctos**

| | |
| --- | --- |
| **Given** | el dropshipper tiene una campaña activa clasificada en fase de Testeo y el sistema ha recopilado datos con al menos 24 horas de antigüedad |
| **When** | el sistema evalúa el rendimiento de esa campaña |
| **Then** | analiza los indicadores propios de Testeo: Hook rate, Tasas de retención de atención, Retention rate y Click rate |
| **And** | no emite alertas de CPA o ROAS hasta que la campaña haya superado la fase de madurez mínima |

**Escenario RF4.1.2 — Detección de bajo rendimiento en fase de Escalado**

| | |
| --- | --- |
| **Given** | el dropshipper tiene una campaña en fase de Escalado con umbrales de CPA y ROAS neto configurados |
| **When** | el sistema detecta que el CPA supera el umbral definido o que el ROAS neto cae por debajo del punto de equilibrio |
| **Then** | genera una alerta indicando la campaña afectada, la fase en que se encuentra y el indicador crítico que falló |
| **And** | registra el evento con la hora, los valores detectados y el contexto de madurez de la campaña |

---

### HU RF5.1 — Protección de datos bajo Ley de Habeas Data

| Historia N° | RF5.1 |
| --- | --- |
| **Yo como** | dropshipper |
| **Quiero** | que el sistema cifre y proteja los datos personales de mis clientes y pedidos provenientes de Shopify o Dropi, cumpliendo con la Ley de Habeas Data |
| **Para** | garantizar que la información privada de mis compradores esté segura y que mi negocio opere dentro del marco legal colombiano |

**Escenario RF5.1.1 — Cifrado de datos personales en tránsito**

| | |
| --- | --- |
| **Given** | el sistema está recibiendo datos de clientes y pedidos desde Shopify o Dropi mediante la integración configurada |
| **When** | los datos se transmiten entre las plataformas externas y ROAX |
| **Then** | el sistema aplica cifrado TLS 1.3 sobre toda la comunicación que contenga información personal |
| **And** | cualquier intento de conexión con protocolos de menor versión es rechazado automáticamente |

**Escenario RF5.1.2 — Datos personales no expuestos en logs ni interfaces no autorizadas**

| | |
| --- | --- |
| **Given** | el sistema ha procesado órdenes con datos personales de clientes |
| **When** | se generan registros internos de actividad, errores o auditoría |
| **Then** | el sistema omite o enmascara los datos personales identificables (nombre, teléfono, dirección) en los logs del sistema |
| **And** | los datos completos solo son accesibles desde las vistas habilitadas para roles con permiso explícito |

---

### HU RF5.2 — Control de acceso diferenciado por roles

| Historia N° | RF5.2 |
| --- | --- |
| **Yo como** | dropshipper con equipo de trabajo |
| **Quiero** | que el sistema restrinja el acceso a la información financiera según el rol de cada miembro del equipo, diferenciando entre Administrador y Vendedor |
| **Para** | que los datos sensibles de mi negocio solo los vea quien realmente debe verlos, y no queden expuestos a todo el equipo |

**Escenario RF5.2.1 — Acceso restringido del rol Vendedor a datos financieros**

| | |
| --- | --- |
| **Given** | un miembro del equipo tiene el rol de Vendedor y ha iniciado sesión en ROAX |
| **When** | intenta acceder a las secciones de rentabilidad por campaña, costos de pauta o márgenes del producto |
| **Then** | el sistema le deniega el acceso y muestra un mensaje indicando que esa información solo está disponible para Administradores |
| **And** | el intento de acceso queda registrado en el log de actividad de la cuenta |

**Escenario RF5.2.2 — Asignación de roles por parte del Administrador**

| | |
| --- | --- |
| **Given** | el dropshipper tiene rol de Administrador y tiene al menos un colaborador registrado en su cuenta de ROAX |
| **When** | accede al módulo de gestión de equipo y asigna o modifica el rol de un colaborador |
| **Then** | el sistema aplica los nuevos permisos de forma inmediata sin necesidad de reiniciar sesión |
| **And** | el colaborador solo puede ver y operar las secciones habilitadas para su rol desde ese momento |

---

### HU RF6.1 — Transparencia de costos antes de ejecutar cambios de presupuesto

| Historia N° | RF6.1 |
| --- | --- |
| **Yo como** | dropshipper |
| **Quiero** | que el sistema me informe previamente sobre cualquier costo adicional, comisión o cargo asociado a cambios automáticos de presupuesto o integraciones externas |
| **Para** | tomar decisiones informadas y evitar gastos inesperados en mi operación publicitaria |

**Escenario RF6.1.1 — Notificación de costo adicional antes de aumentar presupuesto**

| | |
| --- | --- |
| **Given** | el dropshipper tiene campañas activas y el sistema detecta una oportunidad de aumentar automáticamente el presupuesto de pauta |
| **When** | la acción implica costos adicionales por integración, procesamiento o comisiones de terceros |
| **Then** | el sistema muestra una notificación detallando el costo estimado antes de ejecutar el cambio |
| **And** | solicita confirmación explícita del usuario para continuar con la operación |

**Escenario RF6.1.2 — Visualización de costos asociados a integraciones externas**

| | |
| --- | --- |
| **Given** | el dropshipper desea conectar una nueva integración externa dentro de ROAX |
| **When** | el dropshipper inicia el proceso de conexión con una nueva integración |
| **Then** | el sistema informa claramente el tipo de costo, su frecuencia y el servicio asociado antes de completar la integración |
| **And** | el usuario puede aceptar o cancelar el proceso antes de que se genere cualquier cargo |

---

### HU RF6.2 — Interfaz Conversacional de ROAX vía WhatsApp

| Historia N° | RF6.2 |
| --- | --- |
| **Yo como** | dropshipper |
| **Quiero** | interactuar con el sistema a través de un chatbot inteligente en WhatsApp |
| **Para** | supervisar mis campañas, recibir diagnósticos y ejecutar acciones usando lenguaje natural, sin tener que entrar a una plataforma externa o interpretar gráficos complejos |

**Escenario RF6.2.1 — Ejecución de acción inmediata mediante comando en WhatsApp**

| | |
| --- | --- |
| **Given** | el usuario recibe un mensaje de alerta del bot en WhatsApp informando que una campaña tiene un rendimiento deficiente |
| **When** | el usuario responde al chat con un comando natural como "Pausa esa campaña" |
| **Then** | el sistema procesa el lenguaje y ejecuta la instrucción de pausa en la plataforma publicitaria de forma instantánea |
| **And** | el bot responde confirmando: "Listo, campaña pausada exitosamente." |

**Escenario RF6.2.2 — Consulta de métricas de forma conversacional**

| | |
| --- | --- |
| **Given** | el usuario ha iniciado sesión en la aplicación móvil de ROAX |
| **When** | envía un mensaje al bot preguntando: "¿Cómo vamos hoy de rentabilidad?" o "¿Cuál es el margen neto?" |
| **Then** | el sistema interpreta la intención y cruza los datos del negocio en tiempo real |
| **And** | el bot responde con un resumen conciso y fácil de leer detallando las métricas directamente en el chat |

---

### HU RF7.1 — Registro de inventario para decisiones contextualizadas

| Historia N° | RF7.1 |
| --- | --- |
| **Yo como** | dropshipper |
| **Quiero** | que el sistema se sincronice automáticamente con el inventario real de mis productos en mis plataformas de venta y pause las campañas cuando el stock se agote |
| **Para** | no seguir gastando presupuesto en publicidad de productos que ya no puedo entregar y reactivar las campañas en cuanto reabastezca el inventario |

**Escenario RF7.1.1 — Pausa automática de campaña por agotamiento de stock**

| | |
| --- | --- |
| **Given** | el dropshipper tiene una campaña activa promocionando un producto que aún tiene stock en su tienda integrada |
| **When** | el sistema detecta que el stock disponible del producto cae a cero o por debajo del umbral mínimo configurado |
| **Then** | el sistema pausa automáticamente la campaña asociada a ese producto |
| **And** | registra la acción en el historial indicando el motivo (agotamiento de inventario) y notifica al dropshipper para que reabastezca |

**Escenario RF7.1.2 — Reactivación de campaña tras reposición de inventario**

| | |
| --- | --- |
| **Given** | el dropshipper tenía una campaña pausada automáticamente por falta de stock y ha reabastecido el producto en su tienda |
| **When** | el sistema detecta que el inventario del producto vuelve a estar por encima del umbral mínimo configurado |
| **Then** | el sistema reactiva automáticamente la campaña previamente pausada |
| **And** | notifica al dropshipper que la campaña ha vuelto a estar activa, indicando la fecha y la cantidad de stock detectada |

---

### HU RF7.2 — Registro de restricciones financieras del negocio

| Historia N° | RF7.2 |
| --- | --- |
| **Yo como** | administrador |
| **Quiero** | poder registrar las restricciones financieras de mi negocio como deudas activas, límites de flujo de caja y presupuesto máximo mensual de pauta |
| **Para** | que la IA no me recomiende aumentos de presupuesto que mi negocio no puede asumir |

**Escenario RF7.2.1 — Registro de parámetros financieros del negocio**

| | |
| --- | --- |
| **Given** | el administrador tiene sesión iniciada en ROAX |
| **When** | accede al módulo de configuración financiera y registra el presupuesto máximo de pauta, el flujo de caja disponible y las deudas activas |
| **Then** | el sistema guarda esos parámetros como restricciones del negocio |
| **And** | los toma como referencia para validar futuras recomendaciones de la IA |

**Escenario RF7.2.2 — Bloqueo de recomendación que excede el límite financiero**

| | |
| --- | --- |
| **Given** | el administrador ha registrado un presupuesto máximo mensual de pauta |
| **When** | la IA evalúa una recomendación de aumento de presupuesto que superaría ese límite |
| **Then** | el sistema bloquea automáticamente la recomendación |
| **And** | muestra al administrador una explicación clara indicando que la propuesta fue restringida por el techo financiero configurado |

---

### HU RF7.3 — Definición de buyer persona para alineamiento de recomendaciones

| Historia N° | RF7.3 |
| --- | --- |
| **Yo como** | dropshipper |
| **Quiero** | poder definir el perfil cualitativo de mi cliente ideal (buyer persona) |
| **Para** | que las recomendaciones de creativos, segmentación y mensajes que me dé la IA estén alineadas con ese perfil y no sean genéricas |

**Escenario RF7.3.1 — Registro de atributos del buyer persona**

| | |
| --- | --- |
| **Given** | el dropshipper tiene sesión iniciada en ROAX |
| **When** | accede al módulo de buyer persona y registra rango de edad, intereses principales, ubicación geográfica y comportamiento de compra esperado |
| **Then** | el sistema guarda el perfil del cliente ideal asociado al negocio |
| **And** | ese perfil queda disponible para que la IA lo considere en sus recomendaciones |

**Escenario RF7.3.2 — Recomendaciones alineadas al buyer persona definido**

| | |
| --- | --- |
| **Given** | el dropshipper ha registrado el buyer persona de su negocio |
| **When** | la IA genera una recomendación sobre creativos, segmentación o horarios de pauta |
| **Then** | el sistema evalúa la pertinencia de la recomendación contra los atributos del buyer persona registrado |
| **And** | cada recomendación incluye una breve explicación de cómo se alinea con ese perfil |

---

### HU RF7.4 — Integración de tendencias externas del mercado

| Historia N° | RF7.4 |
| --- | --- |
| **Yo como** | dropshipper |
| **Quiero** | que la IA considere tendencias externas del mercado, como variaciones estacionales, picos de búsqueda en Google Trends y comportamiento publicitario de mi competencia |
| **Para** | recibir recomendaciones de pauta que se anticipen a oportunidades o riesgos del contexto externo, y no solo basadas en mi histórico interno |

**Escenario RF7.4.1 — Recomendación de aumento de presupuesto por pico estacional detectado**

| | |
| --- | --- |
| **Given** | el sistema está conectado a fuentes externas de tendencias del mercado y el dropshipper tiene campañas activas |
| **When** | el sistema detecta un pico de demanda estacional para una categoría de producto que el dropshipper está promocionando |
| **Then** | la IA genera una recomendación de aumento de presupuesto justificada con el dato externo detectado |
| **And** | la recomendación incluye una explicación clara del contexto que la motivó (por ejemplo, aumento del 60% en búsquedas de la categoría en Google Trends durante los últimos 7 días) |

**Escenario RF7.4.2 — Alerta por movimiento publicitario agresivo de la competencia**

| | |
| --- | --- |
| **Given** | el sistema monitorea el comportamiento publicitario de competidores definidos por el dropshipper a través de APIs públicas |
| **When** | detecta que un competidor directo aumentó significativamente su inversión publicitaria sobre un producto similar |
| **Then** | la IA genera una alerta contextual al dropshipper informando del movimiento de la competencia |
| **And** | propone ajustes posibles en su propia estrategia de pauta para no perder visibilidad en el mercado |

---

## 3.2 Casos de Uso

### 3.2.1 Diagramas de Casos de Uso

#### CU1
![Caso de uso CU1](Imagenes/RF1%20Datos%20y%20Decisiones/CU%201_page-0001.jpg)

#### CU2
![Caso de uso CU2](Imagenes/RF1%20Datos%20y%20Decisiones/CU%202_page-0001.jpg)

#### CU3
![Caso de uso CU3](Imagenes/RF1%20Datos%20y%20Decisiones/CU%203_page-0001.jpg)

#### CU4
![Caso de uso CU4](Imagenes/RF1%20Datos%20y%20Decisiones/CU%204_page-0001.jpg)

#### CU5
> Pendiente por integración de diagrama de caso de uso entregado por el equipo correspondiente.

#### CU6
![Caso de uso CU6](Imagenes/RF1%20Datos%20y%20Decisiones/CU%206_page-0001.jpg)

#### CU7
![Caso de uso CU7](Imagenes/RF1%20Datos%20y%20Decisiones/CU%207_page-0001.jpg)

### 3.2.2 Formatos Bicolumnares

[Formato Bicolumnar — RF1: Datos y Decisiones](https://docs.google.com/document/d/1Tl-pgph0c5_l7zp6FZbqnuXPiQ6JTkrJtpKxMOWy5VU/edit?usp=sharing)

---

## 4. RF2: Alertas que Razonan

### 4.1 Historias de Usuario

---

#### HU-RF2.1 — Diagnóstico contextual de anomalías mediante IA

| Campo | Contenido |
| --- | --- |
| **Historia N°** | HU-RF2.1 |
| **Yo como** | usuario de ROAX con campañas publicitarias activas |
| **Quiero** | recibir alertas predictivas acompañadas de un diagnóstico contextual generado por IA |
| **Para** | entender no solo qué métrica está fallando, sino por qué está ocurriendo y qué parte del negocio está siendo afectada |

##### Criterios de aceptación

- El sistema debe detectar desviaciones relevantes en métricas como ROAS, CPA o ventas reales.
- El sistema debe cruzar datos de pauta digital con datos de ventas reales.
- El sistema debe generar una explicación en lenguaje natural sobre la causa raíz de la alerta.
- El sistema debe mostrar la alerta contextual en la interfaz de ROAX.

**Prioridad:** Alta  
**Dependencias:** Integración con Meta Ads, Shopify y Dropi.

---

#### HU-RF2.2 — Recomendaciones inteligentes basadas en rendimiento

| Campo | Contenido |
| --- | --- |
| **Historia N°** | HU-RF2.2 |
| **Yo como** | emprendedor o administrador de e-commerce |
| **Quiero** | recibir recomendaciones inteligentes sobre ajustes de campañas, presupuesto o creatividades |
| **Para** | mejorar la rentabilidad de mi negocio sin tener que interpretar manualmente todos los datos |

##### Criterios de aceptación

- El sistema debe identificar campañas con bajo rendimiento.
- El sistema debe sugerir acciones concretas como pausar campañas, reducir presupuesto o reemplazar creativos.
- El sistema debe explicar la razón de cada recomendación.
- El sistema debe permitir aplicar las recomendaciones mediante botones de acción directa.

**Prioridad:** Alta  
**Dependencias:** Datos históricos de campañas, ventas y rendimiento de creatividades.

---

#### HU-RF2.3 — Automatización de decisiones delegadas

| Campo | Contenido |
| --- | --- |
| **Historia N°** | HU-RF2.3 |
| **Yo como** | usuario de ROAX |
| **Quiero** | configurar reglas para que la IA pueda tomar decisiones autónomas bajo límites definidos |
| **Para** | automatizar acciones repetitivas sin perder control sobre mis campañas y presupuesto |

##### Criterios de aceptación

- El sistema debe permitir configurar reglas de automatización.
- El sistema debe validar que una acción esté dentro de los límites definidos por el usuario.
- El sistema debe ejecutar acciones aprobadas automáticamente mediante Meta Ads API.
- El sistema debe notificar al usuario cada vez que se realice una acción autónoma.

**Prioridad:** Alta  
**Dependencias:** Integración con Meta Ads API y configuración previa de reglas.

---

#### HU-RF2.4 — Aprendizaje progresivo basado en interacciones

| Campo | Contenido |
| --- | --- |
| **Historia N°** | HU-RF2.4 |
| **Yo como** | usuario que recibe recomendaciones de ROAX |
| **Quiero** | que el sistema aprenda de mis decisiones y del impacto real de cada recomendación |
| **Para** | recibir sugerencias cada vez más precisas y adaptadas a mi negocio |

##### Criterios de aceptación

- El sistema debe registrar si el usuario acepta, rechaza o ignora una recomendación.
- El sistema debe comparar métricas antes y después de aplicar una recomendación.
- El sistema debe mostrar evidencia del impacto generado.
- El sistema debe usar los resultados históricos para mejorar futuras recomendaciones.

**Prioridad:** Media  
**Dependencias:** Historial de recomendaciones, métricas posteriores y motor de IA.

---

## 4.2 Casos de Uso

### 4.2.1 Diagramas de Casos de Uso

#### CU-RF1 — Generar alertas predictivas y diagnósticos contextuales mediante IA
![Caso de uso CU-RF1](Imagenes/RF2%20Alertas%20Inteligentes/CU1.jpg)

#### CU-RF2 — Emitir recomendaciones inteligentes basadas en el rendimiento del negocio
![Caso de uso CU-RF2](Imagenes/RF2%20Alertas%20Inteligentes/CU2.jpg)

#### CU-RF3 — Automatizar la toma de decisiones autónomas sobre campañas publicitarias
![Caso de uso CU-RF3](Imagenes/RF2%20Alertas%20Inteligentes/CU3.jpg)

#### CU-RF4 — Construir confianza progresiva y aprender del impacto de las recomendaciones
![Caso de uso CU-RF4](Imagenes/RF2%20Alertas%20Inteligentes/CU4.jpg)

### 4.2.2 Formatos Bicolumnares

#### Formato Bicolumnar — CU-RF1: Generar alertas predictivas y diagnósticos contextuales mediante IA

| Campo | Detalle |
| --- | --- |
| **ID** | CU-RF1 |
| **Autor** | Mario Romero y Mariana Carmona |
| **Caso de uso** | Generar alertas predictivas y diagnósticos contextuales mediante IA |

**Casos de uso relacionados**

**CU-RF1.1 — Analizar desviaciones de métricas clave:** El sistema obtiene continuamente las métricas de pauta digital (Meta Ads) y los datos reales de ventas de los e-commerce (Shopify, Dropi), ejecutando una monitorización constante para identificar anomalías críticas como caídas drásticas de ROAS o incrementos inusuales en el CPA.

**CU-RF1.2 — Procesar anomalías a través de un LLM:** Al detectarse una desviación fuera de los rangos normales, el sistema envía los datos estructurados del incidente junto con el historial de la marca a un Modelo de Lenguaje de Gran Escala (LLM) para que interprete el contexto y estructure la lógica del hallazgo.

**CU-RF1.3 — Redactar diagnósticos automatizados en lenguaje natural:** El sistema transforma el análisis del LLM en un informe legible y detallado de cara al usuario, explicitando con precisión matemática y narrativa la causa raíz de la alerta (por ejemplo, especificando qué campaña publicitaria exacta está perdiendo rentabilidad y los motivos asociados).

**Precondición:** Las cuentas de pauta digital (Meta Ads) y los canales de venta (Shopify, Dropi) deben estar correctamente integrados y sincronizando datos en tiempo real en la plataforma ROAX.

**Contexto:** El sistema debe automatizar la interpretación del estado del negocio, evitando que el usuario deba realizar análisis manuales, informándole con precisión qué anomalías ocurren y por qué están sucediendo.

**Secuencia normal**

| Paso | Acción |
| --- | --- |
| 1 | El sistema recopila periódicamente los datos agregados de inversión publicitaria (Meta Ads) y facturación comercial (Shopify, Dropi). |
| 2 | El sistema calcula las variaciones de rendimiento y detecta si indicadores como el ROAS o el CPA presentan desviaciones anómalas respecto a la media histórica del negocio. |
| 3 | El sistema recopila el contexto histórico inmediato de la marca y las métricas afectadas para estructurar el prompt de análisis. |
| 4 | El sistema procesa la información recopilada mediante un Modelo de Lenguaje (LLM) para identificar patrones y correlaciones de causa-raíz. |
| 5 | El sistema genera un diagnóstico automatizado explicativo redactado en lenguaje natural. |
| 6 | El sistema despacha y expone la alerta contextual estructurada a través de las interfaces web de ROAX (app.roaxai.com) y el módulo de Dropi. |

**Postcondición:** El usuario visualiza una notificación detallada en tiempo real que contiene el valor de la métrica afectada y la explicación textual de la causa raíz de la anomalía.

**Excepciones**

| Paso | Acción |
| --- | --- |
| 1 | Fallo de conexión o pérdida de credenciales con las APIs externas → El sistema registra el error en la bitácora y notifica al usuario la necesidad de reautenticar la integración afectada. |
| 4 | Timeout o indisponibilidad del LLM → El sistema reintenta la solicitud de forma interna. Si el fallo persiste, genera una alerta básica basada en reglas tradicionales. |
| 5 | El diagnóstico arrojado carece de coherencia formal o contiene errores → El sistema valida la estructura mediante filtros sintácticos y muestra únicamente las métricas numéricas. |

**Comentarios:** Este requerimiento cambia el paradigma pasivo de las alertas tradicionales de ROAX, pasando de un enfoque puramente cuantitativo ("Qué pasa") a un enfoque cualitativo y de razonamiento asistido por IA ("Por qué pasa").

---

#### Formato Bicolumnar — CU-RF2: Emitir recomendaciones inteligentes basadas en el rendimiento del negocio

| Campo | Detalle |
| --- | --- |
| **ID** | CU-RF2 |
| **Autor** | Equipo Reto 2 |
| **Caso de uso** | Emitir recomendaciones inteligentes basadas en el rendimiento del negocio |

**Casos de uso relacionados**

**CU-RF2.1 — Sugerir ajustes de presupuesto y estado de campañas:** El sistema analiza la rentabilidad real de cada campaña activa comparando el ROAS, CPA y margen neto con los umbrales del negocio. Cuando detecta campañas que están "quemando" dinero (ROAS por debajo del umbral durante N días consecutivos o CPA superior al costo del producto), sugiere de forma proactiva pausarlas o reducir su presupuesto diario, indicando el ahorro estimado. De igual forma, si detecta campañas de alto rendimiento con presupuesto limitado, recomienda aumentar la inversión y proyecta el retorno esperado.

**CU-RF2.2 — Proponer sustitución de creativos de bajo rendimiento:** El sistema identifica las piezas gráficas o videos con CTR, ROAS o tasa de conversión por debajo del promedio histórico de la marca. Para cada creativo de bajo rendimiento detectado, propone su reemplazo por un nuevo anuncio generado con ROAX Ads, priorizando los formatos y estilos visuales que han demostrado mayor probabilidad de conversión según los datos históricos del negocio. La propuesta incluye una vista previa del creativo sugerido y la comparación de métricas esperadas frente al actual.

**CU-RF2.3 — Permitir aplicación directa de mejoras desde la alerta:** Cada tarjeta de recomendación incluye botones de acción directa que permiten al usuario implementar la mejora sugerida al instante, sin salir del panel: pausar campaña, ajustar presupuesto, lanzar creativo nuevo o programar el cambio para más tarde. La interfaz muestra el estado de la acción en tiempo real y registra el resultado para el ciclo de aprendizaje del sistema.

**Precondición:** El usuario debe tener al menos una campaña publicitaria activa con datos conectados desde Meta Ads (Facebook/Instagram). El sistema necesita los datos de ventas de la tienda en línea (Shopify, Tiendanube, WooCommerce o Dropi) para calcular las ganancias reales. El usuario debe fijar sus metas de ganancias (lo mínimo que quiere ganar o lo máximo que puede gastar por venta); si no lo hace, el sistema usará los promedios estándar del mercado.

**Contexto:** El usuario es un emprendedor o administrador de una tienda en línea que invierte en publicidad digital. No solo necesita ver gráficas o datos, sino saber exactamente qué pasos dar para que su negocio sea más rentable. La plataforma debe ir más allá de mostrar reportes y convertirse en una guía que proponga acciones claras que se puedan activar directamente desde la pantalla.

**Secuencia normal**

| Paso | Acción |
| --- | --- |
| El usuario entra a la sección de sugerencias. | El sistema analiza las ganancias en ese momento, cruza los datos de los anuncios con las ventas reales y organiza las sugerencias de mayor a menor importancia. |
| El usuario revisa la sugerencia sobre el presupuesto del anuncio. | El sistema muestra el anuncio analizado, la razón del aviso (por qué está perdiendo dinero y cuánto), el cambio recomendado y la mejora económica que se espera lograr. |
| El usuario revisa la sugerencia sobre el diseño del anuncio. | El sistema señala la imagen o video que no funciona, muestra sus datos actuales, genera una propuesta visual nueva y compara el beneficio estimado. |
| El usuario decide aceptar o rechazar la sugerencia. | El sistema guarda la decisión, el tiempo que tardó en responder y la razón (si decidió rechazarla) para entender mejor las preferencias del usuario. |
| El usuario presiona el botón de acción rápida. | El sistema aplica el cambio y, tras pasar al menos 24 horas, reúne los nuevos resultados para calcular el impacto real de la decisión y compararlo con lo que había prometido. |
| El usuario revisa cómo quedó todo después del cambio. | El sistema muestra una comparación de "antes y después" con dinero y porcentajes reales, y le pide al usuario que califique si la sugerencia fue útil, incorrecta o poco importante. |

**Postcondición:** Los cambios en los anuncios y presupuestos se aplican automáticamente en la cuenta de Meta Ads. El sistema registra cada acción para medir su impacto real a corto plazo y personaliza el asistente según los gustos y decisiones del usuario.

**Excepciones**

| Paso | Acción |
| --- | --- |
| No hay datos históricos suficientes para calcular rentabilidad. | El sistema muestra un aviso indicando la falta de datos, sugiere conectar la fuente de ventas correspondiente y deshabilita los botones de acción directa hasta tener información fiable. |
| La API de Meta Ads no responde al intentar aplicar un cambio. | El sistema informa del fallo de conexión, guarda la acción como pendiente y reintenta automáticamente en el próximo ciclo de sincronización. |
| El usuario no tiene configurados umbrales de rentabilidad. | El sistema aplica valores por defecto basados en benchmarks del sector e-commerce y notifica al usuario que puede personalizar dichos umbrales en la configuración. |
| ROAX Ads no puede generar el creativo sugerido por falta de activos de marca. | El sistema informa que faltan imágenes o textos de referencia, redirige al usuario a subir activos en la sección de configuración de marca y mantiene la recomendación en estado pendiente. |

**Comentarios:** El motivo de cada sugerencia siempre se redactará de forma sencilla y transparente, detallando los datos exactos que la provocaron (cumpliendo con las normativas de transparencia y ética en Inteligencia Artificial). El sistema monitorea si el usuario acepta, rechaza o ignora los consejos. Esto sirve para educar a la herramienta, haciendo que las futuras sugerencias sean cada vez más precisas y adaptadas a la realidad del negocio.

---

#### Formato Bicolumnar — CU-RF3: Automatizar la toma de decisiones autónomas sobre campañas publicitarias

| Campo | Detalle |
| --- | --- |
| **ID** | CU-RF3 |
| **Autor** | Colaboradores Reto 2 |
| **Caso de uso** | Automatizar la toma de decisiones autónomas sobre campañas publicitarias |

**Casos de uso relacionados**

**CU-RF3.1 — Configurar reglas de automatización:** El sistema proporciona un panel de configuración donde el usuario define los límites, condiciones y acciones permitidas para la toma de decisiones autónomas por parte de la IA, incluyendo umbrales de ROAS, presupuesto y restricciones operativas.

**CU-RF3.2 — Ejecutar acciones autónomas en Meta Ads:** El sistema monitorea continuamente las métricas publicitarias y ejecuta automáticamente las acciones previamente autorizadas por el usuario cuando se cumplen las condiciones definidas en las reglas de automatización.

**CU-RF3.3 — Notificar acciones autónomas realizadas:** El sistema genera y envía una notificación inmediata al usuario cada vez que la IA ejecuta una acción autónoma sobre alguna de sus campañas publicitarias.

**Precondición:** El usuario tiene al menos una cuenta publicitaria de Meta Ads conectada al sistema y ha configurado reglas de automatización activas.

**Contexto:** El usuario desea delegar determinadas decisiones operativas a la inteligencia artificial para optimizar el rendimiento de sus campañas publicitarias sin necesidad de intervención manual constante, manteniendo control mediante reglas previamente definidas y notificaciones de seguimiento.

**Secuencia normal**

| Paso | Acción |
| --- | --- |
| El usuario configura las reglas de automatización para sus campañas. | El sistema almacena los umbrales, restricciones y acciones autorizadas para la IA. |
| El usuario mantiene activas sus campañas publicitarias. | El sistema monitorea continuamente las métricas y condiciones definidas. |
| Se alcanza una condición previamente configurada por el usuario. | El sistema evalúa la regla correspondiente y verifica que la acción esté autorizada. |
| El usuario no requiere realizar ninguna intervención. | El sistema ejecuta automáticamente la acción aprobada mediante la API de Meta Ads. |
| La acción es aplicada exitosamente sobre la campaña. | El sistema registra la acción ejecutada junto con la fecha, hora y métricas asociadas. |
| El usuario recibe una notificación. | El sistema envía una confirmación inmediata detallando la acción realizada por la IA. |
| El usuario consulta el historial de automatizaciones. | El sistema presenta el registro completo de acciones autónomas ejecutadas y sus resultados. |

**Postcondición:** La acción autónoma queda ejecutada en la plataforma publicitaria, registrada en el historial del sistema y notificada al usuario.

**Excepciones**

| Paso | Acción |
| --- | --- |
| Se cumple una regla de automatización, pero la API de Meta Ads no está disponible. | El sistema registra el error, suspende temporalmente la ejecución y notifica al usuario. |
| La acción requerida excede los límites configurados por el usuario. | El sistema cancela la automatización y registra el evento en el historial. |
| La cuenta publicitaria pierde conexión con el sistema. | El sistema deshabilita temporalmente las automatizaciones asociadas hasta restablecer la conexión. |
| El servicio de notificaciones presenta fallas. | El sistema almacena la notificación pendiente y realiza nuevos intentos de envío. |
| El usuario elimina o modifica una regla mientras está siendo evaluada. | El sistema actualiza las condiciones de automatización y detiene la ejecución de reglas obsoletas. |

**Comentarios:** Las acciones autónomas pueden incluir pausado de campañas, ajuste de presupuestos, modificación de pujas o cualquier otra operación previamente autorizada por el usuario. Todas las decisiones ejecutadas por la IA deben respetar las restricciones configuradas y quedar registradas para auditoría y trazabilidad.

---

#### Formato Bicolumnar — CU-RF4: Construir confianza progresiva y aprender del impacto de las recomendaciones

| Campo | Detalle |
| --- | --- |
| **ID** | CU-RF4 |
| **Autor** | Colaboradores Reto 2 |
| **Caso de uso** | Construir confianza progresiva y aprender del impacto de las recomendaciones |

**Casos de uso relacionados**

**CU-RF4.1 — Registrar interacción del usuario con las recomendaciones:** El sistema registra todas las acciones realizadas por el usuario sobre las alertas y recomendaciones generadas, incluyendo aceptación, rechazo o ignorar la sugerencia, junto con su respectiva marca de tiempo.

**CU-RF4.2 — Medir impacto posterior a la ejecución:** El sistema compara continuamente el rendimiento de las campañas antes y después de la aplicación de una recomendación para determinar si la acción generó una mejora o deterioro en los resultados del negocio.

**CU-RF4.3 — Retroalimentar y optimizar el modelo de IA:** El sistema utiliza los resultados históricos obtenidos y los patrones de comportamiento del usuario para ajustar los modelos de inteligencia artificial y mejorar la calidad de futuras recomendaciones.

**Precondición:** Existen recomendaciones emitidas previamente y el usuario ha interactuado con al menos una de ellas.

**Contexto:** El usuario necesita evidencias del valor generado por las recomendaciones de la IA y el sistema requiere aprender continuamente de los resultados obtenidos para mejorar su precisión.

**Secuencia normal**

| Paso | Acción |
| --- | --- |
| El usuario recibe una recomendación generada por la IA. | El sistema registra la recomendación emitida. |
| El usuario acepta, rechaza o ignora la recomendación. | El sistema registra la interacción junto con la fecha y hora correspondientes. |
| La campaña continúa ejecutándose. | El sistema monitorea las métricas posteriores a la decisión tomada. |
| El usuario mantiene la operación normal del negocio. | El sistema compara el rendimiento antes y después de la recomendación aplicada. |
| Se obtiene suficiente información para evaluar resultados. | El sistema calcula el impacto generado sobre las métricas clave. |
| El usuario consulta el historial de recomendaciones. | El sistema presenta la evidencia del resultado obtenido. |
| El análisis finaliza. | El sistema utiliza los resultados históricos para ajustar y optimizar futuras recomendaciones. |

**Postcondición:** El impacto de la recomendación queda registrado y el conocimiento generado es incorporado al modelo de inteligencia artificial para futuras decisiones.

**Excepciones**

| Paso | Acción |
| --- | --- |
| El usuario no interactúa con la recomendación. | El sistema registra el evento como recomendación ignorada. |
| No existe suficiente tiempo o datos para medir el impacto. | El sistema informa que la evaluación aún no puede realizarse. |
| La información histórica se encuentra incompleta. | El sistema limita el análisis y notifica la situación al usuario. |
| Se detectan inconsistencias en los datos recopilados. | El sistema suspende temporalmente el proceso de aprendizaje y solicita una nueva sincronización. |

**Comentarios:** El aprendizaje debe considerar tanto el resultado obtenido como el comportamiento del usuario frente a las recomendaciones. Las métricas evaluadas incluyen ROAS, CPA, CTR, conversiones, ingresos y rentabilidad general del negocio.

---

# 5. RF3: Creatividades desde el Rendimiento

## 5.1 Historias de Usuario

### HU3.1.1 — Registro de usuario en ROAX

| Campo | Contenido |
| --- | --- |
| **Título** | Registro de usuario en ROAX |
| **Historia** | Yo, como dueño de un e-commerce, quiero registrarme en ROAX con mis datos básicos, para poder acceder a la plataforma y comenzar a analizar mis campañas. |
| **Criterios de aceptación** | **Scenario 1: Registro exitoso con datos válidos**<br>**Given** el usuario se encuentra en la página de registro<br>**When** ingresa nombre, correo válido y contraseña segura<br>**Then** el sistema crea la cuenta y asigna un ID único.<br><br>**Scenario 2: Registro fallido por correo ya registrado**<br>**Given** el usuario se encuentra en la página de registro<br>**And** el correo ya existe en la base de datos<br>**When** intenta registrarse con ese correo<br>**Then** el sistema rechaza el registro y muestra "El correo ya está registrado". |

---

### HU3.1.2 — Asignación de rol organizacional

| Campo | Contenido |
| --- | --- |
| **Título** | Asignación de rol organizacional |
| **Historia** | Yo, como administrador de una organización en ROAX, quiero asignar roles a los usuarios del equipo, para controlar qué funcionalidades pueden usar. |
| **Criterios de aceptación** | **Scenario 1: Asignación exitosa de rol**<br>**Given** el administrador está en la sección de gestión de usuarios<br>**When** asigna un rol válido a un usuario<br>**Then** el sistema guarda el rol y aplica los permisos correspondientes.<br><br>**Scenario 2: Asignación fallida por rol inválido**<br>**Given** el administrador está en la sección de gestión de usuarios<br>**When** asigna un rol que no existe en el sistema<br>**Then** el sistema rechaza la acción y muestra "Rol no válido". |

---

### HU4.1.1 — Consulta de perfil 360° del consumidor

| Campo | Contenido |
| --- | --- |
| **Título** | Consulta de perfil 360° del consumidor |
| **Historia** | Yo, como Marketing Manager, quiero consultar un perfil único de cada consumidor, para entender su comportamiento real de compra y segmentarlo mejor. |
| **Criterios de aceptación** | **Scenario 1: Consulta de perfil con historial completo**<br>**Given** existe un consumidor registrado con historial de compras y datos demográficos<br>**When** el Marketing Manager busca el perfil por ID o correo<br>**Then** el sistema muestra el perfil 360° con datos históricos consolidados.<br><br>**Scenario 2: Perfil no encontrado**<br>**Given** el Marketing Manager busca un consumidor por ID o correo<br>**But** el ID o correo no existe en la base de datos<br>**When** realiza la búsqueda<br>**Then** el sistema muestra "Perfil no encontrado". |

---

### HU5.D — Propuesta de creatividad mejorada basada en historial

| Campo | Contenido |
| --- | --- |
| **Título** | Propuesta de creatividad mejorada basada en historial |
| **Historia** | Yo, como dueño de e-commerce, quiero recibir propuestas de nuevas creatividades basadas en anuncios exitosos, para mejorar mis campañas sin depender únicamente de prueba y error. |
| **Criterios de aceptación** | **Scenario 1: Propuesta generada con historial suficiente**<br>**Given** existen creatividades históricas con datos de rendimiento registrados<br>**When** el usuario solicita una propuesta de creatividad mejorada<br>**Then** el sistema genera la propuesta y muestra un score de rendimiento esperado.<br><br>**Scenario 2: Propuesta fallida por falta de historial**<br>**Given** el usuario solicita una propuesta de creatividad mejorada<br>**But** no existen suficientes creatividades históricas para comparación<br>**When** el sistema intenta generar la propuesta<br>**Then** el sistema muestra "No hay suficientes datos históricos para generar propuestas". |

---

### HU7.1.1 — Conexión con plataforma externa mediante API

| Campo | Contenido |
| --- | --- |
| **Título** | Conexión con plataforma externa mediante API |
| **Historia** | Yo, como usuario de ROAX, quiero conectar mi cuenta con plataformas externas como Meta Ads, Shopify o Dropi, para que el sistema obtenga automáticamente datos de campañas y ventas reales. |
| **Criterios de aceptación** | **Scenario 1: Conexión exitosa con plataforma externa**<br>**Given** el usuario se encuentra en el módulo de integraciones<br>**When** autoriza el acceso mediante credenciales válidas (OAuth)<br>**Then** el sistema confirma la conexión y comienza la sincronización automática.<br><br>**Scenario 2: Conexión fallida por autorización denegada**<br>**Given** el usuario se encuentra en el módulo de integraciones<br>**When** rechaza permisos o la plataforma externa retorna error de autenticación<br>**Then** el sistema muestra "No fue posible conectar la cuenta". |

---

## 5.2 Casos de Uso

### 5.2.1 Diagramas de Casos de Uso

#### Subsistema A — Gestión de Usuarios
<img width="1421" height="762" alt="Diagrama Subsistema A" src="https://github.com/user-attachments/assets/ca2a671d-0f5e-49b3-af80-97151619465c" />

#### Subsistema E — Integración de APIs Externas
<img width="981" height="589" alt="Diagrama Subsistema E" src="https://github.com/user-attachments/assets/f059d78f-2bbd-4fb7-92ab-675903f04064" />

### 5.2.2 Formatos Bicolumnares

[Formato Bicolumnar — Subsistema A (CU-A-01 / CU-A-02)](https://github.com/user-attachments/files/28204607/Formato.Bicolumnar.Diagrama.A_ID.CU-A-0_CU-A-02.pdf)

[Formato Bicolumnar — Subsistema E (UC7.2.3)](https://github.com/user-attachments/files/28204154/Formato.Bicolumnar.v1.0_Subsitema.E_ID.UC7.2.3.pdf)

[Formato Bicolumnar — Subsistema E (UC7.2.4)](https://github.com/user-attachments/files/28204158/Formato.Bicolumnar.v1.0_Subsistema.E_ID.UC7.2.4.pdf)

---

# 6. RF4: Confianza Progresiva

## 6.1 Historias de Usuario

### RF13 — Agente Conversacional Visual (ACV)

| **Campo** | **Descripción** |
| --- | --- |
| **Título** | Interacción con el agente de IA |
| **Yo, como** | usuario de ROAX (emprendedor o gestor de e-commerce) |
| **Quiero** | comunicarme con un agente de IA mediante voz o texto que me muestre su avatar en pantalla |
| **Para** | entender mis métricas y recomendaciones sin necesidad de interpretar dashboards complejos |

**Scenario 1**

| | |
| --- | --- |
| **Given** | el usuario accede a la plataforma |
| **When** | el agente se carga |
| **Then** | el sistema muestra el avatar, reproduce un saludo e informa que el agente es IA |

**Scenario 2**

| | |
| --- | --- |
| **Given** | el usuario envía un mensaje |
| **When** | el agente procesa la consulta |
| **Then** | responde en lenguaje natural mostrando texto de forma simultánea independientemente del canal de voz |

**Scenario 3**

| | |
| --- | --- |
| **Given** | el usuario desactiva el audio |
| **When** | hace clic en el botón de configuración |
| **Then** | el agente continúa respondiendo solo con texto sin perder funcionalidad |

---

### RF14 — Recomendaciones Inteligentes (REC)

| **Campo** | **Descripción** |
| --- | --- |
| **Título** | Recibir y actuar sobre recomendaciones de campañas |
| **Yo, como** | usuario de ROAX con campañas activas en Meta Ads |
| **Quiero** | recibir recomendaciones claras sobre qué hacer con mis campañas, con su justificación y estimación de impacto |
| **Para** | tomar decisiones informadas sin necesidad de ser experto en métricas publicitarias |

**Scenario 1**

| | |
| --- | --- |
| **Given** | el sistema detecta una campaña con rendimiento por debajo del umbral de la industria |
| **When** | genera la recomendación |
| **Then** | muestra una tarjeta con la acción sugerida en lenguaje simple, la justificación y el impacto estimado |

**Scenario 2**

| | |
| --- | --- |
| **Given** | el usuario revisa una recomendación |
| **When** | hace clic en Aplicar |
| **Then** | el sistema ejecuta la acción y comienza el seguimiento del impacto real versus el estimado |

**Scenario 3**

| | |
| --- | --- |
| **Given** | el usuario rechaza una recomendación |
| **When** | selecciona un motivo |
| **Then** | el sistema registra el rechazo, ajusta el enfoque y continúa generando recomendaciones |

---

### RF15 — Gestión de Alertas (ALR)

| **Campo** | **Descripción** |
| --- | --- |
| **Título** | Recibir alertas críticas sin saturación |
| **Yo, como** | usuario de ROAX con campañas activas fuera del horario laboral |
| **Quiero** | recibir alertas priorizadas sobre situaciones críticas en tiempo real |
| **Para** | actuar rápido sin ahogarme en notificaciones irrelevantes |

**Scenario 1**

| | |
| --- | --- |
| **Given** | el sistema detecta una campaña con gasto elevado sin conversiones |
| **When** | evalúa el impacto relativo al presupuesto del usuario |
| **Then** | envía una alerta crítica por el canal configurado con la situación y las opciones de acción |

**Scenario 2**

| | |
| --- | --- |
| **Given** | el usuario tiene múltiples campañas con indicadores fuera de rango |
| **When** | el sistema evalúa los indicadores en conjunto |
| **Then** | agrupa las alertas por criticidad y presenta un máximo configurable sin saturar al usuario |

**Scenario 3**

| | |
| --- | --- |
| **Given** | el usuario quiere configurar sus notificaciones |
| **When** | accede a la sección de alertas |
| **Then** | puede definir canales (in-app, correo, WhatsApp, push), horarios y nivel mínimo de criticidad |

---

### RF16 — Retroalimentación y Aprendizaje (RFA)

| **Campo** | **Descripción** |
| --- | --- |
| **Título** | Construir confianza progresiva con el agente |
| **Yo, como** | usuario de ROAX que usa las recomendaciones del sistema |
| **Quiero** | ver cómo el sistema aprende de mis decisiones y poder delegar autonomía gradualmente |
| **Para** | confiar en el sistema y permitirle actuar en mi nombre cuando esté fuera |

**Scenario 1**

| | |
| --- | --- |
| **Given** | el usuario ha aplicado varias recomendaciones con resultados positivos |
| **When** | el sistema calcula el nivel de confianza acumulada |
| **Then** | muestra el indicador actualizado y sugiere activar un nivel mayor de automatización |

**Scenario 2**

| | |
| --- | --- |
| **Given** | el usuario rechaza repetidamente un tipo de recomendación |
| **When** | el modelo procesa el patrón |
| **Then** | ajusta el enfoque de futuras recomendaciones sin dejar de recomendar |

**Scenario 3**

| | |
| --- | --- |
| **Given** | el usuario tiene activado el modo de automatización |
| **When** | el sistema va a ejecutar una acción automática |
| **Then** | verifica permisos, ejecuta la acción, notifica al usuario y le ofrece revertirla dentro de 24 horas |

---

## 6.2 Casos de Uso

### 6.2.1 Diagramas de Casos de Uso

#### Diagrama 01 — RF13: Agente Conversacional Visual
![Caso de uso 01-RF13](Imagenes/RF4-ConfianzaProgresiva/Caso%20de%20uso%2001.jpeg)

#### Diagrama 02 — RF13: Agente Conversacional Visual
![Caso de uso 02-RF13](Imagenes/RF4-ConfianzaProgresiva/Caso%20de%20uso%2002.jpeg)

#### Diagrama 01 — RF14: Recomendaciones Inteligentes
![Caso de uso 01-RF14](Imagenes/RF4-ConfianzaProgresiva/Caso%20de%20uso%2003.jpeg)

#### Diagrama 02 — RF14: Recomendaciones Inteligentes
![Caso de uso 02-RF14](Imagenes/RF4-ConfianzaProgresiva/Caso%20de%20uso%2004.jpeg)

#### Diagrama 01 — RF15: Gestión de Alertas
![Caso de uso 01-RF15](Imagenes/RF4-ConfianzaProgresiva/Caso%20de%20uso%2005.jpeg)

#### Diagrama 02 — RF15: Gestión de Alertas
![Caso de uso 02-RF15](Imagenes/RF4-ConfianzaProgresiva/Caso%20de%20uso%2006.jpeg)

#### Diagrama — RF16: Retroalimentación y Aprendizaje
![Caso de uso RF16](Imagenes/RF4-ConfianzaProgresiva/Caso%20de%20uso%2007.jpeg)

### 6.2.2 Formatos Bicolumnares

[Formato Bicolumnar 01 — RF13](https://docs.google.com/document/d/1TDo1TTdEj_wKEtHp9ctVsHX_yG9c6Bq6nMTPyKIl7fE/edit?usp=sharing)

[Formato Bicolumnar 02 — RF13](https://docs.google.com/document/d/1W9J1i2ecVRGP5G9hOKJs7YT8tL1P38t-gC1fvb_BG3k/edit?usp=sharing)

[Formato Bicolumnar 01 — RF14](https://docs.google.com/document/d/1XEnIszNS_L7ecwf0LtUeyBp6_ZerAuZBfnwhDKyjlcs/edit?usp=sharing)

[Formato Bicolumnar 02 — RF14](https://docs.google.com/document/d/1-K1FWEDIBLcpTYH0QG6UmPqgaPHUBNcKKdLmWMUeu2A/edit?usp=sharing)

[Formato Bicolumnar 01 — RF15](https://docs.google.com/document/d/1tnP73K3gOLi3lbml82Woqx60uFBn9MJfaYvp_luhMEg/edit?usp=sharing)

[Formato Bicolumnar 02 — RF15](https://docs.google.com/document/d/1JD7duImYBW1lOvTrh6khlGdWskXr-8m9sPR6lQ6Sl3E/edit?usp=sharing)

[Formato Bicolumnar 01 — RF16](https://docs.google.com/document/d/1iAuLzWd_MS7xk6nPBQ9Vc4ATOAfWvXaoF6ExM6D663c/edit?usp=sharing)

[Formato Bicolumnar 02 — RF16](https://docs.google.com/document/d/1XDNQ0x9D_c9VJY83ohNyv0WCq8bmWZJhL6SQxBMDttM/edit?usp=sharing)

---

# 7. Backlog

El backlog del proyecto consolida las funcionalidades principales identificadas durante la especificación de requerimientos. Estas historias se organizan según los cuatro subsistemas definidos para ROAX: Datos y Decisiones, Alertas que Razonan, Creatividades desde el Rendimiento y Confianza Progresiva.

| ID | Subsistema | Historia de Usuario | Prioridad |
| --- | --- | --- | :---: |
| HU-RF1-01 | Datos y Decisiones | Como usuario de ROAX, quiero visualizar la rentabilidad real de mis campañas para saber cuánto estoy ganando o perdiendo con base en datos de pauta y ventas reales. | Alta |
| HU-RF1-02 | Datos y Decisiones | Como usuario de ROAX, quiero detectar campañas deficitarias para actuar antes de seguir perdiendo presupuesto publicitario. | Alta |
| HU-RF1-03 | Datos y Decisiones | Como usuario de ROAX, quiero consultar métricas actualizadas de campañas, ventas y rendimiento para tomar decisiones basadas en información reciente. | Alta |
| HU-RF1-04 | Datos y Decisiones | Como administrador, quiero configurar reglas de automatización para que el sistema pueda ejecutar acciones bajo condiciones previamente definidas. | Media |
| HU-RF2-01 | Alertas que Razonan | Como usuario de ROAX, quiero recibir alertas predictivas con diagnóstico contextual para entender qué métrica está fallando y por qué ocurre el problema. | Alta |
| HU-RF2-02 | Alertas que Razonan | Como usuario de ROAX, quiero recibir recomendaciones inteligentes sobre campañas, presupuesto o creatividades para mejorar la rentabilidad del negocio. | Alta |
| HU-RF2-03 | Alertas que Razonan | Como usuario de ROAX, quiero aplicar recomendaciones desde la alerta mediante acciones directas para optimizar campañas sin hacer ajustes manuales complejos. | Alta |
| HU-RF2-04 | Alertas que Razonan | Como usuario de ROAX, quiero configurar límites para que la IA tome decisiones autónomas solo dentro de reglas permitidas. | Media |
| HU-RF2-05 | Alertas que Razonan | Como usuario de ROAX, quiero que el sistema aprenda de mis decisiones e interacciones para recibir recomendaciones más precisas con el tiempo. | Media |
| HU-RF3-01 | Creatividades desde el Rendimiento | Como usuario de ROAX, quiero registrar y gestionar usuarios dentro de la plataforma para controlar el acceso al sistema. | Alta |
| HU-RF3-02 | Creatividades desde el Rendimiento | Como usuario de ROAX, quiero consultar perfiles consolidados de consumidores para comprender mejor el comportamiento de compra. | Media |
| HU-RF3-03 | Creatividades desde el Rendimiento | Como usuario de ROAX, quiero generar reportes financieros y operativos para conocer el estado general del negocio. | Alta |
| HU-RF3-04 | Creatividades desde el Rendimiento | Como usuario de ROAX, quiero analizar el rendimiento de creatividades publicitarias para identificar qué anuncios funcionan mejor. | Alta |
| HU-RF3-05 | Creatividades desde el Rendimiento | Como usuario de ROAX, quiero recibir propuestas automáticas de nuevas creatividades basadas en el rendimiento histórico para mejorar mis campañas. | Media |
| HU-RF3-06 | Creatividades desde el Rendimiento | Como usuario de ROAX, quiero conectar plataformas externas mediante APIs para integrar datos de pauta, ventas e inventario. | Alta |
| HU-RF4-01 | Confianza Progresiva | Como usuario de ROAX, quiero interactuar con un agente conversacional de IA para entender recomendaciones y métricas sin depender únicamente de dashboards. | Media |
| HU-RF4-02 | Confianza Progresiva | Como usuario de ROAX, quiero recibir recomendaciones explicadas con datos para comprender por qué la IA sugiere una acción. | Alta |
| HU-RF4-03 | Confianza Progresiva | Como usuario de ROAX, quiero recibir alertas críticas priorizadas para actuar rápido sin saturarme de notificaciones. | Alta |
| HU-RF4-04 | Confianza Progresiva | Como usuario de ROAX, quiero calificar o responder a las recomendaciones para que el sistema aprenda de mis decisiones. | Media |
| HU-RF4-05 | Confianza Progresiva | Como usuario de ROAX, quiero visualizar un nivel de confianza acumulada para decidir gradualmente qué acciones puedo delegar a la IA. | Media |

---

# 8. MockUp

## 8.1 Descripción General

El mockup del proyecto presenta una propuesta visual del MVP de ROAX, integrando las funcionalidades principales definidas en los requerimientos y casos de uso de los cuatro subsistemas trabajados.

La propuesta busca representar una plataforma unificada de inteligencia de negocio para e-commerce, donde el usuario pueda consultar métricas de rendimiento, recibir alertas inteligentes, revisar recomendaciones generadas por IA, analizar creatividades publicitarias y gestionar progresivamente la confianza en las acciones automatizadas del sistema.

El diseño del mockup se construye a partir de la identidad visual de ROAX y mantiene una estructura orientada a dashboard, con navegación lateral, módulos funcionales, tarjetas de información, visualización de métricas, alertas priorizadas y acciones rápidas. Su objetivo es mostrar cómo las funcionalidades especificadas pueden integrarse en una experiencia coherente, clara y accionable para el usuario final.

## 8.2 Enlace MockUp en Figma

> https://www.figma.com/design/HMZFeHdNOGGJ8SEmHM0CQI/Prototipo---Roax?node-id=0-1&t=qTohZvM0j3k5Ur9a-1