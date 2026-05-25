# DOCUMENTO DE ESPECIFICACIÓN DE REQUERIMIENTOS

## ROAX

---

### Equipo Reto 1 - Datos y Decisiones

- Daniel Felipe Herrera Parra - A00413908
- Juan Rikardo Ramírez - A00414615
- Juan José González Chavez - A00415940
- Joshua Vera Hoyos - A00414279
- Juan Pablo Ceballos - A00415570
- Alejandro Sandoval - A00418631
- Juan Esteban Otero - A00414905


### Equipo Reto 2 - Alertas que razonan

- David Altaminaro Altamirano
- Mariana Carmona Galvez
- Santiago Campo
- David Santiago García
- Mario Andrés Romero Rivera
- Andrés Vinasco

### Equipo Reto 3 - Creatividades desde el rendimiento

- MARIA JOSE SANCHEZ 
- MARIANA LUCIA GALEANO
- ESTEBAN BERNAL
- JUAN JOSE MOTATO
- SAMUEL PALMA
- SANTIAGO MILLAN

### Equipo Reto 4 - Confianza progresiva

- Melisa Gomez Gomez
- Samuel Alejandro Estupiñan Gonzales
- Jorge Humberto Garcia Leon
- Juan Camilo Borrero Florez
- Juan Pablo Urbina Ladino
- Matius Montealegre Padilla

---

# Tabla de Contenido

1. Especificación de Requerimientos
   - 1.1. Descripción General  
   - 1.2. Contexto del Proyecto  
   - 1.3. Requisitos  
   - - 1.3.1 Subsistema de Datos y Decisiones  
   - - 1.3.2 Subsistema de Alertas que Razonan  
   - - 1.3.3 Subsistema de Creatividades desde el Rendimiento  
   - - 1.3.4 Subsistema de Confianza Progresiva  

   1.4. Subespecificación por Subsistemas  
   - 1.4.1 RF1: Datos y Decisiones  
   - 1.4.2 RF2: Alertas que Razonan  
   - 1.4.3 RF3: Creatividades desde el Rendimiento  
   - 1.4.4 RF4: Confianza Progresiva  

   1.5. Tabla de Asignación a Subsistemas  

2. PESTLE
   - 2.1 RF1: Datos y Decisiones  
   - 2.2 RF2: Alertas que Razonan  
   - 2.3 RF3: Creatividades desde el Rendimiento  
   - 2.4 RF4: Confianza Progresiva  

3. RF1: Datos y Decisiones
   - 3.1. Historias de Usuario  
   - 3.2. Casos de Uso  
   - - 3.2.1 Diagrama de Casos de Uso  
   - - 3.2.2 Formatos Bicolumnares  

4. RF2: Creatividades desde el rendimiento
   - 4.1. Historias de Usuario  
   - 4.2. Casos de Uso  
   - - 4.2.1 Diagrama de Casos de Uso  
   - - 4.2.2 Formatos Bicolumnares  

5. RF3: Creatividades desde el rendimiento
   - 5.1. Historias de Usuario  
   - 5.2. Casos de Uso  
   - - 5.2.1 Diagrama de Casos de Uso  
   - - 5.2.2 Formatos Bicolumnares  

6. RF4: Confianza Progresiva
   - 6.1. Historias de Usuario  
   - 6.2. Casos de Uso  
   - - 6.2.1 Diagrama de Casos de Uso  
   - - 6.2.2 Formatos Bicolumnares  

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

La solución propuesta se divide en cuatro subsistemas principales: Datos y Decisiones, Alertas Inteligentes, Creatividades desde el rendimiento y Confianza Progresiva. Cada uno de estos componentes busca abordar distintos retos relacionados con automatización, interpretación de datos, generación de recomendaciones y aprendizaje continuo del comportamiento del negocio.

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
# Requisitos de Usuario

## RU1 - Visibilidad de rentabilidad real
El usuario necesita saber en tiempo real cuánto está ganando o perdiendo por cada campaña activa, cruzando automáticamente su inversión en publicidad con las ventas y entregas reales, sin tener que hacer los cálculos manualmente ni entrar a múltiples plataformas.

---

## RU2 - Alertas comprensibles
El usuario necesita recibir alertas que no solo le avisen que algo está mal, sino que le expliquen en lenguaje sencillo por qué está pasando y qué parte del proceso está fallando, ya sea el anuncio, la página de venta o la logística.

---

## RU3 - Control sobre la automatización
El usuario necesita poder definir sus propias reglas de automatización y aprobar las acciones que la IA propone antes de que se ejecuten, manteniendo siempre el control sobre su presupuesto y sus campañas si lo prefiere, sino, puede configurar las automatizaciones que no requieran su aporbación o considere oportunas.

---

## RU4 - Monitoreo sin intervención
El usuario necesita que el sistema vigile sus campañas las 24 horas del día los 7 días de la semana, actuando de forma autónoma dentro de los límites que él mismo configuró, para evitar pérdidas mientras no está disponible.

---

## RU5 - Privacidad y acceso seguro
El usuario necesita que los datos de sus clientes y pedidos estén protegidos, y que cada miembro de su equipo solo pueda ver la información que le corresponde según su rol.

---

## RU6 - Transparencia y acceso móvil
El usuario necesita conocer cualquier costo adicional antes de aplicar cambios en su presupuesto, y poder gestionar todo desde su telefono -ya sea en app o en portal web o en un chatbot de wspp- sin perder funcionalidades.

---

## RU7 - Decisiones con contexto real
El usuario puede preferir que la IA tenga en cuenta factores reales de su negocio como el inventario disponible, sus restricciones financieras y el perfil de su cliente ideal, para que las recomendaciones sean útiles y no genéricas; o puede usar las recomendaciones de MEta Advantage.

---

# Requisitos del Sistema

## RF1
El sistema debe calcular la rentabilidad real del negocio integrando fuentes de pauta y ventas.

### RF1.1
El sistema debe cruzar automáticamente los datos de Meta Ads (Inversión, ROAS, CPA) con los de las plataformas de venta como Shopify o Dropi, para saber cuánto está ganando o perdiendo el negocio por cada campaña activa.

### RF1.2
El sistema debe detectar de forma proactiva las campañas que no están siendo rentables, comparando el ROAS actual contra el punto de equilibrio real del producto.

---

## RF2
El sistema debe explicar el porqué de cada métrica de rentabilidad.

### RF2.1
Las alertas del sistema no deben limitarse a mostrar datos. Deben explicar qué está pasando y por qué, por ejemplo:

> "La campaña X está quemando dinero porque el CPA superó el margen de ganancia en un 15%".

### RF2.2
El sistema aprenderá de las decisiones del usuario -aprobaciones, rechazos y modificaciones- para ajustar progresivamente su nivel de autonomía.

El usuario puede configurar en cualquier momento qué tipo de acciones puede ejecutar la IA sin pedir permiso -En modo Automatico- basándose en el historial de interacciones que haya acumulado.

El nivel de autonomía activado siempre es reversible.

---

## RF3
El sistema debe ejecutar acciones correctivas de forma autónoma sobre la publicidad digital.

### RF3.1
Cada usuario debe poder configurar sus propias reglas de automatización, como pausar campañas o ajustar presupuestos, basándose en la rentabilidad real del negocio y no solo en las métricas de pauta.

### RF3.2
Cada acción automática debe quedar registrada con:
- la fecha,
- lo que se hizo,
- y la razón por la que se tomó esa decisión.

---

## RF4
El sistema debe monitorear el negocio de forma autónoma las 24 horas, los 7 días de la semana.

### RF4.1
El sistema debe revisar continuamente los datos de Meta Ads para detectar, incluso fuera del horario de trabajo del usuario, cuando el CPA o el ROAS estén fallando de forma crítica y poniendo en riesgo la rentabilidad.

La evaluación debe considerar el tiempo de madurez de cada campaña, reconociendo que los datos de Meta Ads tienen un delay natural de hasta 24 horas, y clasificar el rendimiento según la fase en que se encuentre la campaña:
- Testeo,
- Optimización,
- Escalado.

---

## RF5
El sistema debe proteger la integridad y privacidad de los datos del e-commerce.

### RF5.1
El sistema debe cumplir con la Ley de Habeas Data y cifrar los datos de clientes y pedidos de Shopify o Dropi usando protocolos TLS 1.3.

### RF5.2
El acceso a los datos financieros debe estar dividido por roles:
- Administrador,
- Vendedor,

para que la información sensible solo la vea quien debe verla.

---

## RF6
El sistema debe ser transparente con los costos y funcionar bien en dispositivos móviles.

### RF6.1
Antes de ejecutar cualquier cambio de presupuesto o activar una integración que pueda generar costos adicionales, el sistema debe informar al usuario sobre:
- el monto estimado,
- la frecuencia,
- y el servicio involucrado.

Esto aplica tanto desde la plataforma web como desde el chatbot de WhatsApp, y el sistema siempre debe esperar confirmación explícita antes de proceder.

Sin sorpresas, en ningún canal.

