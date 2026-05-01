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

## Tabla de Contenido

1. Especificación de Requerimientos
   - 1.1 Descripción general
   - 1.2 Contexto del proyecto
   - 1.3 Requisitos
   - 1.4 Subespecificación por subsistemas
   - 1.5 Tabla de asignación a subsistemas
2. PESTLE
3. Backlog
4. MockUp
   - 4.1 Descripción general
   - 4.2 Enlace MockUp

---

## 1. Especificación de Requerimientos

### 1.1 Descripción General

El presente documento describe el análisis, diseño y propuesta de solución para el **Reto 4: Confianza Progresiva** del proyecto **ROAX by Dropi**, desarrollado en el marco de la asignatura de Ingeniería de Software.

El reto consiste en diseñar un sistema que permita a la plataforma ROAX pasar de mostrar datos a tomar decisiones concretas por el usuario, construyendo gradualmente la confianza necesaria para que este delegue acciones críticas de su negocio a la inteligencia artificial. Para ello se identificaron requerimientos funcionales y no funcionales, se propuso una arquitectura de solución y se desarrolló un prototipo visual del agente inteligente.

---

### 1.2 Contexto del Proyecto

ROAX by Dropi es una plataforma de inteligencia de negocio para e-commerce que integra datos de publicidad digital (Meta Ads, y próximamente TikTok) con datos reales de ventas y logística (Shopify, Tienda Nube, WooCommerce y Dropi), con el objetivo de calcular la rentabilidad real de un negocio digital.

La plataforma actualmente cuenta con más de 5.600 usuarios registrados y opera en dos modalidades: como módulo interno dentro de Dropi, y como plataforma externa independiente en app.roaxai.com, que es el foco del presente proyecto.

Hoy, ROAX funciona principalmente como una plataforma de reportería: conecta fuentes de datos, calcula métricas clave como ROAS, CPA, CTR, CPC y CPM, y genera alertas sobre el rendimiento de las campañas. Sin embargo, el modelo actual presenta una limitación estructural: **muestra información pero no ayuda a tomar decisiones**. El usuario debe interpretar solo qué significan los números y qué hacer con ellos, lo cual genera una alta fricción en la adopción del producto.

Con el avance de la inteligencia artificial, las plataformas de data enfrentan el reto de evolucionar: pasar de responder *"¿qué está pasando?"* a responder *"¿qué debo hacer para mejorar mi negocio?"*. En este contexto, ROAX plantea su **Refactor 2026**, un proceso de rediseño profundo orientado a convertir la IA en el motor central de decisiones de la plataforma.

Dentro de este refactor se definen cuatro retos técnicos. El presente proyecto aborda el **Reto 4: Confianza Progresiva**, cuyo foco es diseñar el mecanismo mediante el cual un sistema de recomendaciones basado en IA logra que el usuario confíe en él, actúe sobre sus sugerencias, y permita que el sistema aprenda y mejore con el tiempo.

Este reto cobra especial relevancia dado el contexto del usuario de ROAX: un emprendedor o marca que invierte en promedio entre 1.500 y 2.000 dólares mensuales en publicidad digital, que opera en múltiples plataformas simultáneamente, y que ya ha desarrollado una desconfianza hacia las recomendaciones automáticas de Meta, debido a que estas priorizan el gasto publicitario por encima de la rentabilidad real del negocio.

---

### 1.3 Requisitos

#### Requerimientos Funcionales

| # | Requerimiento |
|---|---------------|
| **R1** | **El sistema debe identificar automáticamente campañas con bajo rendimiento** mediante el análisis de métricas claves como ROAS, CPA, tasa de conversión y comportamiento histórico |
| **R2** | **El sistema debe generar recomendaciones sobre campañas** (pausar, escalar o modificar) basadas en análisis de datos y patrones detectados |
| **R3** | **El sistema debe presentar una explicación clara y basada en datos** que justifique cada recomendación, incluyendo comparaciones con el rendimiento histórico y tendencias relevantes |
| **R4** | **El sistema debe permitir al usuario visualizar y explorar datos** que respaldan cada recomendación, incluyendo métricas, variaciones temporales y análisis de embudo de conversión |
| **R5** | **El sistema debe proporcionar una estimación de impacto esperado** de la recomendación antes de su ejecución, expresada en métricas como ROAS, CPA o ingresos |
| **R6** | **El sistema debe permitir al usuario interactuar con cada recomendación** mediante las opciones aplicar, rechazar o posponer la acción sugerida |
| **R7** | **El sistema debe permitir al usuario proporcionar retroalimentación explícita** sobre las recomendaciones, indicando si fueron útiles, incorrectas o irrelevantes |
| **R8** | **El sistema debe ajustar sus futuras recomendaciones** en función del comportamiento del usuario, considerando acciones como aceptación, rechazo o ignorar recomendaciones |
| **R9** | **El sistema debe permitir configurar niveles de automatización**, desde recomendaciones manuales hasta ejecución automática de acciones, según la preferencia del usuario |
| **R10** | **El sistema debe notificar al usuario sobre situaciones críticas** que requieran acción inmediata, priorizando aquellas con mayor impacto en el negocio |
| **R11** | **El sistema debe agrupar y priorizar recomendaciones** en función de su impacto potencial, evitando la saturación de información al usuario |
| **R12** | **El sistema debe solicitar y almacenar información cualitativa del negocio** (inventarios, costos, perfil de cliente) para mejorar la precisión de las recomendaciones |
| **R13** | **El sistema debe permitir la comunicación con el usuario** mediante un agente conversacional visual en tiempo real |

#### Requerimientos No Funcionales

| # | Requerimiento |
|---|---------------|
| **RNF1** | **Disponibilidad:** el sistema debe estar disponible 24/7 |
| **RNF2** | **Procesamiento en tiempo real:** el sistema debe procesar y analizar datos en tiempo real o con mínima latencia |
| **RNF3** | **Interfaz de usuario:** el sistema debe ofrecer una interfaz intuitiva, clara y orientada a la toma de decisiones |
| **RNF4** | **Portabilidad:** el sistema debe ser accesible desde múltiples dispositivos |
| **RNF5** | **Interacción por voz:** el sistema debe permitir interacción mediante audio, procesando comandos del usuario en tiempo real |
| **RNF6** | **Transparencia IA:** el sistema debe hacer visible cuando una recomendación es generada por inteligencia artificial |

---

### 1.4 Subespecificación por Subsistemas

*(Por completar)*

---

### 1.5 Tabla de Asignación a Subsistemas de Segundo Nivel

*(Por completar)*

---

## 2. PESTLE

*(Por completar)*

---

## 3. Backlog

*(Por completar)*

---

## 4. MockUp

### 4.1 Descripción General

*(Por completar)*

### 4.2 Enlace MockUp

*(Por completar)*