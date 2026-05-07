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

#### RF3. El sistema debe medir y aprender del impacto de las decisiones tomadas
- **RF3.1** El sistema debe registrar las acciones tomadas por el usuario o ejecutadas automáticamente a partir de recomendaciones.
  
- **RF3.2** El sistema debe evaluar el impacto de dichas acciones en métricas clave del negocio (por ejemplo: ventas, ROAS, conversiones).
  
- **RF3.3** El sistema debe ajustar futuras recomendaciones basándose en los resultados obtenidos previamente, mejorando su precisión con el tiempo.

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
## 🧩 Análisis PESTLE – RF1: Detección de campañas de bajo desempeño

| Dimensión | Hallazgo | Impacto | Requerimiento derivado |
|----------|----------|---------|-------------------------|
| P — Político | No existen lineamientos específicos en Colombia sobre transparencia en algoritmos que evalúan desempeño de campañas. | El sistema podría ser cuestionado si no justifica cómo clasifica una campaña como de bajo desempeño. | **RNFP-1-01:** El sistema debe permitir consultar las métricas, umbrales y reglas utilizadas para clasificar una campaña como de bajo desempeño, mostrando al menos: nombre de la métrica, valor calculado, umbral aplicado y resultado de la evaluación. |
| E — Económico | El cálculo frecuente de métricas sobre grandes volúmenes de campañas implica alto costo computacional. | Puede afectar la escalabilidad y costos operativos del sistema. | **RNFE-1-02:** El sistema debe calcular métricas de desempeño mediante procesamiento incremental o por lotes, reduciendo en al menos un 30% el tiempo de procesamiento respecto a un cálculo completo sobre todos los datos históricos. |
| S — Social | Usuarios no expertos pueden no comprender métricas como CTR, ROI o tasa de conversión. | Riesgo de mala interpretación del desempeño de campañas. | **RNFS-1-03:** El sistema debe mostrar una descripción textual comprensible (máximo 100 palabras) para cada métrica utilizada, accesible desde la interfaz de evaluación de campañas. |
| T — Tecnológico | La evaluación depende de la actualización oportuna de datos de campañas. | Datos desactualizados generan clasificaciones incorrectas. | **RNFT-1-04:** El sistema debe actualizar las métricas de desempeño de campañas con una latencia máxima de 5 minutos desde la recepción de nuevos datos, garantizando que al menos el 95% de las actualizaciones cumplan este límite. |
| L — Legal | El sistema maneja datos sensibles de negocio asociados a campañas. | Riesgo de incumplimiento de normativas de protección de datos. | **RNFL-1-05:** El sistema debe restringir el acceso a la información de desempeño de campañas mediante control de roles, garantizando que solo usuarios autorizados puedan visualizar o modificar dichos datos. |
| E — Ético | La clasificación automática influye en decisiones comerciales del usuario. | Clasificaciones poco transparentes pueden inducir decisiones erróneas. | **RNFEt-1-06:** El sistema debe indicar explícitamente si la clasificación de bajo desempeño fue generada por reglas del sistema o configuraciones del usuario, mostrando esta información en la vista de resultados de cada campaña. |

## 3. RF1: Subsistema A <<Nombre el Subsistema>>

### 3.1 Historias de usuario

**Nombre de la historia:**

**Descripción:** Como [tipo de usuario] quiero [objetivo] para [beneficio].

**Criterios de aceptación:**
- Criterio 1
- Criterio 2
- Criterio 3

**Prioridad:** Alta / Media / Baja

**Dependencias:**

---

### 3.2 Casos de uso

#### 3.2.1 Diagrama de casos de uso

#### 3.2.2 Formatos bicolumnares

<<Enlace Formatos bicolumnares>>

---

## 4. RF2: Subsistema B <<Nombre el Subsistema>>

### 4.1 Historias de usuario

**Nombre de la historia:**

**Descripción:** Como [tipo de usuario] quiero [objetivo] para [beneficio].

**Criterios de aceptación:**

- Criterio 1
- Criterio 2
- Criterio 3

**Prioridad:** Alta / Media / Baja

**Dependencias:**

---

### 4.2 Casos de uso

#### 4.2.1 Diagrama de casos de uso

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