### RF6.2
El sistema debe funcionar correctamente en navegadores móviles de Android e iOS, ya que la mayoría de los dropshippers manejan su negocio desde el celular.

---

## RF7
El sistema debe tomar decisiones considerando el contexto operativo real del negocio, más allá de los datos de las APIs de publicidad, integrando:
- el inventario,
- las restricciones financieras,
- y el perfil cualitativo del cliente ideal.

### RF7.1
El sistema debe sincronizarse de forma automática con el inventario real de cada producto, leyendo el stock disponible en tiempo real desde las plataformas de venta integradas:
- Shopify,
- Dropi,
- WooCommerce,
- Tienda Nube.

Cuando un producto se quede sin stock o caiga por debajo del umbral mínimo definido, el sistema debe pausar automáticamente las campañas asociadas para evitar gasto publicitario innecesario, y reactivarlas cuando el inventario sea repuesto.

### RF7.2
Además, el sistema debe identificar campañas ganadoras -aquellas con ROAS y CPA sostenidos en zona positiva por más de 24 horas- y sugerir proactivamente un aumento de presupuesto cuando haya margen financiero disponible según las restricciones registradas.

La sugerencia debe incluir:
- el monto recomendado,
- la proyección de gasto en las próximas 24 horas,
- y el resultado esperado,

antes de que el usuario confirme.

### RF7.3
El sistema debe conectarse con la API de Meta Advantage para analizar la configuració.n de los públicos en las campañas activas, detectar errores o inconsistencias en la segmentación actual y sugerir ajustes concretos.

El usuario siempre puede:
- aceptar,
- modificar,
- o descartar cada sugerencia.

El sistema no aplica cambios de segmentación de forma automática.

### RF7.4
El sistema debe integrar fuentes de datos externos del mercado:
- tendencias estacionales,
- picos de demanda detectables en plataformas como Google Trends,
- comportamiento publicitario de la competencia accesible vía APIs públicas de Meta.

Además, debe alimentar a la IA con esa información para que sus recomendaciones de pauta consideren el contexto externo, anticipándose a oportunidades o riesgos que no son visibles desde los datos internos del negocio.

---

# Requisitos de Proceso

## RP1
El desarrollo del módulo se llevará a cabo bajo metodología Scrum, con:
- sprints de 2 semanas,
- y reuniones de revisión al final de cada sprint con el Product Owner de ROAX.

---

## RP2
El código fuente del sistema debe gestionarse mediante control de versiones usando Git, con ramas separadas para:
- desarrollo,
- pruebas,
- y producción.

---

## RP3
Toda integración con APIs externas:
- Meta Ads,
- Shopify,
- Dropi,

debe realizarse respetando los permisos y condiciones de uso vigentes de cada plataforma.

---

## RP4
El sistema debe ser diseñado para operar sobre la infraestructura existente de ROAX en:

> app.roaxai.com

sin requerir cambios en la arquitectura base de la plataforma externa.


---

### 1.3.2 Subsistema de Alertas que razonan

#### RF1. El sistema debe mostrar al usuario las campañas cuyo desempeño se encuentre por debajo de un umbral definido.
   
#### RF2. El sistema generará recomendaciones inteligentes basadas en losresultados del negocio

#### RF3. El sistema debe medir, analizar y aprender del impacto de las decisiones tomadas en campañas publicitarias y resultados del negocio.

#### RF4. El sistema debe construir confianza progresiva en las recomendaciones generadas por IA

---

### 1.3.3 Subsistema de Creatividades desde el rendimiento

<DESCRIPCIÓN DE LOS REQUISITOS DE ALTO NIVEL>

| RF  | Requerimiento de alto nivel                                                                    |
| ------- | ---------------------------------------------------------------------------------------------- |
| RF1     | El sistema debe capturar la información básica del usuario.                                    |
| RF1.1   | El sistema debe permitir la identificación única de cada cliente.                              |
| RF1.1.1 | El sistema debe clasificar a los usuarios según su perfil dentro de la organización.           |
| RF2     | El sistema debe gestionar el perfil detallado del cliente.                                     |
| RF2.1   | El sistema debe centralizar la información detallada del consumidor.                           |
| RF2.1.1 | El sistema debe consolidar datos demográficos, históricos y preferencias en un solo perfil.    |
| RF3     | El sistema debe generar reportes de estado de negocio.                                         |
| RF3.1   | El sistema debe emitir informes sobre situación financiera y operativa.                        |
| RF3.1.1 | El sistema debe integrar indicadores de deuda, impuestos y costos fijos en el balance general. |
| RF3.1.2 | El sistema debe notificar el estado del inventario y flujo de procesos actuales.               |
| RF4     | El sistema debe gestionar estrategias de marketing basadas en datos.                           |
| RF4.1   | El sistema debe analizar el rendimiento de campañas publicitarias.                             |
| RF4.1.1 | El sistema debe generar propuestas de mejora basadas en comparación de resultados históricos.  |

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

   ### 1.4.1 RF1: Datos y Decisiones

   1.4 Subespecificación por Subsistemas  
SS1 - Motor de Rentabilidad
RF1.1. El sistema debe cruzar automáticamente los datos de Meta Ads (Inversión, ROAS, CPA) con los de las plataformas de venta como Shopify o Dropi, para saber cuánto está ganando o perdiendo el negocio por cada campaña activa.
RF1.2. El sistema debe detectar de forma proactiva las campañas que no están siendo rentables, comparando el ROAS actual contra el punto de equilibrio real del producto, no solo mostrar números, sino avisar cuando algo está saliendo mal.

SS2 - Motor de IA Explicativa
RF2.1. Las alertas del sistema no deben limitarse a mostrar datos. Deben explicar qué está pasando y por qué, por ejemplo: "La campaña X está quemando dinero porque el CPA superó el margen de ganancia en un 15%".
RF2.2. El sistema aprenderá de las decisiones del usuario (aprobaciones, rechazos, modificaciones) antes de ejecutar cualquier acción automática  y ajustará progresivamente el nivel de autonomía de la IA, permitiendo que el usuario lo revise y modifique en cualquier momento. 

SS3 - Motor de Automatización y Reglas
RF3.1. Cada usuario debe poder configurar sus propias reglas de automatización, como pausar campañas o ajustar presupuestos, basándose en la rentabilidad real del negocio y no solo en las métricas de pauta.
RF3.2. Cada acción automática debe quedar registrada con la fecha, lo que se hizo y la razón por la que se tomó esa decisión. El usuario siempre debe poder saber qué hizo el sistema y por qué.


SS4 - Monitor 24/7 y Detección de Anomalías
RF4.1. El sistema debe revisar continuamente los datos de Meta Ads para detectar, incluso fuera del horario de trabajo del usuario, cuando el CPA o el ROAS estén fallando de forma crítica y poniendo en riesgo la rentabilidad. Para hacer esta evaluación correctamente, el sistema debe reconocer el tiempo de madurez de la campaña y el delay de 24 horas propio de Meta Ads, usando indicadores diferenciados según la fase activa: Hook rate, Retention rate, Click rate y Tasas de retención en Testeo; Tasas de conversión en Optimización; y CPA y ROAS neto en Escalado. 



SS5 - Seguridad, Privacidad y Control de Acceso
RF5.1. El sistema debe cumplir con la Ley de Habeas Data y cifrar los datos de clientes y pedidos de Shopify o Dropi usando protocolos TLS 1.3. Proteger la información de los compradores no es opcional.
RF5.2. El acceso a los datos financieros debe estar dividido por roles, Administrador y Vendedor  para que la información privada solo la vea quien debe verla.


SS6 - Interfaz Conversacional y Movilidad
RF6.1: Transparencia de costos antes de ejecutar cambios (web y WhatsApp)
RF6.2: Conversación con bot inteligente vía WhatsApp


SS7 - Integraciones y Contexto Operativo
RF7.1: Sincronización automática con inventario
RF7.2: Restricciones financieras y sugerencia de escalar en campañas ganadoras
RF7.3: API Meta Advantage — segmentación y auditoría de públicos
RF7.4: Fuentes externas del mercado (Google Trends, competencia)

   
   ---
   
   ### 1.4.2 RF2: Alertas que razonan
   
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
   
   ### 1.4.3 RF3: Creatividades desde el rendimiento

   
Subsistema A — Gestión de Usuarios
| Código      | Subrequerimiento                                                 |
| ----------- | ---------------------------------------------------------------- |
| USU_RF1.1   | Registrar usuarios con identificador único, correo y contraseña. |
| USU_RF1.1.1 | Asignar roles organizacionales a usuarios.                       |
| USU_RF1.1.2 | Permitir inicio de sesión seguro.                                |
| USU_RF1.1.3 | Permitir recuperación de contraseña mediante correo.             |

