# DOCUMENTO DE ESPECIFICACIÓN DE REQUERIMIENTOS

## <NOMBRE DE LA PLATAFORMA DESARROLLADA>

## <NOMBRE DE LA EMPRESA / CLIENTE>

---

## INTEGRANTES

- David Altaminaro Altamirano
- Mariana Carmona Galvez
- Santiago Campo
- David Santiago García
- Mario Andrés Romero Rivera
- Andrés Vinasco

---

## Tabla de Contenido

1. Especificación de requerimientos  
   1.1 Descripción general  
   1.2 Contexto del proyecto  
   1.3 Requisitos  
   1.4 Subespecificación por subsistemas  
   1.5 Tabla de asignación a subsistemas  

2. PESTLE  
   2.1 Listado de requerimientos  

3. RF1: Subsistema A  
   3.1 Historias de usuario  
   3.2 Casos de uso  
     3.2.1 Diagrama de casos de uso  
     3.2.2 Formatos bicolumnares  

4. RF2: Subsistema B  
   4.1 Historias de usuario  
   4.2 Casos de uso  
     4.2.1 Diagrama de casos de uso  
     4.2.2 Formatos bicolumnares  

5. RF3: Subsistema C  
   5.1 Historias de usuario  
   5.2 Casos de uso  
     5.2.1 Diagrama de casos de uso  
     5.2.2 Formatos bicolumnares  

6. Backlog  

7. MockUp  
   7.1 Descripción general  
   7.2 Enlace MockUp  

---

## 1. Especificación de requerimientos

### 1.1 Descripción general

En esta sección se describirán y analizarán los requerimientos del proyecto titulado <NOMBRE_DEL_PROYECTO>, por medio de análisis con enfoque de entidades e historias de usuario.

### 1.2 Contexto del proyecto

<DESCRIPCIÓN GENERAL DE LAS FUNCIONALIDADES DEL PROYECTO>

**Ejemplo:**  
Las funcionalidades que este sistema ofrece son las referentes al módulo de contabilidad, encargado del proceso de recepción, verificación, corrección y aceptación de solicitudes monetarias. La aplicación permite el envío de solicitudes, seguimiento, cambio de estado y gestión posterior.

### 1.3 Requisitos

<DESCRIPCIÓN DE LOS REQUISITOS DE ALTO NIVEL>

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
### 1.4 Subespecificación por subsistemas

<ESCRIBIR_REQUERIMIENTOS_SUBESPECIFICADOS_POR_SUBSISTEMA_PARA_TODOS_SUS_REQUERIMIENTOS>
**Ejemplo:**
- APIR1.1 El sistema debe permitir conexión con API académica para validar promedio superior a 4.2.

### 1.5 Tabla de asignación a subsistemas

| Requisito | Subsistema | Descripción |
|----------|------------|-------------|
|          |            |             |

---

## 2. PESTLE
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

## 3. RF1: Subsistema A <<Nombre el Subsistema>>

### 3.1 Historias de usuario

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

### 4.2 Casos de uso

#### 4.2.1 Diagrama de casos de uso

#### 4.2.2 Formatos bicolumnares

<<Enlace Formatos bicolumnares>>

---

## 5. RF3: Subsistema C <<Nombre el Subsistema>>

### 5.1 Historias de usuario

# Historia de Usuario 1

**ID:** HU1  
**Título:** Registro de acciones tomadas sobre campañas

## Historia
Como usuario de la plataforma, quiero que el sistema registre las acciones realizadas manual o automáticamente sobre mis campañas para poder analizar posteriormente su impacto en el negocio.

---
## Criterios de Aceptación 

### Scenario: Registro exitoso de acción manual
-Given que el usuario modifica manualmente una campaña

-When la acción es confirmada

-Then el sistema registra la acción realizada

-And almacena la fecha, campaña afectada y tipo de acción


### Scenario: Registro de acción automática
-Given que el sistema ejecuta una recomendación automática

-When la acción es aplicada sobre una campaña

-Then el sistema registra la acción automaticamente

-And la asocia al análisis correspondiente

### Scenario: Registro fallido de acción manual por datos incompletos

-Given que el usuario modifica una campaña

-And la información de la acción no contiene datos válidos de la campaña afectada

-When la acción es confirmada

-Then el sistema no registra la acción aplicada

-And muestra un mensaje que la modificación es erronea o inválida


---
**ID:** HU2 
**Título:** Consulta de información histórica

## Historia

Como usuario de la plataforma, quiero consultar información histórica diaria y mensual para identificar tendencias y cambios en el comportamiento de mis campañas.

---

## Criterios de Aceptación 

### Scenario: Consulta de historial diario


-Given que existen registros históricos almacenados

-When el usuario selecciona una campaña y un rango de fechas

-Then el sistema muestra el comportamiento histórico diario

