# DOCUMENTO DE ESPECIFICACIÓN DE REQUERIMIENTOS

## ROAX

---

**INTEGRANTES**

###Equipo Reto 1 - Datos y Decisiones

-

###Equipo Reto 2 - Alertas que razonan

- David Altaminaro Altamirano
- Mariana Carmona Galvez
- Santiago Campo
- David Santiago García
- Mario Andrés Romero Rivera
- Andrés Vinasco

###Equipo Reto 3 - Creatividades desde el rendimiento

-

###Equipo Reto 4 - Confianza progresiva

- Melisa Gomez Gomez
- Samuel Alejandro Estupiñan Gonzales
- Jorge Humberto Garcia Leon
- Juan Camilo Borrero Florez
- Juan Pablo Urbina Ladino
- Matius Montealegre Padilla

---

# Tabla de Contenido

1. Especificación de Requerimientos
   1.1 Descripción General
   1.2 Contexto del Proyecto
   1.3 Requisitos
      1.3.1 Subsistema de Datos y Decisiones
      1.3.2 Subsistema de Alertas que razonan
      1.3.3 Subsistema de Creatividades desde el rendimiento
      1.3.4 Subsistema de Confianza Progresiva

   1.4 Subespecificación por Subsistemas
      1.4.1 RF1: Datos y Decisiones
      1.4.2 RF2: Alertas que razonan
      1.4.3 RF3: Creatividades desde el rendimiento
      1.4.4 RF4: Confianza Progresiva

   1.5 Tabla de Asignación a Subsistemas

2. PESTLE
      2.1 RF1: Datos y Decisiones
      2.2 RF2: Alertas que razonan
      2.3 RF3: Creatividades desde el rendimiento
      2.4 RF4: Confianza Progresiva

3. RF1: Datos y Decisiones
   3.1 Historias de Usuario
   3.2 Casos de Uso
      3.2.1 Diagrama de Casos de Uso
      3.2.2 Formatos Bicolumnares

4. RF2: Alertas Inteligentes
   4.1 Historias de Usuario
   4.2 Casos de Uso
      4.2.1 Diagrama de Casos de Uso
      4.2.2 Formatos Bicolumnares

5. RF3: Inteligencia Creativa
   5.1 Historias de Usuario
   5.2 Casos de Uso
      5.2.1 Diagrama de Casos de Uso
      5.2.2 Formatos Bicolumnares

6. RF4: Confianza Progresiva
   6.1 Historias de Usuario
   6.2 Casos de Uso
      6.2.1 Diagrama de Casos de Uso
      6.2.2 Formatos Bicolumnares

7. Backlog

8. MockUp
   8.1 Descripción General
   8.2 Enlace MockUp

---

# 1. Especificación de Requerimientos

## 1.1 Descripción General

En esta sección se describen y analizan los requerimientos del proyecto ROAX Refactor 2026, una plataforma de inteligencia de negocio orientada a e-commerce que busca transformar la manera en que los usuarios interpretan, analizan y ejecutan decisiones relacionadas con sus campañas de marketing digital y desempeño comercial.

Actualmente, ROAX integra múltiples fuentes de datos provenientes de plataformas como Meta Ads, Shopify, Dropi y otros entornos de comercio electrónico, permitiendo visualizar métricas relacionadas con rentabilidad, conversión y rendimiento publicitario. Sin embargo, el sistema actual se centra principalmente en la visualización de información, dejando en manos del usuario la interpretación de los datos y la toma de decisiones estratégicas.

El objetivo de este proyecto es rediseñar la plataforma para convertir la inteligencia artificial en el núcleo operativo del sistema, permitiendo no solo visualizar datos, sino también analizar comportamientos, generar recomendaciones, contextualizar alertas, sugerir acciones concretas y fortalecer progresivamente la confianza del usuario en las decisiones automatizadas.

La solución propuesta se divide en cuatro subsistemas principales: Datos y Decisiones, Alertas Inteligentes, Inteligencia Creativa y Confianza Progresiva. Cada uno de estos componentes busca abordar distintos retos relacionados con automatización, interpretación de datos, generación de recomendaciones y aprendizaje continuo del comportamiento del negocio.

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

---

### 1.3.2 Subsistema de Alertas que razonan

#### RF1. El sistema debe mostrar al usuario las campañas cuyo desempeño se encuentre por debajo de un umbral definido.
   
#### RF2. El sistema generará recomendaciones inteligentes basadas en losresultados del negocio

#### RF3. El sistema debe medir, analizar y aprender del impacto de las decisiones tomadas en campañas publicitarias y resultados del negocio.

#### RF4. El sistema debe construir confianza progresiva en las recomendaciones generadas por IA

---

### 1.3.3 Subsistema de Creatividades desde el rendimiento

---

### 1.3.4 Subsistema de Confianza Progresiva

### Requerimientos Funcionales

| **RF** | **Descripción** |
| --- | --- |
| **RF13** | El sistema debe permitir la comunicación con el usuario mediante un agente conversacional visual en tiempo real |
| **RF14** | El sistema debe generar y presentar recomendaciones inteligentes sobre campañas publicitarias basadas en análisis de datos y comportamiento histórico |
| **RF15** | El sistema debe gestionar alertas priorizadas sobre indicadores críticos del negocio evitando la saturación de información al usuario |
| **RF16** | El sistema debe gestionar la retroalimentación del usuario y ajustar progresivamente sus recomendaciones para construir confianza progresiva |

### Requerimientos No Funcionales