Subsistema B — Perfilamiento del Cliente
| Código      | Subrequerimiento                                                |
| ----------- | --------------------------------------------------------------- |
| PER_RF2.1   | Centralizar información del consumidor desde múltiples fuentes. |
| PER_RF2.1.1 | Consolidar datos históricos y demográficos en un perfil único.  |
| PER_RF2.1.2 | Consultar perfil 360° por ID o correo.                          |
| PER_RF2.1.3 | Guardar trazabilidad de la fuente de cada dato.                 |
| PER_RF2.1.4 | Fusionar registros duplicados automáticamente.                  |
| PER_RF2.1.5 | Registrar consentimiento para tratamiento de datos.             |

Subsistema C — Reportes de Inteligencia de Negocio
| Código      | Subrequerimiento                                      |
| ----------- | ----------------------------------------------------- |
| REP_RF3.1   | Generar reportes financieros y operativos.            |
| REP_RF3.1.1 | Integrar costos fijos, impuestos y deudas.            |
| REP_RF3.1.2 | Integrar métricas de inventario y flujo de productos. |
| REP_RF3.1.3 | Exportar reportes en PDF y Excel.                     |
| REP_RF3.1.4 | Generar reportes periódicos automáticos.              |

Subsistema D — Optimización de Campañas con IA
| Código      | Subrequerimiento                                                    |
| ----------- | ------------------------------------------------------------------- |
| OPT_RF4.1   | Analizar el rendimiento de campañas activas.                        |
| OPT_RF4.1.1 | Asociar creatividades con métricas reales de conversión.            |
| OPT_RF4.1.2 | Clasificar creatividades por estilo, copy y formato.                |
| OPT_RF4.1.3 | Identificar patrones comunes en creatividades exitosas.             |
| OPT_RF4.1.4 | Generar propuestas automáticas de mejora para nuevas creatividades. |
| OPT_RF4.1.5 | Predecir rendimiento esperado antes de lanzar una creatividad.      |

Subsistema E — Integración de APIs Externas
| Código   | Subrequerimiento                               |
| -------- | ---------------------------------------------- |
| API_INT1 | Integrarse con Meta Ads API.                   |
| API_INT2 | Integrarse con Shopify API.                    |
| API_INT3 | Integrarse con Dropi API.                      |
| API_INT4 | Integrarse con TikTok Ads API.                 |
| API_INT5 | Implementar OAuth 2.0 y manejo de rate limits. |
   
   ---
   
   ### 1.4.4 RF4: Confianza Progresiva

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

### Tabla de Asignación a Subsistemas - RF1 y RF2

| Requerimiento | Motor de Datos y Análisis | Motor de Alertas Inteligentes | Motor de Creatividades desde el rendimiento | Motor de Confianza y Aprendizaje | Integraciones y APIs | Sistema Conversacional | Monitor de Rendimiento y Riesgos |
| --- | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| RF1 | X |  |  |  | X |  |  |
| RF1.1 | X |  |  |  | X |  |  |
| RF1.1.1 | X |  |  |  | X |  |  |
| RF1.1.2 | X |  |  |  | X |  |  |
| RF1.1.3 | X |  |  |  | X |  |  |
| RF1.2 | X | X |  |  | X |  | X |
| RF1.2.1 | X | X |  |  | X |  | X |
| RF1.2.2 | X | X |  |  | X |  | X |
| RF1.3 | X |  |  | X | X |  |  |
| RF1.3.1 | X |  |  | X | X |  |  |
| RF1.4 | X | X |  |  | X |  | X |
| RF1.4.1 | X | X |  |  | X |  | X |
| RF1.4.2 | X | X |  |  | X |  | X |
| RF2.1 | X | X |  |  | X |  | X |
| RF2.1.1 | X | X |  |  |  |  | X |
| RF2.1.2 | X | X |  |  |  |  |  |
| RF2.1.3 | X | X |  |  |  |  |  |
| RF2.2 |  | X | X |  | X |  |  |
| RF2.2.1 | X | X |  |  | X |  |  |
| RF2.2.2 |  | X | X |  | X |  |  |
| RF2.2.3 |  | X |  | X | X |  |  |
| RF2.3 | X | X |  | X | X |  | X |
| RF2.3.1 | X | X |  | X |  |  |  |
| RF2.3.2 | X | X |  | X |  |  | X |
| RF2.3.3 | X |  |  | X |  |  |  |
| RF2.3.4 | X | X |  |  | X |  | X |
| RF2.3.5 | X | X |  |  | X |  | X |
| RF2.3.6 | X | X |  |  | X |  |  |
| RF2.3.7 | X | X |  |  | X |  | X |
| RF2.3.8 | X | X |  |  | X |  | X |
| RF2.3.9 | X | X |  |  | X |  | X |
| RF2.3.10 | X | X |  |  | X |  | X |
| RF2.3.11 | X | X |  | X |  |  |  |
| RF2.3.12 | X | X |  | X |  | X |  |
| RF2.3.13 | X | X |  | X |  |  |  |
| RF2.3.14 | X | X |  | X | X |  | X |
| RF2.3.15 | X |  |  | X |  |  |  |

### Tabla de Asignación a Subsistemas - RF3 y RF4

| Requerimiento | Motor de Datos y Análisis | Motor de Alertas Inteligentes | Motor de Creatividades desde el rendimiento | Motor de Confianza y Aprendizaje | Integraciones y APIs | Sistema Conversacional | Monitor de Rendimiento y Riesgos |
| --- | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| RF3 |  |  | X |  | X | X |  |
| RF3.1 |  |  | X |  | X | X |  |
| RF3.1.1 |  |  | X |  | X | X |  |
| RF3.1.2 |  | X | X |  | X | X |  |
| RF3.1.3 |  |  | X |  | X | X |  |
| RF3.2 |  | X | X |  | X | X |  |
| RF3.2.1 |  | X | X |  | X | X |  |
| RF3.2.2 |  | X | X |  | X | X |  |
| RF3.2.3 |  | X | X |  | X | X |  |
| RF3.3 |  |  | X |  | X | X |  |
| RF3.3.1 |  |  | X |  | X | X |  |
| RF4.1 |  | X |  | X |  |  |  |
| RF4.1.1 |  | X |  | X |  |  |  |
| RF4.1.2 | X | X |  | X |  |  |  |
| RF4.2 |  | X |  | X |  |  | X |
| RF4.2.1 |  | X |  | X |  |  | X |
| RF4.2.2 | X | X |  | X |  |  |  |
| RF4.3 |  |  |  | X |  | X |  |
| RF4.3.1 |  |  |  | X |  | X |  |
| RF4.3.2 | X |  |  | X |  |  |  |
| RF4.4 |  | X |  | X |  |  |  |
| RF4.4.1 | X | X |  | X |  |  |  |
| RF4.4.2 |  | X |  | X |  |  |  |
| RF4.5 |  |  |  | X |  | X |  |
| RF4.5.1 |  |  |  | X |  | X |  |
| RF4.5.2 | X |  |  | X |  |  |  |


# 2. PESTLE

> El análisis PESTLE se aplica a los requerimientos funcionales que toman decisiones sobre personas, usan datos sensibles o pueden generar impacto negativo. Para cada dimensión se identifica el hallazgo verificado, su impacto real y el requerimiento derivado.


   ### 2.1 RF1: Datos y Decisiones

   # 2. PESTLE

