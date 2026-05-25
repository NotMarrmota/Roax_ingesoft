# DOCUMENTO DE ESPECIFICACIÓN DE REQUERIMIENTOS

## <ROAX>

---

## INTEGRANTES

- MARIA JOSE SANCHEZ 
- MARIANA LUCIA GALEANO
- ESTEBAN BERNAL
- JUAN JOSE MOTATO
- SAMUEL PALMA
- SANTIAGO MILLAN

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

En esta sección se describen y analizan los requerimientos del proyecto “ROAX Creatividades desde el Rendimiento”, un módulo inteligente dentro de la plataforma ROAX que permite conectar creatividades publicitarias generadas con IA con datos reales de desempeño (CTR, CPA, ROAS, conversiones, ventas), con el fin de mejorar campañas futuras y predecir el rendimiento esperado de nuevos anuncios.

El levantamiento de requerimientos se realizó a partir del análisis del brief del producto ROAX y entrevistas realizadas con la gerente del sistema, identificando requerimientos funcionales de alto nivel orientados a: gestión de usuarios, perfilamiento de clientes, reportes del negocio y optimización de campañas basada en inteligencia artificial.

### 1.2 Contexto del proyecto

<DESCRIPCIÓN GENERAL DE LAS FUNCIONALIDADES DEL PROYECTO>

ROAX es una plataforma de inteligencia de negocio para e-commerce que integra datos de publicidad digital (Meta Ads y próximamente TikTok Ads) con datos reales de ventas provenientes de canales digitales como Shopify, Dropi, WooCommerce y Tienda Nube, con el fin de calcular la rentabilidad real de un negocio. ROAX actualmente cuenta con más de 3.600 usuarios registrados, dashboards de métricas, alertas y generación de anuncios con inteligencia artificial mediante su producto ROAX Ads.

Sin embargo, actualmente ROAX se centra en mostrar información y métricas, respondiendo principalmente a la pregunta: “¿Qué está pasando?”, mientras que el usuario requiere que la plataforma evolucione hacia un sistema inteligente que responda: “¿Qué debo hacer para mejorar mi negocio?”, sugiriendo acciones concretas, automatizando decisiones y aprendiendo del historial del negocio.

En este contexto, el reto técnico asignado es el Reto 3: Creatividades desde el rendimiento, el cual busca que las creatividades generadas por ROAX Ads estén conectadas directamente a los datos reales de conversión, permitiendo que el sistema genere anuncios basados en lo que ya ha funcionado, e incluso que analice creatividades existentes para predecir su desempeño futuro.

### 1.3 Requisitos

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


### 1.4 Subespecificación por subsistemas

Subsistema A — Gestión de Usuarios
<ESCRIBIR_REQUERIMIENTOS_SUBESPECIFICADOS_POR_SUBSISTEMA_PARA_TODOS_SUS_REQUERIMIENTOS>
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

### 1.5 Tabla de asignación a subsistemas

| Requerimiento | Subsistema A Usuarios | Subsistema B Perfil Cliente | Subsistema C Reportes | Subsistema D IA Creatividades | Subsistema E APIs |
| ------------- | --------------------- | --------------------------- | --------------------- | ----------------------------- | ----------------- |
| RF1           | X                    |                             |                       |                               |                   |
| RF1.1         | X                    |                             |                       |                               |                   |
| RF1.1.1       | X                    |                             |                       |                               |                   |
| RF2           |                       | X                          |                       |                               | X                |
| RF2.1         |                       | X                          |                       |                               | X                |
| RF2.1.1       |                       | X                          |                       | X                            | X                |
| RF3           |                       |                             | X                    |                               | X                |
| RF3.1         |                       |                             | X                    |                               | X                |
| RF3.1.1       |                       |                             | X                    |                               | X                |
| RF3.1.2       |                       |                             | X                    | X                            | X                |
| RF4           |                       | X                          | X                    | X                            | X                |
| RF4.1         |                       |                             |                       | X                            | X                |
| RF4.1.1       |                       | X                          |                       | X                            | X                |


---

## 2. PESTLE

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


## 3. RF1: Subsistema A — Gestión de Usuarios

### 3.1 Historias de usuario
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

### 3.2 Casos de uso

---

3.2.1 Diagrama de casos de uso

<img width="1421" height="762" alt="image" src="https://github.com/user-attachments/assets/ca2a671d-0f5e-49b3-af80-97151619465c" />

---

## 4. RF2: Subsistema B — Perfilamiento del Cliente

### 4.1 Historias de usuario

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

### 4.2 Casos de uso

---

4.2.1 Diagrama de casos de uso 

<img width="821" height="359" alt="Subsistema B jpg" src="https://github.com/user-attachments/assets/7c595e39-cebd-4d50-b581-4ec1412d05ea" />

---

## 5. RF3: Subsistema C — Reportes de Inteligencia de Negocio

### 5.1 Historias de usuario

---

## 5. RF3: Subsistema C <<Nombre el Subsistema>>

### 5.1 Historias de usuario

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

## 6. RF4: Subsistema D — Optimización de Campañas con IA

### 6.1 Historias de usuario

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

### 7.1 Historias de usuario

HU7.1.1 — Conexión con plataforma externa mediante API
| Campo                       | Contenido                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| --------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Título**                  | Conexión con plataforma externa mediante API                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Historia**                | Yo, como usuario de ROAX, quiero conectar mi cuenta con plataformas externas como Meta Ads, Shopify o Dropi, para que el sistema obtenga automáticamente datos de campañas y ventas reales.                                                                                                                                                                                                                                                                                                                                                                                       |
| **Criterios de aceptación** | **Scenario 1: Conexión exitosa con plataforma externa**<br>**Given** el usuario se encuentra en el módulo de integraciones<br>**When** autoriza el acceso mediante credenciales válidas (OAuth)<br>**Then** el sistema confirma la conexión y comienza la sincronización automática.<br><br>**Scenario 2: Conexión fallida por autorización denegada**<br>**Given** el usuario se encuentra en el módulo de integraciones<br>**When** rechaza permisos o la plataforma externa retorna error de autenticación<br>**Then** el sistema muestra "No fue posible conectar la cuenta". |

---

### 7.2 Casos de uso

---

7.2.1 Diagramas de casos de uso

<img width="981" height="589" alt="Use Case Diagram2" src="https://github.com/user-attachments/assets/f059d78f-2bbd-4fb7-92ab-675903f04064" />

---

## 6. Backlog

| ID | Historia de Usuario | Prioridad |
|----|--------------------|----------|
| 1  | Registro de Usuario | Alta     |

---

## 7. MockUp

### 7.1 Descripción general

Se presenta el MVP que cumple con todas las funcionalidades propuestas. Estas no se referencian en los formatos bicolumnares debido a la extensión del proyecto.

### 7.2 Enlace MockUp

<<Enlace MockUp>>