| **RNF** | **Descripción** |
| --- | --- |
| **RNF1** | **Disponibilidad:** el sistema debe estar disponible 24/7 para monitoreo continuo de campañas |
| **RNF2** | **Procesamiento en tiempo real:** el sistema debe procesar y analizar datos con mínima latencia |
| **RNF3** | **Interfaz de usuario:** el sistema debe ofrecer una interfaz intuitiva, clara y orientada a la toma de decisiones |
| **RNF4** | **Portabilidad:** el sistema debe ser accesible desde múltiples dispositivos incluyendo móviles |
| **RNF5** | **Interacción por voz:** el sistema debe permitir interacción mediante audio procesando comandos en tiempo real |
| **RNF6** | **Transparencia IA:** el sistema debe hacer visible cuando una recomendación es generada por inteligencia artificial |
| **RNF7** | **Escalabilidad:** el sistema debe gestionar el consumo de recursos según el plan de suscripción del usuario |

---

## 1.4 Subespecificación por Subsistemas

   ###1.4.1 RF1: Datos y Decisiones
   
   ---
   
   ###1.4.2 RF2: Alertas que razonan
   
   #### RF1. El sistema debe mostrar al usuario las campañas cuyo desempeño se encuentre por debajo de un umbral definido.
   
- **RF1.1.** El sistema debe calcular el desempeño de cada campaña utilizando métricas cuantificables definidas (por ejemplo: tasa de conversión, CTR, ROI) y compararlas contra un umbral configurado.
   
- **RF1.2** El sistema debe permitir al usuario definir y modificar los umbrales de desempeño mediante valores numéricos o porcentuales para cada métrica.
   
- RF1.3 El sistema debe permitir al usuario seleccionar las métricas que serán utilizadas para evaluar el desempeño de las campañas.

#### RF2. El sistema generará recomendaciones inteligentes basadas en losresultados del negocio
- **RF 2.1** El asistente sugerirá cambios en el dinero invertido diariamente en cada campaña publicitaria. Esto lo hará analizando si la inversión actual está generando ventas reales o si se está perdiendo dinero.
  
- **RF 2.2** El sistema de recomendaciones propondrá cambiar las imágenes o videos que no están funcionando por anuncios nuevos creados con la inteligencia artificial de la plataforma. El sistema elegirá los diseños que tienen más probabilidades de atraer clientes basándose en los gustos del público y en las ventas que ya se han logrado anteriormente.
  
- **RF 2.3** La pantalla de alertas incluirá un botón para aplicar las mejoras sugeridas al instante y sin complicaciones. Al presionarlo, el sistema realizará los cambios automáticamente en las cuentas de publicidad y ventas del usuario, ahorrando tiempo y asegurando que las decisiones se tomen rápido.

#### RF3. El sistema debe medir, analizar y aprender del impacto de las decisiones tomadas en campañas publicitarias y resultados del negocio.

- **RF3.1** El sistema debe registrar las acciones tomadas manualmente por el usuario o ejecutadas automáticamente a partir de recomendaciones inteligentes generadas por la plataforma.

- **RF3.2** El sistema debe evaluar el impacto de las acciones realizadas utilizando métricas clave del negocio y de publicidad digital, como ROAS, CTR, CPC, conversiones, compras, facturación, alcance, impresiones, clicks, video views, porcentaje de visualización completa de videos, add to cart y conversion rate.

- **RF3.3** El sistema debe almacenar información histórica diaria y mensual para identificar cambios de comportamiento, tendencias y resultados derivados de las decisiones tomadas.

- **RF3.4** El sistema debe estructurar el análisis de datos siguiendo la jerarquía de las plataformas publicitarias: Business Manager (BM), cuentas publicitarias, campañas, conjuntos de anuncios y anuncios.

- **RF3.5** El sistema debe permitir analizar el rendimiento de campañas y anuncios en cada nivel de la jerarquía publicitaria para identificar qué elemento está afectando positiva o negativamente el desempeño del negocio.

- **RF3.6** El sistema debe relacionar las métricas publicitarias con las métricas reales de ventas provenientes de tiendas integradas como Shopify, Dropi, WooCommerce o Tienda Nube.

- **RF3.7** El sistema debe permitir realizar seguimiento del recorrido del usuario consumidor final dentro del embudo de conversión, relacionando eventos como impresiones, clicks, visitas a la página, add to cart y compras realizadas, con el fin de identificar puntos de pérdida dentro del proceso de venta.

- **RF3.8** El sistema debe relacionar las compras realizadas con la tienda correspondiente y con las campañas publicitarias asociadas para medir el impacto real de cada anuncio sobre las ventas.

- **RF3.9** El sistema debe calcular métricas de conversión y relación entre interacción y ventas, incluyendo conversion rate, relación click/ventas, costo por conversión y calidad de tráfico, para evaluar la efectividad de las campañas.

- **RF3.10** El sistema debe analizar la calidad de la página de destino y su influencia en el rendimiento de campañas y conversiones del negocio.

- **RF3.11** El sistema debe permitir personalizar el análisis y las recomendaciones según las necesidades específicas del negocio y las métricas relevantes para cada usuario.

- **RF3.12** El sistema debe utilizar un agente inteligente personalizado basado en el contexto, historial y comportamiento del negocio, evitando respuestas o recomendaciones genéricas.

- **RF3.13** El sistema debe diferenciar entre distintos modelos de negocio, como dropshipping y marcas propias, para adaptar las recomendaciones, métricas prioritarias y análisis de rendimiento.

- **RF3.14** El sistema debe detectar comportamientos anormales o riesgos asociados a baneos y restricciones en cuentas publicitarias, generando alertas preventivas.

- **RF3.15** El sistema debe utilizar el historial de comportamiento del negocio para construir un perfil inteligente del usuario y mejorar continuamente la toma de decisiones automatizadas.
  