| Dimensión | Hallazgo | Impacto | Requerimiento derivado |
| --- | --- | --- | --- |
| **P — Político** | La autonomía configurable de la IA y la posibilidad de delegar decisiones según el historial de confianza están en una zona gris legal en Colombia. No queda claro quién responde si algo sale mal. | Si la IA ejecuta una acción financiera sin que el usuario la haya aprobado manualmente, hay que definir de antemano quién asume la responsabilidad. Lo mismo aplica si el usuario aplica un cambio de segmentación sugerido por la IA y el resultado empeora. | **RNFP-7-01:** Antes de activar el "Modo Autónomo", el sistema debe mostrar una cláusula de aceptación de riesgos vinculada al historial de confianza del usuario.<br><br>**RNFP-7-02:** Cuando el sistema sugiera un cambio de segmentación vía Meta Advantage, debe advertir que la decisión y sus consecuencias son responsabilidad del usuario, y registrar su aceptación explícita antes de aplicar cualquier cambio. |
| **E — Económico** | Las sugerencias de escalado de presupuesto en campañas ganadoras, combinadas con el delay de 24 h de Meta, pueden afectar el flujo de caja antes de ver si el dinero valió la pena. A esto se suma el riesgo de actuar sobre sugerencias de segmentación o tendencias externas sin medir el impacto económico previo. | Escalar sin considerar el delay puede generar sobrecostos antes de ver resultados. Cambiar la segmentación puede reducir el alcance y subir el CPM. Actuar sobre una tendencia de Google Trends que no se convierte en ventas es un gasto igualmente evitable. | **RNFE-7-02:** Antes de sugerir escalar el presupuesto de una campaña en etapa de "madurez temprana", el sistema debe proyectar cuánto se va a gastar en las próximas 24 horas.<br><br>**RNFE-7-03:** Antes de sugerir un ajuste de segmentación vía Meta Advantage, el sistema debe estimar el impacto en alcance y CPM proyectado para que el usuario entienda el costo económico del cambio.<br><br>**RNFE-7-04:** Cuando una recomendación se base en tendencias externas (Google Trends u otras), el sistema debe aclarar que es contextual y no garantiza conversiones, antes de sugerir cualquier aumento de presupuesto. |
| **S — Social** | Pasar de tableros visuales a un chatbot por WhatsApp cambia radicalmente cómo el usuario consume los datos de su negocio. Además, el acceso fácil a sugerencias de audiencia puede hacer que con el tiempo el usuario deje de desarrollar su propio criterio de segmentación. | Con respuestas puntuales por chat es fácil perder la visión completa del negocio. Ver una métrica suelta no es lo mismo que ver cómo se comporta frente al mes anterior. | **RNFS-7-03:** El chatbot debe permitir que el usuario solicite resúmenes ejecutivos en PDF o imagen, para que pueda revisar métricas de forma visual fuera del hilo de conversación. |
| **T — Tecnológico** | El sistema depende de tres APIs externas críticas: WhatsApp Business, Meta Ads para gestión de campañas y Meta Advantage para segmentación de públicos. A estas se suman Google Trends y las APIs públicas de Meta para datos de competencia, todas fuera del control del proyecto. | Si Meta cambia permisos, revoca acceso a la API de segmentación o WhatsApp Business se cae, el usuario queda sin gestión operativa móvil y sin sugerencias de audiencia. Y eso puede pasar en el peor momento. | **RNFT-7-04:** El sistema debe tener un mecanismo de "Heartbeat" que avise al usuario por SMS o correo cuando falle cualquiera de estas conexiones: WhatsApp Business API, Meta Ads API, Meta Advantage Segmentation API o las fuentes de datos externos. |
| **L — Legal** | Manejar datos de ventas por WhatsApp, acceder a audiencias de Meta Advantage y almacenar información financiera del negocio saca datos sensibles del entorno controlado de la plataforma y genera obligaciones adicionales bajo la Ley 1581. | Datos de clientes en chat, datos de comportamiento de audiencias y datos financieros como deudas o límites de caja requieren consentimiento explícito, cifrado y acceso restringido. Sin esto, el sistema es un riesgo legal activo. | **RNFL-7-05:** Cualquier mensaje del chatbot que contenga datos sensibles de clientes debe ir precedido de una confirmación de identidad del usuario en el dispositivo móvil.<br><br>**RNFL-7-06:** Antes de activar la integración con Meta Advantage, el sistema debe informar al usuario que se accederá a datos de audiencias bajo las políticas de Meta y la Ley 1581, y registrar su aceptación.<br><br>**RNFL-7-07:** Los datos financieros registrados (deudas, límites de caja, presupuestos) deben tratarse con el mismo nivel de protección que los datos de clientes: cifrado TLS 1.3 y acceso restringido al rol Administrador. |
| **É — Ético** | La IA aprende los hábitos del usuario y puede reforzarlos aunque no sean los mejores. Además, las sugerencias de segmentación pueden introducir sesgos en la audiencia publicitaria, y la lógica de escalar campañas ganadoras puede incentivar un gasto mayor del que el negocio realmente soporta. | Una IA que valida hábitos malos, sugiere públicos sesgados o empuja a gastar más sin verificar la salud financiera real del negocio termina siendo un problema, no una ayuda. | **RNFE-7-06:** Cuando las automatizaciones basadas en hábitos del usuario vayan en contra de los KPIs de rentabilidad neta, el sistema debe emitir una "Alerta de Salud de Negocio".<br><br>**RNFE-7-07:** El sistema debe auditar periódicamente los públicos sugeridos para detectar si las recomendaciones excluyen sistemáticamente grupos demográficos sin justificación de rendimiento, y alertar al usuario si detecta un patrón.<br><br>**RNFE-7-08:** Cuando sugiera escalar el presupuesto de una campaña ganadora, el sistema debe verificar primero que las métricas de rentabilidad neta del negocio (no solo de la campaña) soporten ese crecimiento. |
   
   ---
   
   ### 2.2 RF2: Alertas que razonan
   
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
   
 ### 2.3 RF3: Creatividades desde el rendimiento

   2.1 Listado de requerimientos PESTLE
| Factor      | Situación                                        | Requerimiento derivado                                                                   |
| ----------- | ------------------------------------------------ | ---------------------------------------------------------------------------------------- |
| Político    | Regulación futura de IA generativa en publicidad | P1: El sistema debe etiquetar anuncios generados por IA en la metadata.                  |
| Político    | Transparencia en publicidad dirigida             | P2: El sistema debe generar reportes auditables sobre creación de anuncios.              |
| Económico   | Presupuestos en USD y ventas en COP              | E1: El sistema debe normalizar métricas usando tasa de cambio vigente.                   |
| Económico   | CPM creciente obliga optimización                | E2: El sistema debe mostrar impacto del CPM en rentabilidad.                             |
| Social      | Preferencia por anuncios auténticos (UGC)        | S1: El sistema debe clasificar creatividades por estilo y correlacionar con rendimiento. |
| Social      | Fatiga publicitaria                              | S2: El sistema debe medir fatiga mediante caída progresiva del CTR.                      |
| Tecnológico | Uso de Meta Ads API y Shopify                    | T1: El sistema debe integrarse con APIs externas para campañas y ventas reales.          |
| Tecnológico | Restricciones de tracking (cookies/iOS)          | T2: El sistema debe manejar atribución con datos disponibles.                            |
| Legal       | Habeas Data (Ley 1581)                           | L1: El sistema debe registrar consentimiento antes de consolidar datos personales.       |
| Legal       | Derecho al olvido y portabilidad                 | L2: El sistema debe permitir eliminación y exportación de datos personales.              |
| Ambiental   | Alto consumo energético de IA                    | A1: El sistema debe optimizar análisis con caché y modelos eficientes.                   |
   
   ---
   
 ### 2.4 RF4: Confianza Progresiva
   
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

# Historias de usuario y Casos de uso

## 3. RF1: Datos y Decisiones

## 3.1 Historias de Usuario
   

**RF1: Motor de Rentabilidad**

**HU RF1.1 - Visualización de rentabilidad real por campaña**

| **Historia N°:** | RF1.1                                                                                                                    |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------ |
| **Yo como**      | dropshipper                                                                                                              |
| **Quiero**       | que el sistema cruce automáticamente mis datos de inversión en Meta Ads con las ventas reales de mi tienda               |
| **Para**         | saber en tiempo real cuánto estoy ganando o perdiendo por cada campaña activa, sin tener que hacer los cálculos yo mismo |

Escenario RF1.1.1

| **Scenario: Cálculo del margen neto real por campaña** | |
| --- | | --- |
| **Given** | el dropshipper tiene sesión iniciada y ha integrado su cuenta de Meta Ads y su tienda en ROAX |
| **When** | accede al dashboard de rentabilidad |
| **Then** | el sistema muestra el margen neto real por campaña usando órdenes efectivamente entregadas, no solo las vendidas |
| **And** | el dashboard distingue entre órdenes entregadas, pendientes y devueltas |

Escenario RF1.1.2

| **Scenario: Actualización de datos con retraso máximo de 15 minutos** | |
| --- | | --- |
| **Given** | el dropshipper tiene campañas activas con datos en Meta Ads y Shopify/Dropi |
| **When** | consulta el dashboard de rentabilidad |
| **Then** | el sistema muestra información actualizada con un máximo de 15 minutos de retraso respecto a las fuentes de datos |
| **And** | se indica la hora de la última actualización |

**HU RF1.2 - Detección proactiva de campañas deficitarias**

| **Historia N°:** | RF1.2                                                                                                                  |
| ---------------- | ---------------------------------------------------------------------------------------------------------------------- |
| **Yo como**      | dropshipper                                                                                                            |
| **Quiero**       | recibir una alerta automática cuando alguna campaña activa esté por debajo del punto de equilibrio real de mi producto |
| **Para**         | poder actuar antes de perder más dinero del necesario                                                                  |

**Escenario RF1.2.1**

| **Scenario: Alerta por campaña bajo el punto de equilibrio** | |
| --- | | --- |
| **Given** | el dropshipper tiene una campaña activa con el margen del producto registrado en ROAX |
| **When** | el ROAS de la campaña cae por debajo del umbral de equilibrio durante más de 2 horas continuas |
| **Then** | el sistema genera una alerta automática indicando qué campaña está afectada |
| **And** | la alerta muestra cuánto dinero se está perdiendo por hora y desde cuándo ocurre la caída |

**Escenario RF1.2.2**

| **Scenario: Cálculo automático del ROAS de equilibrio** | |
| --- | | --- |
| **Given** | el dropshipper ha registrado el margen del producto en ROAX |
| **When** | el sistema analiza el rendimiento de la campaña |
| **Then** | calcula automáticamente el ROAS de equilibrio a partir del margen del producto registrado |
| **And** | usa ese umbral como referencia para activar alertas de déficit |

**HU RF3.1 - Configuración de reglas de automatización personalizadas**

