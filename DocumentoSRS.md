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

## RF1. El sistema debe mostrar al usuario las campañas cuyo desempeño se encuentre por debajo de un umbral definido.
   
- RF1.1. El sistema debe calcular el desempeño de cada campaña utilizando métricas cuantificables definidas (por ejemplo: tasa de conversión, CTR, ROI) y compararlas contra un umbral configurado.
   
   - RF1.2 El sistema debe permitir al usuario definir y modificar los umbrales de desempeño mediante valores numéricos o porcentuales para cada métrica.
   
- RF1.3 El sistema debe permitir al usuario seleccionar las métricas que serán utilizadas para evaluar el desempeño de las campañas.
## RF4. El sistema debe construir confianza progresiva en las recomendaciones generadas por IA

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

El listado de requerimientos de PESTLE se organiza en torno a seis factores: Políticos (estabilidad gubernamental, políticas fiscales), Económicos (inflación, tasas de interés, crecimiento económico), Sociales (demografía, estilo de vida, tendencias culturales), Tecnológicos (innovación, automatización, acceso a la tecnología), Legales (normativas laborales, de competencia, de seguridad) y Ambientales (regulación ambiental, sostenibilidad, cambio climático).


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