#### RF4. El sistema debe construir confianza progresiva en las recomendaciones generadas por IA

- **RF4.1** El sistema debe presentar las recomendaciones acompañadas de una justificación explicable, indicando qué métricas del negocio motivaron la sugerencia (por ejemplo: "Se recomienda pausar esta campaña porque su ROAS lleva 3 días por debajo de tu umbral configurado y ha generado pérdida neta de $X").

- **RF4.2** El sistema debe clasificar cada recomendación según un nivel de confianza calculado, basado en la cantidad de datos históricos disponibles del negocio del usuario y en el historial de aciertos de recomendaciones previas similares.

- **RF4.3** El sistema debe permitir que el usuario ejecute las recomendaciones de forma gradual, ofreciendo opciones escalonadas (por ejemplo: aplicar cambio parcial, programar para mañana, o aplicar de inmediato), reduciendo la fricción de adopción sin eliminar el control del usuario.

- **RF4.4** El sistema debe registrar si el usuario aceptó, rechazó o ignoró cada recomendación, y en qué tiempo lo hizo, para construir un perfil de adopción que permita personalizar cómo y cuándo se presentan futuras recomendaciones.

- **RF4.5** El sistema debe mostrar, posterior a la ejecución de una recomendación, un resumen del impacto real medido (comparando métricas antes y después), cerrando el ciclo de confianza con evidencia concreta del resultado.

   
   ---
   
   ###1.4.3 RF3: Creatividades desde el rendimiento
   
   ---
   
   ###1.4.4 RF4: Confianza Progresiva

#### RF13 — Agente Conversacional Visual (ACV)

| **ID** | **Subrequerimiento** |
| --- | --- |
| **ACV R13.1** | El sistema debe mostrar el avatar visual del agente mediante una ventana fija en la interfaz principal de la plataforma |
| **ACV R13.2** | El sistema debe reproducir la voz del agente mediante síntesis de voz clonada de actriz al momento de emitir una recomendación o alerta |
| **ACV R13.3** | El sistema debe mostrar el texto de la respuesta en un panel de conversación junto al avatar para usuarios que prefieran leer |
| **ACV R13.4** | El sistema debe permitir al usuario enviar mensajes al agente mediante un campo de texto o por entrada de voz |
| **ACV R13.5** | El sistema debe responder al usuario en lenguaje natural evitando tecnicismos innecesarios mediante el procesamiento del LLM |
| **ACV R13.6** | El sistema debe permitir al usuario activar o desactivar la voz del agente mediante un botón de configuración en la interfaz |

---

#### RF14 — Recomendaciones Inteligentes (REC)

| **ID** | **Subrequerimiento** |
| --- | --- |
| **REC R14.1** | El sistema debe identificar automáticamente campañas con bajo rendimiento mediante el análisis de métricas como ROAS, CPA, CTR y comportamiento histórico |
| **REC R14.2** | El sistema debe presentar cada recomendación en una tarjeta de acción que incluya la acción sugerida, la explicación basada en datos y la estimación de impacto esperado |
| **REC R14.3** | El sistema debe permitir al usuario interactuar con cada recomendación mediante tres opciones: Aplicar, Rechazar o Posponer, mostradas como botones diferenciados en la interfaz |
| **REC R14.4** | El sistema debe permitir al usuario expandir cada recomendación para acceder a una vista detallada con gráficas de evolución temporal y análisis del embudo de conversión |
| **REC R14.5** | El sistema debe solicitar y almacenar información cualitativa del negocio (inventario disponible, costos fijos, perfil del cliente) mediante un formulario de onboarding para mejorar la precisión de las recomendaciones |
| **REC R14.6** | El sistema debe mostrar, posterior a la aplicación de una recomendación, un seguimiento del impacto real versus el impacto estimado en formato antes/después con métricas en valores monetarios y porcentajes |

---

#### RF15 — Gestión de Alertas (ALR)

| **ID** | **Subrequerimiento** |
| --- | --- |
| **ALR R15.1** | El sistema debe enviar notificaciones inmediatas al usuario cuando detecte una campaña en situación crítica, priorizando aquellas con mayor impacto económico potencial |
| **ALR R15.2** | El sistema debe agrupar y priorizar las alertas según su impacto potencial mediante un sistema de pesos por indicador, mostrando un máximo de alertas críticas por sesión |
| **ALR R15.3** | El sistema debe analizar indicadores en conjunto (CTR + CPA + CBR) en lugar de dispararlos individualmente, para evitar la saturación de alertas al usuario |
| **ALR R15.4** | El sistema debe permitir al usuario configurar sus preferencias de notificación incluyendo canales (in-app, correo, WhatsApp, push móvil), horarios de envío y nivel de criticidad mínimo |

---

#### RF16 — Retroalimentación y Aprendizaje (RFA)

| **ID** | **Subrequerimiento** |
| --- | --- |
| **RFA R16.1** | El sistema debe presentar al usuario un mecanismo de retroalimentación explícita que le permita calificar la utilidad de cada recomendación (útil, incorrecta, irrelevante) con comentario opcional |
| **RFA R16.2** | El sistema debe registrar retroalimentación implícita derivada del comportamiento del usuario: frecuencia de aceptación, tiempo antes de actuar, recomendaciones ignoradas y acciones revertidas |
| **RFA R16.3** | El sistema debe continuar generando recomendaciones aunque el usuario las rechace de forma repetida, ajustando el tipo y enfoque de las sugerencias según el patrón detectado |
| **RFA R16.4** | El sistema debe permitir al usuario configurar niveles de automatización desde recomendaciones manuales hasta ejecución automática de acciones según su preferencia y nivel de confianza acumulada |
| **RFA R16.5** | El sistema debe mostrar al usuario un indicador de nivel de confianza acumulada con el agente de IA, reflejando el historial de recomendaciones aceptadas y sus resultados medibles |