### Scenario: Consulta de historial mensual


-Given que existen datos históricos mensuales

-When el usuario consulta el resumen histórico

-Then el sistema presenta tendencias mensuales de rendimiento


---

**Prioridad:** Alta / Media / Baja

**Dependencias:**

---

### 5.2 Casos de uso

#### 5.2.1 Diagrama de casos de uso

#### 4.2.2 Formatos bicolumnares

<<Enlace Formatos bicolumnares>>

---

## 5. RF3: Subsistema C <<Nombre el Subsistema>>

### 5.1 Historias de usuario

**Nombre de la historia:**

**Descripción:**  Como [tipo de usuario] quiero [objetivo] para [beneficio].

**Criterios de aceptación:**

- Criterio 1
- Criterio 2
- Criterio 3

**Prioridad:** Alta / Media / Baja

**Dependencias:**

---

### 5.2 Casos de uso

#### 5.2.1 Diagrama de casos de uso

#### 5.2.2 Formatos bicolumnares

<<Enlace Formatos bicolumnares>>

---

## 6. RF3: Subsistema D <<Nombre el Subsistema>>

### 6.1 Historias de usuario

# Historia de Usuario 1

**ID:** HU1  
**Título:** Explicación detallada de recomendaciones IA

## Historia

Como usuario, quiero visualizar una explicación clara de cada recomendación para entender qué datos motivaron la sugerencia.

## Criterios de Aceptación

### Scenario: Visualización correcta de explicación

- Given que el sistema genera una recomendación

- When el usuario consulta el detalle de la sugerencia

- Then el sistema muestra una explicación asociada

- And presenta las métricas y tendencias utilizadas para generar la recomendación

**Prioridad:** Alta

**Dependencias:** RF4.1

---

# Historia de Usuario 2

**ID:** HU2  
**Título:** Visualización de nivel de confianza

## Historia

Como usuario, quiero conocer el nivel de confianza de una recomendación para decidir si debo aplicarla.

## Criterios de Aceptación

### Scenario: Consulta de nivel de confianza

- Given que el sistema genera una recomendación

- When el usuario revisa la sugerencia

- Then el sistema muestra un porcentaje o nivel de confianza asociado

- And explica brevemente cómo fue calculado

---

# Historia de Usuario 3

**ID:** HU3  
**Título:** Aplicación gradual de recomendaciones

## Historia

Como usuario, quiero aplicar parcialmente una recomendación para evaluar resultados antes de ejecutar cambios completos.

## Criterios de Aceptación

### Scenario: Aplicación parcial exitosa

- Given que existe una recomendación disponible

- When el usuario selecciona aplicación parcial

- Then el sistema ejecuta únicamente una parte de los cambios

- And registra la configuración aplicada

---

# Historia de Usuario 4

**ID:** HU4  
**Título:** Historial de decisiones sobre recomendaciones

## Historia

Como usuario, quiero consultar recomendaciones aceptadas, rechazadas o ignoradas para revisar decisiones anteriores y comprender cómo han impactado mis campañas.

## Criterios de Aceptación

### Scenario: Consulta exitosa del historial

- Given que existen recomendaciones registradas

- When el usuario accede al historial de recomendaciones

- Then el sistema muestra las recomendaciones junto con su estado

- And presenta la fecha y tiempo de respuesta del usuario

### Scenario: Historial vacío

- Given que no existen recomendaciones registradas

- When el usuario consulta el historial

- Then el sistema informa que no hay registros disponibles

**Prioridad:** Media

**Dependencias:** RF4.4

---

# Historia de Usuario 5

**ID:** HU5  
**Título:** Comparación de resultados antes y después de aplicar recomendaciones

## Historia

Como usuario, quiero visualizar las métricas antes y después de aplicar una recomendación para evaluar si realmente mejoró el rendimiento de mis campañas.

## Criterios de Aceptación

### Scenario: Comparación exitosa de resultados

- Given que una recomendación fue aplicada previamente

- When el usuario consulta el impacto generado

- Then el sistema muestra métricas anteriores y posteriores a la aplicación

- And presenta las variaciones obtenidas en el rendimiento de la campaña

### Scenario: Datos insuficientes para comparación

- Given que aún no existe suficiente información posterior a la aplicación

- When el usuario consulta el impacto de la recomendación

- Then el sistema informa que el análisis todavía no está disponible

**Prioridad:** Alta

**Dependencias:** RF4.5


## 7. Backlog

| ID | Historia de Usuario | Prioridad |
|----|--------------------|----------|
| 1  | Registro de Usuario | Alta     |

---

## 8. MockUp

### 8.1 Descripción general

Se presenta el MVP que cumple con todas las funcionalidades propuestas. Estas no se referencian en los formatos bicolumnares debido a la extensión del proyecto.

### 8.2 Enlace MockUp

<<Enlace MockUp>>