| **Historia N°:** | RF3.1                                                                                                                                             |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Yo como**      | dropshipper                                                                                                                                       |
| **Quiero**       | poder configurar mis propias reglas de automatización, como pausar campañas o ajustar presupuestos, basadas en la rentabilidad real de mi negocio |
| **Para**         | tener control sobre las acciones automáticas del sistema sin depender solo de las métricas de Meta                                                |

**Escenario RF3.1.1**

| **Scenario: Creación de una regla para pausar campaña por CPA alto** | |
| --- | | --- |
| **Given** | el dropshipper tiene sesión iniciada y tiene campañas activas integradas en ROAX |
| **When** | accede al módulo de automatización y define una regla del tipo "Si el CPA supera X valor durante más de Y horas pausar la campaña" |
| **Then** | el sistema guarda la regla y la asocia a las campañas seleccionadas |
| **And** | muestra una confirmación con el resumen de la regla creada y las campañas afectadas |

**Escenario RF3.1.2**

| **Scenario: Edición y desactivación de una regla existente** | |
| --- | | --- |
| **Given** | el dropshipper tiene al menos una regla de automatización configurada |
| **When** | accede a la lista de reglas y selecciona una para editarla o desactivarla |
| **Then** | el sistema actualiza la regla con los nuevos parámetros o la marca como inactiva |
| **And** | las campañas asociadas dejan de estar sujetas a esa regla hasta que el usuario la reactive |

**HU RF3.2 - Registro auditado de acciones automáticas**

| **Historia N°:** | RF3.2                                                                                                             |
| ---------------- | ----------------------------------------------------------------------------------------------------------------- |
| **Yo como**      | dropshipper                                                                                                       |
| **Quiero**       | que el sistema registre cada acción automática que ejecute, indicando qué hizo, cuándo y por qué                  |
| **Para**         | poder revisar el historial de decisiones del sistema y entender si está actuando correctamente sobre mis campañas |

**Escenario RF3.2.1**

| **Scenario: Consulta del historial de acciones automáticas** | |
| --- | | --- |
| **Given** | el dropshipper tiene sesión iniciada y el sistema ha ejecutado al menos una acción automática |
| **When** | accede al módulo de historial de automatización |
| **Then** | el sistema muestra una lista cronológica de todas las acciones ejecutadas, con la fecha, la campaña afectada, la acción tomada y la regla o condición que la disparó |
| **And** | cada entrada incluye el estado anterior y posterior de la campaña para que el usuario pueda comparar |

**Escenario RF3.2.2**

| **Scenario: Detalle de una acción automática específica** | |
| --- | | --- |
| **Given** | el dropshipper está consultando el historial de acciones automáticas |
| **When** | selecciona una acción específica de la lista |
| **Then** | el sistema muestra el detalle completo: hora exacta, métricas que activaron la regla (por ejemplo, CPA en ese momento), la decisión tomada y si el usuario la revirtió manualmente después |
| **And** | ofrece la opción de deshacer la acción si aún es posible hacerlo |

**HU RF4.1 - Monitoreo continuo del negocio**

| **Historia N°:** | RF4.1                                                                                                                                                                                                                     |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Yo como**      | dropshipper                                                                                                                                                                                                               |
| **Quiero**       | que el sistema monitoree continuamente mis campañas en Meta Ads evaluando su rendimiento según la fase en que se encuentran (Testeo, Optimización o Escalado) y considerando el delay de 24 horas propio de la plataforma |
| **Para**         | recibir alertas precisas que no confundan una campaña inmadura con una campaña fallida, y poder tomar decisiones correctas en el momento adecuado                                                                         |

**Escenario RF4.1.1**

| **Scenario: Evaluación de campaña en fase de Testeo con indicadores correctos** | |
| --- | | --- |
| **Given** | el dropshipper tiene una campaña activa clasificada en fase de Testeo y el sistema ha recopilado datos con al menos 24 horas de antigüedad |
| **When** | el sistema evalúa el rendimiento de esa campaña |
| **Then** | analiza los indicadores propios de Testeo: Hook rate, Tasas de retención de atención, Retention rate y Click rate |
| **And** | no emite alertas de CPA o ROAS hasta que la campaña haya superado la fase de madurez mínima |

**Escenario RF4.1.2**

| **Scenario: Detección de bajo rendimiento en fase de Escalado** | |
| --- | | --- |
| **Given** | el dropshipper tiene una campaña en fase de Escalado con umbrales de CPA y ROAS neto configurados |
| **When** | el sistema detecta que el CPA supera el umbral definido o que el ROAS neto cae por debajo del punto de equilibrio |
| **Then** | genera una alerta indicando la campaña afectada, la fase en que se encuentra y el indicador crítico que falló |
| **And** | registra el evento con la hora, los valores detectados y el contexto de madurez de la campaña para que el usuario pueda interpretar correctamente la situación |

**HU RF5.1 - Protección de datos bajo Ley de Habeas Data**

| **Historia N°:** | RF5.1                                                                                                                                               |
| ---------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Yo como**      | dropshipper                                                                                                                                         |
| **Quiero**       | que el sistema cifre y proteja los datos personales de mis clientes y pedidos provenientes de Shopify o Dropi, cumpliendo con la Ley de Habeas Data |
| **Para**         | garantizar que la información privada de mis compradores esté segura y que mi negocio opere dentro del marco legal colombiano                       |

**Escenario RF5.1.1**

| **Scenario: Cifrado de datos personales en tránsito** | |
| --- | | --- |
| **Given** | el sistema está recibiendo datos de clientes y pedidos desde Shopify o Dropi mediante la integración configurada por el dropshipper |
| **When** | los datos se transmiten entre las plataformas externas y ROAX |
| **Then** | el sistema aplica cifrado TLS 1.3 sobre toda la comunicación que contenga información personal como nombres, direcciones y datos de contacto de compradores |
| **And** | cualquier intento de conexión con protocolos de menor versión es rechazado automáticamente |

**Escenario RF5.1.2**

| **Scenario: Datos personales no expuestos en logs ni interfaces no autorizadas** | |
| --- | | --- |
| **Given** | el sistema ha procesado órdenes con datos personales de clientes |
| **When** | se generan registros internos de actividad, errores o auditoría |
| **Then** | el sistema omite o enmascara los datos personales identificables (nombre, teléfono, dirección) en los logs del sistema |
| **And** | los datos completos solo son accesibles desde las vistas habilitadas para roles con permiso explícito |

**HU RF5.2 - Control de acceso diferenciado por roles**

| **Historia N°:** | RF5.2                                                                                                                                                |
| ---------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Yo como**      | dropshipper con equipo de trabajo                                                                                                                    |
| **Quiero**       | que el sistema restrinja el acceso a la información financiera según el rol de cada miembro del equipo, diferenciando entre Administrador y Vendedor |
| **Para**         | que los datos sensibles de mi negocio solo los vea quien realmente debe verlos, y no queden expuestos a todo el equipo                               |

**Escenario RF5.2.1**

| **Scenario: Acceso restringido del rol Vendedor a datos financieros** | |
| --- | | --- |
| **Given** | un miembro del equipo tiene el rol de Vendedor y ha iniciado sesión en ROAX |
| **When** | intenta acceder a las secciones de rentabilidad por campaña, costos de pauta o márgenes del producto |
| **Then** | el sistema le deniega el acceso y muestra un mensaje indicando que esa información solo está disponible para Administradores |
| **And** | el intento de acceso queda registrado en el log de actividad de la cuenta |

**Escenario RF5.2.2**

| **Scenario: Asignación de roles por parte del Administrador** | |
| --- | | --- |
| **Given** | el dropshipper tiene rol de Administrador y tiene al menos un colaborador registrado en su cuenta de ROAX |
| **When** | accede al módulo de gestión de equipo y asigna o modifica el rol de un colaborador |
| **Then** | el sistema aplica los nuevos permisos de forma inmediata sin necesidad de reiniciar sesión |
| **And** | el colaborador solo puede ver y operar las secciones habilitadas para su rol desde ese momento |

**HU RF6.1 - Transparencia de costos antes de ejecutar cambios de presupuesto**

| **Historia N°:** | RF6.1                                                                                                                                                          |
| ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Yo como**      | dropshipper                                                                                                                                                    |
| **Quiero**       | que el sistema me informe previamente sobre cualquier costo adicional, comisión o cargo asociado a cambios automáticos de presupuesto o integraciones externas |
| **Para**         | tomar decisiones informadas y evitar gastos inesperados en mi operación publicitaria                                                                           |

**Escenario RF6.1.1**

| **Scenario: Notificación de costo adicional antes de aumentar presupuesto** | |
| --- | | --- |
| **Given** | el dropshipper tiene campañas activas y el sistema detecta una oportunidad de aumentar automáticamente el presupuesto de pauta |
| **When** | la acción implica costos adicionales por integración, procesamiento o comisiones de terceros |
| **Then** | el sistema muestra una notificación detallando el costo estimado antes de ejecutar el cambio |
| **And** | solicita confirmación explícita del usuario para continuar con la operación |