---

## 1.5 Tabla de Asignación a Subsistemas

| **Requerimiento** | **RF13 - ACV** | **RF14 - REC** | **RF15 - ALR** | **RF16 - RFA** |
| --- | :---: | :---: | :---: | :---: |
| Agente conversacional visual | X | | | |
| Síntesis de voz clonada | X | | | |
| Identificación de campañas | | X | | |
| Tarjetas de recomendación | | X | | |
| Opciones aplicar/rechazar/posponer | | X | | |
| Datos cualitativos del negocio | | X | | |
| Alertas priorizadas | | | X | |
| Sistema de pesos de indicadores | | | X | |
| Configuración de notificaciones | | | X | |
| Retroalimentación explícita | | | | X |
| Aprendizaje por comportamiento | | | | X |
| Niveles de automatización | | | | X |
| Indicador de confianza acumulada | | | | X |


# 2. PESTLE

> El análisis PESTLE se aplica a los requerimientos funcionales que toman decisiones sobre personas, usan datos sensibles o pueden generar impacto negativo. Para cada dimensión se identifica el hallazgo verificado, su impacto real y el requerimiento derivado.


   ###2.1 RF1: Datos y Decisiones
   
   ---
   
   ###2.2 RF2: Alertas que razonan
   
   ## Análisis PESTLE – RF1: Detección de campañas de bajo desempeño

| Dimensión | Hallazgo | Impacto | Requerimiento derivado |
|----------|----------|---------|-------------------------|
| P — Político | No existen lineamientos específicos en Colombia sobre transparencia en algoritmos que evalúan desempeño de campañas. | El sistema podría ser cuestionado si no justifica cómo clasifica una campaña como de bajo desempeño. | **RNFP-1-01:** El sistema debe permitir consultar las métricas, umbrales y reglas utilizadas para clasificar una campaña como de bajo desempeño, mostrando al menos: nombre de la métrica, valor calculado, umbral aplicado y resultado de la evaluación. |
| E — Económico | El cálculo frecuente de métricas sobre grandes volúmenes de campañas implica alto costo computacional. | Puede afectar la escalabilidad y costos operativos del sistema. | **RNFE-1-02:** El sistema debe calcular métricas de desempeño mediante procesamiento incremental o por lotes, reduciendo en al menos un 30% el tiempo de procesamiento respecto a un cálculo completo sobre todos los datos históricos. |
| S — Social | Usuarios no expertos pueden no comprender métricas como CTR, ROI o tasa de conversión. | Riesgo de mala interpretación del desempeño de campañas. | **RNFS-1-03:** El sistema debe mostrar una descripción textual comprensible (máximo 100 palabras) para cada métrica utilizada, accesible desde la interfaz de evaluación de campañas. |
| T — Tecnológico | La evaluación depende de la actualización oportuna de datos de campañas. | Datos desactualizados generan clasificaciones incorrectas. | **RNFT-1-04:** El sistema debe actualizar las métricas de desempeño de campañas con una latencia máxima de 5 minutos desde la recepción de nuevos datos, garantizando que al menos el 95% de las actualizaciones cumplan este límite. |
| L — Legal | El sistema maneja datos sensibles de negocio asociados a campañas. | Riesgo de incumplimiento de normativas de protección de datos. | **RNFL-1-05:** El sistema debe restringir el acceso a la información de desempeño de campañas mediante control de roles, garantizando que solo usuarios autorizados puedan visualizar o modificar dichos datos. |
| E — Ético | La clasificación automática influye en decisiones comerciales del usuario. | Clasificaciones poco transparentes pueden inducir decisiones erróneas. | **RNFEt-1-06:** El sistema debe indicar explícitamente si la clasificación de bajo desempeño fue generada por reglas del sistema o configuraciones del usuario, mostrando esta información en la vista de resultados de cada campaña. |

# Análisis PESTLE - RF2: sistema generará recomendaciones inteligentes basadas en los resultados del negocio 

| Dimensión | Hallazgo | Impacto | Requerimiento derivado |
|-----------|----------|---------|-------------------------|
| **P — Político** | Las plataformas como Meta y TikTok pueden cambiar sus reglas sobre cómo se permite ajustar presupuestos o publicar anuncios automáticamente. | Si Meta decide restringir la automatización, ROAX perdería la capacidad de aplicar cambios instantáneos (RF 2.3), y el usuario tendría que volver a hacer todo manualmente. | El sistema debe anticipar estos cambios mostrando una alerta al usuario del tipo “Meta cambió sus reglas, por ahora solo podemos sugerir, no aplicar automáticamente”. Así el usuario no se frustra y confía en que ROAX está al día. |
| **E — Económico** | Analizar si cada campaña está quemando dinero o generando ventas reales (RF 2.1) requiere procesar muchos datos históricos. |  la plataforma sería cara de mantener y el precio para el usuario final tendría que aumentar. | El sistema debe priorizar el análisis solo en campañas que más invierten y ajustar cada 4 horas, no en tiempo real. Así se reduce costo sin perder efectividad. |
| **S — Social** | Muchos usuarios de ROAX son dropshippers o pequeños empresarios, no expertos en marketing. Si ven una recomendación de “cambiar inversión” sin entender el porqué, pueden ignorarla o aplicarla mal. | El usuario termina tomando malas decisiones o no usa la función por miedo. El problema que resuelve ROAX (falta de acción) no se soluciona. | El sistema debe explicar cada recomendación en una frase simple, como: “Esta campaña gastó 100.000 $ y solo vendió 30.000 $. Te sugiero bajar la inversión a 50.000 $ diarios”. Así el usuario entiende antes de aceptar. |
| **T — Tecnológico** | ROAX ya genera anuncios con IA, pero conectarlos con datos reales de venta para que aprenda de lo que ya convierte (RF 2.2) es complejo. | Si la IA propone creatividades bonitas pero que no venden, el usuario pierde confianza rápidamente y deja de usar la función. | El sistema debe etiquetar cada creatividad generada con una predicción simple: “Alta probabilidad de venta”, “Media”, “Baja” basada en anuncios anteriores que sí funcionaron. El usuario decide si probarla. |
| **L — Legal** | El sistema puede llegar a pausar campañas o redistribuir presupuesto automáticamente (RF 2.3) basado en rentabilidad. Si lo hace mal, el usuario pierde ventas reales. | ROAX podría ser demandado o perder muchos usuarios por mala publicidad. La confianza se rompe. | La plataforma debe pedir un consentimiento explícito al inicio: "Autorizo a ROAX a hacer cambios automáticos hasta por un límite de $X diarios". Además, cada acción debe poder deshacerse con un botón "Reversar cambio". |
| **E — Ético** | El sistema decide qué algunas recomendaciones "no están funcionando" (RF 2.2) basándose en ventas pasadas. Eso puede dejar fuera a nuevos diseños que con más tiempo sí funcionarían. | El usuario puede terminar viendo siempre el mismo tipo de anuncio, saturando a su audiencia y sin explorar nuevas ideas. | El sistema debe reservar un pequeño porcentaje del presupuesto para probar creatividades nuevas sin que la IA las descarte de entrada. Y mostrar un mensaje: "Probamos algo nuevo por si te funciona". |

> **RF3.** El sistema debe medir, analizar y aprender del impacto de las decisiones tomadas en campañas publicitarias y resultados del negocio.

| Dimensión | Hallazgo | Impacto | Requerimiento derivado |
|----------|----------|---------|-------------------------|
| **P — Político** | Las plataformas publicitarias (Meta Ads, TikTok Ads, Google Ads) pueden cambiar políticas o restricciones sobre acceso y uso de datos analíticos. | Cambios externos podrían afectar la continuidad del análisis y aprendizaje del sistema. | **RNFP-3-01:** El sistema debe registrar y notificar cambios en la disponibilidad de datos provenientes de plataformas publicitarias integradas, indicando el servicio afectado y el impacto sobre los análisis generados. |
| **E — Económico** | El procesamiento continuo de métricas históricas, embudos y relaciones entre campañas y ventas implica alto consumo computacional y almacenamiento. | Incremento de costos operativos y riesgo de baja escalabilidad. | **RNFE-3-02:** El sistema debe optimizar el almacenamiento y procesamiento histórico utilizando consolidación incremental de datos diarios y mensuales, reduciendo en al menos un 25% el consumo de recursos respecto a un procesamiento completo continuo. |
| **S — Social** | Usuarios con distintos niveles de experiencia pueden interpretar incorrectamente métricas complejas como ROAS, conversion rate o calidad de tráfico. | Riesgo de tomar decisiones comerciales equivocadas. | **RNFS-3-03:** El sistema debe proporcionar explicaciones contextuales y descripciones comprensibles para cada métrica y recomendación mostrada, utilizando textos de máximo 120 palabras accesibles desde la interfaz de análisis. |
| **T — Tecnológico** | El sistema depende de integración constante con múltiples plataformas externas (Shopify, WooCommerce, Meta Ads, TikTok Ads, etc.). | Fallas de sincronización pueden generar análisis incorrectos o incompletos. | **RNFT-3-04:** El sistema debe sincronizar datos provenientes de plataformas integradas con una disponibilidad mínima del 99% mensual y una latencia máxima de 10 minutos para actualizaciones críticas de métricas y conversiones. |
| **L — Legal** | El sistema maneja información sensible relacionada con ventas, comportamiento de usuarios y datos comerciales. | Riesgo de incumplimiento de normativas de protección de datos y privacidad. | **RNFL-3-05:** El sistema debe proteger la información histórica y analítica mediante autenticación, control de acceso basado en roles y cifrado de datos sensibles almacenados y transmitidos. |
| **E — Ético** | Las recomendaciones inteligentes y decisiones automatizadas pueden influir directamente en inversiones publicitarias y estrategias de negocio. | Recomendaciones poco transparentes o sesgadas podrían afectar negativamente a los usuarios. | **RNFEt-3-06:** El sistema debe mostrar la justificación de cada recomendación o decisión automatizada indicando las métricas, tendencias históricas y reglas utilizadas para generarla. |

   
   ---
   
   ###2.3 RF3: Creatividades desde el rendimiento
   
   ---
   
   ###2.4 RF4: Confianza Progresiva
   
   ## PESTLE — RF13: Agente Conversacional Visual