**Escenario RF6.1.2**

| **Scenario: Visualización de costos asociados a integraciones externas** | |
| --- | | --- |
| **Given** | el dropshipper desea conectar una nueva integración externa dentro de ROAX |
| **When** | el dropshipper inicia el proceso de conexión con una nueva integración dentro de ROAX |
| **Then** | el sistema informa claramente el tipo de costo, su frecuencia y el servicio asociado antes de completar la integración |
| **And** | el usuario puede aceptar o cancelar el proceso antes de que se genere cualquier cargo |

**HU RF6.2 - Interfaz Conversacional de ROAX vía WhatsApp**

| **Historia N°:** | RF6.2                                                                                                                                                                      |
| ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Yo como**      | dropshipper                                                                                                                                                                |
| **Quiero**       | interactuar con el sistema a través de un chatbot inteligente en WhatsApp                                                                                                  |
| **Para**         | supervisar mis campañas, recibir diagnósticos y ejecutar acciones usando lenguaje natural, sin tener que entrar a una plataforma externa o interpretar gráficos complejos. |

**Escenario RF6.2.1**

| **Scenario: Ejecución de acción inmediata mediante comando en WhatsApp** | |
| --- | | --- |
| **Given** | que el usuario recibe un mensaje de alerta del bot en WhatsApp informando que una campaña tiene un rendimiento deficiente . |
| **When** | el usuario responde al chat con un comando natural como "Pausa esa campaña". |
| **Then** | el sistema procesa el lenguaje y ejecuta la instrucción de pausa en la plataforma publicitaria de forma instantánea. |
| **And** | el bot responde confirmando: "Listo, campaña pausada exitosamente." |

**Escenario RF6.2.2**

| **Scenario: Consulta de métricas de forma conversacional** | |
| --- | | --- |
| **Given** | que el usuario ha iniciado sesión en la aplicación móvil de ROAX. |
| **When** | envía un mensaje al bot preguntando: "¿Cómo vamos hoy de rentabilidad?" o "¿Cuál es el margen neto?" |
| **Then** | el sistema interpreta la intención y cruza los datos del negocio en tiempo real |
| **And** | el bot responde con un resumen conciso y fácil de leer detallando las métricas directamente en el chat. |

**HU RF7.1 - Registro de inventario para decisiones contextualizadas**

| **Historia N°:** | RF7.1                                                                                                                                                          |
| ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Yo como**      | dropshipper                                                                                                                                                    |
| **Quiero**       | que el sistema se sincronice automáticamente con el inventario real de mis productos en mis plataformas de venta y pause las campañas cuando el stock se agote |
| **Para**         | no seguir gastando presupuesto en publicidad de productos que ya no puedo entregar y reactivar las campañas en cuanto reabastezca el inventario                |

**Escenario RF7.1.1**

| **Scenario: Pausa automática de campaña por agotamiento de stock** | |
| --- | | --- |
| **Given** | el dropshipper tiene una campaña activa promocionando un producto que aún tiene stock en su tienda integrada |
| **When** | el sistema detecta que el stock disponible del producto cae a cero o por debajo del umbral mínimo configurado |
| **Then** | el sistema pausa automáticamente la campaña asociada a ese producto |
| **And** | registra la acción en el historial indicando el motivo (agotamiento de inventario) y notifica al dropshipper para que reabastezca |

**Escenario RF7.1.2**

| **Scenario: Reactivación de campaña tras reposición de inventario** | |
| --- | | --- |
| **Given** | el dropshipper tenía una campaña pausada automáticamente por falta de stock y ha reabastecido el producto en su tienda |
| **When** | el sistema detecta que el inventario del producto vuelve a estar por encima del umbral mínimo configurado |
| **Then** | el sistema reactiva automáticamente la campaña previamente pausada |
| **And** | notifica al dropshipper que la campaña ha vuelto a estar activa, indicando la fecha y la cantidad de stock detectada |

**HU RF7.2 - Registro de restricciones financieras del negocio**

| **Historia N°:** | RF7.2                                                                                                                                           |
| ---------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| **Yo como**      | administrador                                                                                                                                   |
| **Quiero**       | poder registrar las restricciones financieras de mi negocio como deudas activas, límites de flujo de caja y presupuesto máximo mensual de pauta |
| **Para**         | que la IA no me recomiende aumentos de presupuesto que mi negocio no puede asumir                                                               |

**Escenario RF7.2.1**

| **Scenario: Registro de parámetros financieros del negocio** | |
| --- | | --- |
| **Given** | el administrador tiene sesión iniciada en ROAX |
| **When** | accede al módulo de configuración financiera y registra el presupuesto máximo de pauta, el flujo de caja disponible y las deudas activas |
| **Then** | el sistema guarda esos parámetros como restricciones del negocio |
| **And** | los toma como referencia para validar futuras recomendaciones de la IA |

**Escenario RF7.2.2**

| **Scenario: Bloqueo de recomendación que excede el límite financiero** | |
| --- | | --- |
| **Given** | el administrador ha registrado un presupuesto máximo mensual de pauta |
| **When** | la IA evalúa una recomendación de aumento de presupuesto que superaría ese límite |
| **Then** | el sistema bloquea automáticamente la recomendación |
| **And** | muestra al administrador una explicación clara indicando que la propuesta fue restringida por el techo financiero configurado |

**HU RF7.3 - Definición de buyer persona para alineamiento de recomendaciones**

| **Historia N°:** | RF7.3                                                                                                                            |
| ---------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| **Yo como**      | dropshipper                                                                                                                      |
| **Quiero**       | poder definir el perfil cualitativo de mi cliente ideal (buyer persona)                                                          |
| **Para**         | que las recomendaciones de creativos, segmentación y mensajes que me dé la IA estén alineadas con ese perfil y no sean genéricas |

**Escenario RF7.3.1**

| **Scenario: Registro de atributos del buyer persona** | |
| --- | | --- |
| **Given** | el dropshipper tiene sesión iniciada en ROAX |
| **When** | accede al módulo de buyer persona y registra rango de edad, intereses principales, ubicación geográfica y comportamiento de compra esperado |
| **Then** | el sistema guarda el perfil del cliente ideal asociado al negocio |
| **And** | ese perfil queda disponible para que la IA lo considere en sus recomendaciones |

**Escenario RF7.3.2**

| **Scenario: Recomendaciones alineadas al buyer persona definido** | |
| --- | | --- |
| **Given** | el dropshipper ha registrado el buyer persona de su negocio |
| **When** | la IA genera una recomendación sobre creativos, segmentación o horarios de pauta |
| **Then** | el sistema evalúa la pertinencia de la recomendación contra los atributos del buyer persona registrado |
| **And** | cada recomendación incluye una breve explicación de cómo se alinea con ese perfil |

**HU RF7.4**

| **Historia N°:** | RF7.4                                                                                                                                                                  |
| ---------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Yo como**      | dropshipper                                                                                                                                                            |
| **Quiero**       | que la IA considere tendencias externas del mercado, como variaciones estacionales, picos de búsqueda en Google Trends y comportamiento publicitario de mi competencia |
| **Para**         | recibir recomendaciones de pauta que se anticipen a oportunidades o riesgos del contexto externo, y no solo basadas en mi histórico interno                            |

**Escenario RF7.4.1**

| **Scenario: Recomendación de aumento de presupuesto por pico estacional detectado** | |
| --- | | --- |
| **Given** | el sistema está conectado a fuentes externas de tendencias del mercado y el dropshipper tiene campañas activas |
| **When** | el sistema detecta un pico de demanda estacional para una categoría de producto que el dropshipper está promocionando |
| **Then** | la IA genera una recomendación de aumento de presupuesto justificada con el dato externo detectado |
| **And** | la recomendación incluye una explicación clara del contexto que la motivó (por ejemplo, aumento del 60% en búsquedas de la categoría en Google Trends durante los últimos 7 días) |

**Escenario RF7.4.2**

| **Scenario: Alerta por movimiento publicitario agresivo de la competencia** | |
| --- | | --- |
| **Given** | el sistema monitorea el comportamiento publicitario de competidores definidos por el dropshipper a través de APIs públicas |
| **When** | detecta que un competidor directo aumentó significativamente su inversión publicitaria sobre un producto similar |
| **Then** | la IA genera una alerta contextual al dropshipper informando del movimiento de la competencia |
| **And** | propone ajustes posibles en su propia estrategia de pauta para no perder visibilidad en el mercado |

---
   
## 3.2 Casos de Uso (Datos y Decisiones)


### 3.2.1 Diagrama de Casos de Uso

![Caso de uso]()

> Pendiente por integración de diagramas de casos de uso entregados por el equipo correspondiente.


### 3.2.2 Formatos Bicolumnares 