| Dimensión | Hallazgo | Impacto | Requerimiento derivado |
|-----------|----------|---------|----------------------|
| **P — Político** | Colombia tiene en trámite el Proyecto de Ley 043 de 2025 de Inteligencia Artificial, radicado ante el Congreso por MinCiencias y MinTIC, que clasifica los sistemas de IA por nivel de riesgo. Los agentes conversacionales que toman decisiones comerciales podrían clasificarse como riesgo limitado o alto según este marco. | Si el proyecto es aprobado, los agentes de IA conversacionales deberán cumplir con requisitos de trazabilidad, transparencia y gobernanza. | El sistema debe documentar y hacer trazable toda acción sugerida o ejecutada por el agente de IA. |
| **E — Económico** | La síntesis de voz clonada y el procesamiento LLM en tiempo real implican costos por token y por llamada a APIs externas. Con más de 5.600 usuarios activos, el costo por interacción puede escalar rápidamente.| Sin control de consumo, el servicio puede volverse inviable a escala. | El sistema debe gestionar el consumo por niveles de suscripción e implementar caché de respuestas frecuentes para reducir costos. |
| **S — Social** | Usuarios con discapacidad auditiva pueden verse excluidos de la interacción verbal.| Un agente que solo funciona por voz excluye a usuarios con discapacidad auditiva o en entornos ruidosos. | El sistema debe mostrar siempre el texto de las respuestas de forma simultánea a la voz. |
| **T — Tecnológico** | La síntesis de voz en tiempo real con más de 5.600 usuarios puede desbordarse bajo alta concurrencia.| Si el motor de voz se satura, el agente pierde respuesta en tiempo real destruyendo la experiencia del usuario. | El sistema debe degradar al modo texto cuando el procesamiento de voz supere la capacidad disponible. |
| **L — Legal** | El agente accede a datos financieros del negocio. En Colombia aplica la Ley 1581 de Habeas Data. Dado que Dropi opera en Europa con más de 180.000 usuarios, el EU AI Act (vigente desde agosto 2024, plenamente aplicable desde agosto 2026) exige que los usuarios sean informados de que interactúan con una máquina. | No identificar el agente como IA ante usuarios europeos viola el EU AI Act, con multas de hasta 35 millones de euros. | El sistema debe identificar al agente como IA al inicio de cada sesión y cifrar las conversaciones almacenadas. |
| **E — Ético** |  la voz clonada puede ofrecerse como una opción elegible por el usuario junto a otras alternativas como voz sintética estándar o solo texto. | Si el usuario no sabe que interactúa con una IA, la confianza puede erosionarse cuando lo descubra. | El sistema debe ofrecer la voz clonada como una opción entre varias e identificar siempre al agente como IA independientemente de la modalidad elegida. |

---

## PESTLE — RF14: Recomendaciones Inteligentes

| Dimensión | Hallazgo | Impacto | Requerimiento derivado |
|-----------|----------|---------|----------------------|
| **P — Político** | Meta Ads ya está implementando en 2025-2026 restricciones en el acceso a datos para categorías sensibles (salud, finanzas, política).| El sistema puede perder datos clave para generar recomendaciones en categorías restringidas. | El sistema debe adaptarse cuando una fuente de datos esté parcialmente restringida sin interrumpir el servicio. |
| **E — Económico** | Un usuario promedio invierte entre 1.500 y 2.000 USD/mes en publicidad digital.| Una recomendación incorrecta puede generar pérdidas significativas y abandono de la plataforma. | El sistema debe mostrar el nivel de confianza de cada recomendación y advertir cuando los datos sean insuficientes. |
| **S — Social** |Entendimiento de las metricas dentro de ROAX | Si las recomendaciones usan jerga técnica el usuario no actúa sobre ellas. | El sistema debe presentar las recomendaciones en lenguaje no técnico. |
| **T — Tecnológico** | El cruce de datos entre Meta, Shopify y Dropi hoy es manual porque son bases de datos distintas | Datos inconsistentes pueden generar recomendaciones incorrectas y dañinas. | El sistema debe indicar la última sincronización de cada fuente y marcar recomendaciones de baja confianza si los datos están desactualizados. |
| **L — Legal** |  El EU AI Act exige transparencia sobre decisiones generadas por IA. | El sistema puede generar expectativas incorrectas si no aclara la naturaleza de sus sugerencias. | El sistema debe avisar que las recomendaciones son sugerencias automatizadas y que el usuario conserva la decisión final. |
| **E — Ético** |Usar datos agregados de todos los usuarios para mejorar recomendaciones individuales es válido y valioso. | El modelo puede volverse sesgado y perjudicial si no contrasta con parámetros objetivos de rentabilidad. | El sistema debe combinar el aprendizaje individual con benchmarks de industria y alertar cuando los patrones del usuario afecten negativamente su ROAS. |

---

## PESTLE — RF15: Gestión de Alertas

| Dimensión | Hallazgo | Impacto | Requerimiento derivado |
|-----------|----------|---------|----------------------|
| **P — Político** | Dado que Dropi opera en Europa, el envío de alertas con datos financieros a usuarios europeos está sujeto al GDPR y al EU AI Act. Las notificaciones automatizadas con datos personales deben cumplir requisitos de consentimiento. | Sin cumplimiento del GDPR, ROAX puede recibir sanciones regulatorias europeas. | El sistema debe diferenciar los perfiles de notificación según la región del usuario. |
| **E — Económico** | El envío masivo de alertas por correo o push implica costos por notificación que escalan con la base de usuarios. | Sin control, los costos de notificación pueden volverse inviables económicamente. | El sistema debe agrupar alertas para reducir el volumen de notificaciones sin perder cobertura crítica. |
| **S — Social** | Laura mencionó que el sistema anterior generaba hasta 250 alertas diarias causando fatiga total. Algunos canales menos invasivos como WhatsApp o correo electrónico. | La saturación de alertas lleva al usuario a desactivarlas todas, perdiendo el valor del monitoreo 24/7. | El sistema debe limitar las alertas críticas y ofrecer canales menos invasivos configurables por el usuario. |
| **T — Tecnológico** | El motor de alertas debe operar 24/7.  | Una falla nocturna puede generar pérdidas significativas y destruir la confianza en el sistema. | El sistema debe implementar redundancia en el motor de alertas y notificar al usuario ante cualquier interrupción. |
| **L — Legal** | Las alertas con métricas financieras enviadas por canales externos deben estar cifradas según la Ley 1581 y el GDPR. | El envío de datos financieros sin cifrado constituye una violación de datos personales. | El sistema debe cifrar el contenido de las notificaciones que incluyan métricas financieras del usuario. |
| **E — Ético** | El sistema prioriza alertas por impacto económico absoluto, lo que puede perjudicar a usuarios con menor volumen de inversión. | Un usuario pequeño puede perder el 100% de su presupuesto sin recibir alertas críticas. | El sistema debe calcular el impacto de las alertas de forma relativa al presupuesto de cada usuario. |