[Formato Bicolumnar](https://docs.google.com/document/d/1Tl-pgph0c5_l7zp6FZbqnuXPiQ6JTkrJtpKxMOWy5VU/edit?usp=sharing)

---

## 4. RF2: Creatividades desde el rendimiento

## 4.1 Historias de Usuario

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


---

## 4. RF2: Subsistema B 

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
### Historia de Usuario 2

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

## 4.2 Caso de uso (RF1 - Alertas que Razonan)

### 4.2.1 Diagrama de Casos de Uso

![Caso de uso](Imagenes/RF2%20Alertas%20Inteligentes/CU1.jpg)


### 4.2.2 Formatos Bicolumnares 

[Formato Bicolumnar](https://docs.google.com/document/d/1I5PSUtAMPhLh_innqdz-A928Sz32RkF9yD_Muy9xxfQ/edit?usp=sharing)

---

## 4.2 Caso de uso (RF2 - Alertas que Razonan)

### 4.2.1 Diagrama de Casos de Uso

![Caso de uso](Imagenes/RF2%20Alertas%20Inteligentes/CU2.jpg)


### 4.2.2 Formatos Bicolumnares 

[Formato Bicolumnar](https://docs.google.com/document/d/1kVJW99QKqUjJ05fXVkuUhwnXC7O3ZaBO1HmUkGof8d8/edit?usp=sharing)

---

## 4.2 Caso de uso (RF3 - Alertas que Razonan)

### 4.2.1 Diagrama de Casos de Uso

![Caso de uso](Imagenes/RF2%20Alertas%20Inteligentes/CU3.jpg)


### 4.2.2 Formatos Bicolumnares 

[Formato Bicolumnar](https://docs.google.com/document/d/1WLJjKFNwn3YCgUH8YzMMTfWK1elJ8eaHyZ5qe-wIuTU/edit?usp=sharing)

---

## 4.2 Caso de uso (RF4 - Alertas que Razonan)

### 4.2.1 Diagrama de Casos de Uso

![Caso de uso](Imagenes/RF2%20Alertas%20Inteligentes/CU4.jpg)


### 4.2.2 Formatos Bicolumnares 

[Formato Bicolumnar](https://docs.google.com/document/d/1rLeiiLk7PSYA9xlqEuBpiSFBjkFmd7_GfpwAof3BpNo/edit?usp=sharing)

---


## 5. RF3: Creatividades desde el rendimiento
   
### 5.1 Historias de Usuario

## 3. RF1: Subsistema A — Gestión de Usuarios

HU3.1.1 — Registro de usuario en ROAX

| Campo                       | Contenido                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| --------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Título**                  | Registro de usuario en ROAX                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Historia**                | Yo, como dueño de un e-commerce, quiero registrarme en ROAX con mis datos básicos, para poder acceder a la plataforma y comenzar a analizar mis campañas.                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Criterios de aceptación** | **Scenario 1: Registro exitoso con datos válidos**<br>**Given** el usuario se encuentra en la página de registro<br>**When** ingresa nombre, correo válido y contraseña segura<br>**Then** el sistema crea la cuenta y asigna un ID único.<br><br>**Scenario 2: Registro fallido por correo ya registrado**<br>**Given** el usuario se encuentra en la página de registro<br>**And** el correo ya existe en la base de datos<br>**When** intenta registrarse con ese correo<br>**Then** el sistema rechaza el registro y muestra "El correo ya está registrado". |

---

HU3.1.2 — Asignación de rol organizacional

| Campo                       | Contenido                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| --------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Título**                  | Asignación de rol organizacional                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Historia**                | Yo, como administrador de una organización en ROAX, quiero asignar roles a los usuarios del equipo, para controlar qué funcionalidades pueden usar.                                                                                                                                                                                                                                                                                                                                                       |
| **Criterios de aceptación** | **Scenario 1: Asignación exitosa de rol**<br>**Given** el administrador está en la sección de gestión de usuarios<br>**When** asigna un rol válido a un usuario<br>**Then** el sistema guarda el rol y aplica los permisos correspondientes.<br><br>**Scenario 2: Asignación fallida por rol inválido**<br>**Given** el administrador está en la sección de gestión de usuarios<br>**When** asigna un rol que no existe en el sistema<br>**Then** el sistema rechaza la acción y muestra "Rol no válido". |

---

### 5.2 Casos de uso

---

3.2.1 Diagrama de casos de uso

<img width="1421" height="762" alt="image" src="https://github.com/user-attachments/assets/ca2a671d-0f5e-49b3-af80-97151619465c" />

---

3.2.2 Formato bicolumanr

[Formato Bicolumnar Diagrama A_ID CU-A-0_CU-A-02.pdf](https://github.com/user-attachments/files/28204607/Formato.Bicolumnar.Diagrama.A_ID.CU-A-0_CU-A-02.pdf)

---

## 4. RF2: Subsistema B — Perfilamiento del Cliente

### 5.1 Historias de usuario

HU4.1.1 — Consulta de perfil 360° del consumidor
| Campo                       | Contenido                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| --------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Título**                  | Consulta de perfil 360° del consumidor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Historia**                | Yo, como Marketing Manager, quiero consultar un perfil único de cada consumidor, para entender su comportamiento real de compra y segmentarlo mejor.                                                                                                                                                                                                                                                                                                                                                                                           |
| **Criterios de aceptación** | **Scenario 1: Consulta exitosa del perfil consolidado**<br>**Given** el usuario está autenticado en ROAX<br>**And** el consumidor existe en la base de datos<br>**When** busca el consumidor por correo o ID<br>**Then** el sistema muestra el perfil unificado con historial, demografía y preferencias.<br><br>**Scenario 2: Consulta fallida por consumidor inexistente**<br>**Given** el usuario está autenticado en ROAX<br>**When** busca un consumidor con un ID inexistente<br>**Then** el sistema muestra "Consumidor no encontrado". |

---

HU4.1.2 — Consolidación automática de datos del consumidor
| Campo                       | Contenido                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| --------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Título**                  | Consolidación automática de datos del consumidor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Historia**                | Yo, como analista de datos, quiero que el sistema consolide automáticamente datos del consumidor desde varias fuentes, para evitar duplicidad y mejorar el análisis.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Criterios de aceptación** | **Scenario 1: Consolidación exitosa con coincidencia de identificador**<br>**Given** el consumidor existe en dos fuentes conectadas<br>**And** ambas fuentes coinciden en el correo del consumidor<br>**When** el sistema ejecuta el proceso de consolidación<br>**Then** el sistema fusiona la información en un único perfil y registra las fuentes.<br><br>**Scenario 2: Consolidación fallida por falta de coincidencia**<br>**Given** existen consumidores en dos fuentes conectadas<br>**But** no existe coincidencia en correo o identificador<br>**When** el sistema intenta consolidar la información<br>**Then** el sistema mantiene los perfiles separados y marca el caso como "Sin coincidencia". |

---

### 5.2 Casos de uso

---

4.2.1 Diagrama de casos de uso 

<img width="821" height="359" alt="Subsistema B jpg" src="https://github.com/user-attachments/assets/7c595e39-cebd-4d50-b581-4ec1412d05ea" />

---
4.2.2 Formato bicolumnar

[Formato Bicolumnar Diagrama B_CU-B-0_CU-B-02.pdf](https://github.com/user-attachments/files/28204612/Formato.Bicolumnar.Diagrama.B_CU-B-0_CU-B-02.pdf)

---

## 5. RF3: Subsistema C — Reportes de Inteligencia de Negocio

### 5.1 Historias de usuario

---


HU5.1.1 — Generación de reporte financiero y operativo
| Campo                       | Contenido                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| --------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Título**                  | Generación de reporte financiero y operativo                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Historia**                | Yo, como dueño del e-commerce, quiero generar reportes financieros y operativos, para conocer la rentabilidad real del negocio.                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Criterios de aceptación** | **Scenario 1: Generación exitosa de reporte**<br>**Given** existen datos de ventas y campañas del periodo seleccionado<br>**When** el usuario solicita generar el reporte<br>**Then** el sistema genera el reporte y lo muestra en pantalla.<br><br>**Scenario 2: Generación fallida por falta de datos**<br>**Given** el usuario solicita un reporte de un periodo específico<br>**But** no existen datos suficientes para ese periodo<br>**When** el sistema intenta generar el reporte<br>**Then** el sistema muestra "No hay datos suficientes para generar el reporte". |

---

HU5.1.2 — Alerta por inventario bajo en producto promocionado
| Campo                       | Contenido                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| --------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Título**                  | Alerta por inventario bajo en producto promocionado                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Historia**                | Yo, como dueño del e-commerce, quiero recibir alertas cuando un producto promocionado tenga inventario bajo, para evitar gastar presupuesto en campañas sin stock.                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Criterios de aceptación** | **Scenario 1: Alerta enviada por inventario bajo**<br>**Given** un producto tiene una campaña activa asociada<br>**And** el inventario baja del umbral configurado<br>**When** el sistema detecta la reducción de stock<br>**Then** el sistema envía una notificación con el producto afectado y recomendación.<br><br>**Scenario 2: No se genera alerta si no hay campaña activa**<br>**Given** un producto tiene inventario bajo<br>**But** no está asociado a ninguna campaña activa<br>**When** el sistema analiza el inventario<br>**Then** el sistema no envía alertas relacionadas con pauta publicitaria. |

---

### 5.2 Casos de uso

---

5.2.1 Diagrama de casos de uso 

<img width="884" height="669" alt="Roax-3 jpg (2)" src="https://github.com/user-attachments/assets/b548cb96-d1f8-4e89-a34b-1a0067843135" />

---

5.2.2 Formato bicolumnar

[Formato Bicolumnar Diagrama C_ID CU-C-01_CU-C-02.pdf](https://github.com/user-attachments/files/28204618/Formato.Bicolumnar.Diagrama.C_ID.CU-C-01_CU-C-02.pdf)

---

## 6. RF4: Subsistema D — Optimización de Campañas con IA

### 5.1 Historias de usuario

HU6.1.1 — Análisis de rendimiento de creatividades
| Campo                       | Contenido                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Título**                  | Análisis de rendimiento de creatividades                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Historia**                | Yo, como Marketing Manager, quiero analizar el rendimiento de las creatividades usadas en mis campañas, para identificar qué anuncios convierten mejor.                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Criterios de aceptación** | **Scenario 1: Análisis exitoso de creatividades**<br>**Given** existen campañas con anuncios activos y creatividades asociadas<br>**When** el usuario consulta el módulo de creatividades<br>**Then** el sistema muestra métricas como CTR, CPA, ROAS y tasa de conversión por creatividad.<br><br>**Scenario 2: Análisis fallido por falta de creatividades**<br>**Given** el usuario entra al módulo de creatividades<br>**But** no existen anuncios o creatividades registradas en el sistema<br>**When** solicita el análisis<br>**Then** el sistema muestra "No hay creatividades disponibles para analizar". |


---

HU6.1.2 — Propuesta automática de creatividad mejorada
| Campo                       | Contenido                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| --------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Título**                  | Propuesta automática de creatividad mejorada                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Historia**                | Yo, como dueño de e-commerce, quiero recibir propuestas de nuevas creatividades basadas en anuncios exitosos, para mejorar mis campañas sin depender únicamente de prueba y error.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Criterios de aceptación** | **Scenario 1: Propuesta generada con historial suficiente**<br>**Given** existen creatividades históricas con datos de rendimiento registrados<br>**When** el usuario solicita una propuesta de creatividad mejorada<br>**Then** el sistema genera la propuesta y muestra un score de rendimiento esperado.<br><br>**Scenario 2: Propuesta fallida por falta de historial**<br>**Given** el usuario solicita una propuesta de creatividad mejorada<br>**But** no existen suficientes creatividades históricas para comparación<br>**When** el sistema intenta generar la propuesta<br>**Then** el sistema muestra "No hay suficientes datos históricos para generar propuestas". |

---

## 7. Subsistema E — Integración de APIs Externas

### 5.1 Historias de usuario

HU7.1.1 — Conexión con plataforma externa mediante API
| Campo                       | Contenido                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| --------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Título**                  | Conexión con plataforma externa mediante API                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Historia**                | Yo, como usuario de ROAX, quiero conectar mi cuenta con plataformas externas como Meta Ads, Shopify o Dropi, para que el sistema obtenga automáticamente datos de campañas y ventas reales.                                                                                                                                                                                                                                                                                                                                                                                       |
| **Criterios de aceptación** | **Scenario 1: Conexión exitosa con plataforma externa**<br>**Given** el usuario se encuentra en el módulo de integraciones<br>**When** autoriza el acceso mediante credenciales válidas (OAuth)<br>**Then** el sistema confirma la conexión y comienza la sincronización automática.<br><br>**Scenario 2: Conexión fallida por autorización denegada**<br>**Given** el usuario se encuentra en el módulo de integraciones<br>**When** rechaza permisos o la plataforma externa retorna error de autenticación<br>**Then** el sistema muestra "No fue posible conectar la cuenta". |

---

### 5.2 Casos de uso

---

7.2.1 Diagramas de casos de uso

<img width="981" height="589" alt="Use Case Diagram2" src="https://github.com/user-attachments/assets/f059d78f-2bbd-4fb7-92ab-675903f04064" />

---

7.2.2 Formatos bicolumnares

[Formato Bicolumnar v1.0_Subsitema E_ID UC7.2.3.pdf](https://github.com/user-attachments/files/28204154/Formato.Bicolumnar.v1.0_Subsitema.E_ID.UC7.2.3.pdf)

[Formato Bicolumnar v1.0_Subsistema E_ID UC7.2.4.pdf](https://github.com/user-attachments/files/28204158/Formato.Bicolumnar.v1.0_Subsistema.E_ID.UC7.2.4.pdf)

---

## 6. RF4: Confianza Progresiva
   
### 6.1 Historias de Usuario
  

# 3. RF13 — Agente Conversacional Visual (ACV)


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

### 6.2 Caso de uso

## 6.2.1 Diagrama de Casos de Uso - 01-RF13

![Caso de uso 01-RF13](Imagenes/RF4-ConfianzaProgresiva/Caso%20de%20uso%2001.jpeg)

## 6.2.1 Diagrama de Casos de Uso - RF13

![Caso de uso 02-RF13](Imagenes/RF4-ConfianzaProgresiva/Caso%20de%20uso%2002.jpeg)


## 6.2.2 Formatos Bicolumnares -01-RF13

[Formato Bicolumnar-01-RF13](https://docs.google.com/document/d/1TDo1TTdEj_wKEtHp9ctVsHX_yG9c6Bq6nMTPyKIl7fE/edit?usp=sharing)

## 6.2.2 Formatos Bicolumnares - 02-RF13

[Formato Bicolumnar-02-RF13](https://docs.google.com/document/d/1W9J1i2ecVRGP5G9hOKJs7YT8tL1P38t-gC1fvb_BG3k/edit?usp=sharing)



---

## 6.1 Historias de Usuario

# 4. RF14 — Recomendaciones Inteligentes (REC)

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


## 6.2 Caso de uso 

## 6.2.1 Diagrama de Casos de Uso  01-RF14:

![Caso de uso 01-RF14](Imagenes/RF4-ConfianzaProgresiva/Caso%20de%20uso%2003.jpeg)


## 6.2.1 Diagrama de Casos de Uso  02-RF14:

![Caso de uso 02-RF14](Imagenes/RF4-ConfianzaProgresiva/Caso%20de%20uso%2004.jpeg)


## 6.2.2 Formatos Bicolumnares-01-RF14:

[Formato Bicolumnar-01-RF14](https://docs.google.com/document/d/1XEnIszNS_L7ecwf0LtUeyBp6_ZerAuZBfnwhDKyjlcs/edit?usp=sharing)

## 6.2.2 Formatos Bicolumnares-02-RF14:

[Formato Bicolumnar-02-RF14](https://docs.google.com/document/d/1-K1FWEDIBLcpTYH0QG6UmPqgaPHUBNcKKdLmWMUeu2A/edit?usp=sharing)





---

## 6.1 Historias de Usuario

# 5. RF15 — Gestión de Alertas (ALR)

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

## 6.2 Caso de uso 

## 6.2.1 Diagrama de Casos de Uso  01-RF15:

![Caso de uso 01-RF15](Imagenes/RF4-ConfianzaProgresiva/Caso%20de%20uso%2005.jpeg)


## 6.2.1 Diagrama de Casos de Uso 02-RF15_

![Caso de uso 02-RF15](Imagenes/RF4-ConfianzaProgresiva/Caso%20de%20uso%2006.jpeg)


## 6.2.2 Formatos Bicolumnares-01-RF15

[Formato Bicolumnar-01-RF15](https://docs.google.com/document/d/1tnP73K3gOLi3lbml82Woqx60uFBn9MJfaYvp_luhMEg/edit?usp=sharing)

## 6.2.2 Formatos Bicolumnares-02-RF15

[Formato Bicolumnar-02-RF15](https://docs.google.com/document/d/1JD7duImYBW1lOvTrh6khlGdWskXr-8m9sPR6lQ6Sl3E/edit?usp=sharing)

---

## 6.1 Historias de Usuario

# 6. RF16 — Retroalimentación y Aprendizaje (RFA)

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

## 6.2 Caso de uso 

### 6.2.1 Diagrama de Casos de Uso

![Caso de uso 02-RF16](Imagenes/RF4-ConfianzaProgresiva/Caso%20de%20uso%2007.jpeg)

## 6.2.2 Formatos Bicolumnares-01-RF16

[Formato Bicolumnar-01-RF16](https://docs.google.com/document/d/1iAuLzWd_MS7xk6nPBQ9Vc4ATOAfWvXaoF6ExM6D663c/edit?usp=sharing)

## 6.2.2 Formatos Bicolumnares-02-RF16

[Formato Bicolumnar-02-RF16](https://docs.google.com/document/d/1XDNQ0x9D_c9VJY83ohNyv0WCq8bmWZJhL6SQxBMDttM/edit?usp=sharing)

## 7. Backlog

## 8. MockUp (Aún no solicitado)
   8.1 Descripción General
   8.2 Enlace MockUp