---

## PESTLE — RF16: Retroalimentación y Aprendizaje

| Dimensión | Hallazgo | Impacto | Requerimiento derivado |
|-----------|----------|---------|----------------------|
| **P — Político** | ROAX opera actualmente en Latinoamérica y Europa a través de Dropi, que tiene más de 180.000 usuarios en esa región. El EU AI Act ya está en vigor desde agosto 2024 con alcance extraterritorial y multas de hasta 35 millones de euros. | Si el motor de aprendizaje no es auditable, ROAX puede enfrentar sanciones europeas que afecten su operación en toda la región. | El sistema debe mantener logs auditables de cómo la retroalimentación del usuario modifica el modelo de recomendaciones. |
| **E — Económico** | El reentrenamiento del modelo con retroalimentación de más de 5.600 usuarios puede crecer en costos computacionales de forma no lineal. | Costos insostenibles pueden limitar la frecuencia de actualización reduciendo la personalización percibida. | El sistema debe actualizar el modelo por lotes con un ciclo máximo de 24 horas para optimizar costos. |
| **S — Social** | Usuarios con alta desconfianza inicial rechazan todas las recomendaciones sin probarlas.| Sin interacciones iniciales el sistema no puede personalizar, generando el ciclo de baja confianza.| El sistema debe ofrecer un modo de observación donde el usuario vea el impacto hipotético de recomendaciones sin necesidad de aplicarlas. |
| **T — Tecnológico** | La automatización completa requiere integración con la API de Meta, que ya ha cambiado políticas de forma abrupta y está restringiendo categorías en 2025-2026. | Si Meta revoca permisos sin aviso, la automatización falla en el momento más crítico. | El sistema debe verificar los permisos de escritura de Meta antes de cada acción automatizada. |
| **L — Legal** | El historial de comportamiento del usuario es un dato personal bajo la Ley 1581 y el GDPR, que incluye el derecho al olvido para usuarios europeos. | Almacenar datos de comportamiento sin mecanismo de eliminación viola ambas regulaciones. | El sistema debe permitir al usuario eliminar su historial de interacciones y reiniciar su modelo personalizado. |
| **E — Ético** |La IA debe usar datos de toda la base de usuarios para enriquecer recomendaciones, pero también debe proteger al usuario de reforzar sus propias malas prácticas. | El sistema puede volverse cómplice de pérdidas si refuerza decisiones que el usuario acepta pero que son objetivamente perjudiciales. | El sistema debe balancear el aprendizaje individual con parámetros objetivos de rentabilidad de la industria. |


   
   ---
   
##3. RF1: Datos y Decisiones
   
###3.1 Historias de Usuario

---
   
###3.2 Casos de Uso (Aún no solicitado)

####3.2.1 Diagrama de Casos de Uso

####3.2.2 Formatos Bicolumnares

---

##4. RF2: Alertas Inteligentes

###4.1 Historias de Usuario

# Historia de Usuario 1

**ID:** HU1  
**Título:** Visualización de campañas con bajo rendimiento

## Historia

Como usuario de la plataforma, quiero identificar fácilmente las campañas con bajo rendimiento para poder tomar decisiones rápidas y evitar pérdidas de dinero

## Criterios de Aceptación
### Scenario: Visualización correcta de campañas con bajo rendimiento
- Given que existen campañas con métricas por debajo del umbral definido

- And que el usuario ha configurado previamente los umbrales de desempeño

- When el usuario accede al módulo de campañas

- Then el sistema muestra únicamente las campañas que están por debajo del umbral

- And presenta las métricas clave asociadas (ROAS, CTR, conversiones)

**Prioridad:** Alta / Media / Baja

**Dependencias:**

---

# Historia de Usuario 2

**ID:** HU2  
**Título:** Configuración de métricas prioritarias

## Historia

Como especialista en marketing, quiero seleccionar qué métricas tienen mayor prioridad en la evaluación para adaptar el análisis a mis objetivos comerciales.

## Criterios de Aceptación

### Scenario: Selección exitosa de métricas prioritarias

- Given que el usuario accede a la configuración de evaluación de campañas

- When selecciona las métricas prioritarias para el análisis

- Then el sistema guarda la configuración seleccionada

- And utiliza dichas métricas en futuras evaluaciones de desempeño

### Scenario: Intento de guardar configuración sin métricas

- Given que el usuario accede a la configuración de métricas

- And no selecciona ninguna métrica

- When intenta guardar la configuración

- Then el sistema no permite continuar

- And muestra un mensaje indicando que debe seleccionar al menos una métrica

**Prioridad:** Alta

**Dependencias:** RF1.3

---

# Historia de Usuario 3

**ID:** HU3  
**Título:** Visualización comparativa contra umbrales

## Historia

Como usuario, quiero visualizar el valor actual de cada métrica junto al umbral configurado para entender rápidamente por qué una campaña fue clasificada como deficiente.

## Criterios de Aceptación

### Scenario: Comparación correcta de métricas y umbrales

- Given que existen campañas evaluadas por el sistema

- And que el usuario ha configurado previamente umbrales de desempeño

- When el usuario consulta el análisis de una campaña

- Then el sistema muestra el valor actual de cada métrica

- And presenta el umbral correspondiente

- And resalta visualmente las métricas que incumplen el umbral configurado

**Prioridad:** Alta

**Dependencias:** RF1.1, RF1.2

---

# Historia de Usuario 4

**ID:** HU4  
**Título:** Configuración de umbrales por tipo de campaña

## Historia

Como usuario, quiero configurar umbrales distintos según el tipo de campaña para evaluar correctamente estrategias con objetivos diferentes.

## Criterios de Aceptación

### Scenario: Configuración exitosa de umbrales diferenciados

- Given que existen distintos tipos de campañas registradas

- When el usuario define umbrales específicos para cada tipo

- Then el sistema almacena la configuración de manera independiente

- And utiliza el umbral correspondiente durante la evaluación

### Scenario: Configuración inválida de umbrales

- Given que el usuario intenta ingresar un umbral inválido

- When el valor ingresado es negativo o inconsistente

- Then el sistema rechaza la configuración

- And muestra un mensaje indicando el error

**Prioridad:** Media

**Dependencias:** RF1.2

---

# Historia de Usuario 5

**ID:** HU5  
**Título:** Detección automática de campañas críticas

## Historia

Como usuario, quiero que el sistema destaque automáticamente campañas extremadamente por debajo del umbral para priorizar acciones urgentes.

---

## Criterios de Aceptación

### Scenario: Identificación de campañas críticas

- Given que existen campañas con métricas significativamente inferiores al umbral

- When el sistema realiza el análisis de desempeño

- Then las campañas críticas son resaltadas visualmente

- And el sistema asigna un nivel de severidad alto

### Scenario: Campañas sin criticidad elevada

- Given que las campañas presentan desviaciones menores

- When el sistema procesa la evaluación

- Then las campañas se muestran como advertencias normales

- And no son clasificadas como críticas

**Prioridad:** Alta

**Dependencias:** RF1.1

### 3.2 Casos de uso

#### 3.2.1 Diagrama de casos de uso

#### 3.2.2 Formatos bicolumnares

<<Enlace Formatos bicolumnares>>

---

## 4. RF2: Subsistema B <<Nombre el Subsistema>>

### 4.1 Historias de usuario

# Historia de Usuario 1

**ID:** HU1  
**Título:** Aplicación rápida de recomendaciones

## Historia

Como usuario de la plataforma, quiero aplicar automáticamente las recomendaciones sugeridas por el sistema para optimizar mis campañas sin tener que realizar ajustes manuales.

## Criterios de Aceptación

### Scenario: Aplicación exitosa de una recomendación

-Given que el sistema ha generado una recomendación para una campaña

-And que la cuenta del usuario está correctamente integrada con las plataformas externas

-When el usuario hace clic en el botón de aplicar recomendación

-Then el sistema ejecuta automáticamente los cambios sugeridos


-And actualiza la configuración de la campaña en la plataforma externa

### Scenario: Error al aplicar recomendación por falta de integración

-Given que el sistema ha generado una recomendación para una campaña

-And que la cuenta del usuario no está correctamente integrada con la plataforma externa

-When el usuario intenta aplicar la recomendación

-Then el sistema no ejecuta ningún cambio

-And muestra un mensaje de error indicando el problema de integración

**Prioridad:** Alta / Media / Baja

**Dependencias:**

---
Historia de Usuario 2

ID: HU2
##Titulo## Recomendación automática de inversión publicitaria

Como usuario de la plataforma, quiero que el sistema detecte anuncios poco efectivos y genere nuevas imágenes o videos utilizando inteligencia artificial para atraer más clientes y mejorar las ventas.

## Criterios de Aceptación
Scenario: Generación válida de nuevo anuncio

-Given que el sistema detecta un anuncio con bajo rendimiento

-And que existen datos históricos de preferencias y ventas

-When el sistema inicia el proceso de optimización

-Then el sistema genera nuevas imágenes o videos automáticamente

-And presenta las nuevas propuestas publicitarias al usuario

## Scenario: Generación inválida por error en la inteligencia artificial

-Given que el sistema intenta generar un nuevo anuncio

-And que el servicio de inteligencia artificial presenta una falla

-When el usuario solicita la generación del anuncio

-Then el sistema no crea contenido publicitario

-And muestra un mensaje de error indicando que no fue posible generar el anuncio

Prioridad: Alta

Dependencias: Servicio de inteligencia artificial e integración con base de datos de campañas


---

###4.2 Casos de Uso (Aún no solicitado)

####4.2.1 Diagrama de Casos de Uso

####4.2.2 Formatos Bicolumnares

---

##5. RF3: Inteligencia Creativa
   
###5.1 Historias de Usuario
   
---

###5.2 Casos de Uso (Aún no solicitado)

####5.2.1 Diagrama de Casos de Uso

####5.2.2 Formatos Bicolumnares

---

## 6. RF4: Confianza Progresiva
   
###6.1 Historias de Usuario
  
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

# 5. RF15 — Gestión de Alertas (ALR)

## 5.1 Historias de Usuario

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

# 6. RF16 — Retroalimentación y Aprendizaje (RFA)

## 6.1 Historias de Usuario

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

###6.2 Casos de Uso (Aún no solicitado)

####6.2.1 Diagrama de Casos de Uso

####6.2.2 Formatos Bicolumnares

7. Backlog (Aún no solicitado)

8. MockUp (Aún no solicitado)
   8.1 Descripción General
   8.2 Enlace MockUp
