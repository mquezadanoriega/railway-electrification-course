# MÓDULO 5 · LECCIÓN 9
# CENTROS DE TRANSFORMACIÓN AÉREOS PARA INSTALACIONES ASOCIADAS (NAE 400)

## Documento base

> **Documento base:** NAE 400, «Montaje de centros de transformación aéreos para
> alimentación eléctrica de instalaciones asociadas», 1ª edición (jun 2024), 14 págs.
> Grupo de trabajo GT-300 · Propuesta: 25-jun-2024 · Aprobada por el Comité de
> Normativa (26-jun-2024). No deroga ningún documento normativo. Entró en vigor en
> la fecha de su aprobación.
>
> **Complementaria:** ET 03.364.506.0 — «Transformadores aéreos» (1ª ed., jun. 2025),
> 24 págs., GT-300. Fija las características y condiciones de suministro de los
> transformadores de distribución que se montan en los CT aéreos de la LAC.

---

## 1. RESULTADO DE APRENDIZAJE

Al terminar esta lección serás capaz de:

1. Explicar qué es un **centro de transformación (CT) aéreo** y qué instalaciones
   asociadas alimenta (calefacción de agujas, alumbrado de túneles, BTS, BTO,
   casetas técnicas PCA/PICV y edificios técnicos)
2. Identificar los **elementos** de la acometida (seccionador, fusible, pararrayos,
   transformador, envolvente, protecciones de BT) y su misión
3. Seleccionar el **transformador** (potencia, tensiones, conexión, refrigeración)
   según el tipo de acometida (Tabla 1 de la NAE 400)
4. Conocer los **tipos de poste** (X-3AV, X-5AV, XL-5AV, XLL-7AV) en función de la
   acometida y la potencia
5. Aplicar las **condiciones de montaje** (alturas mínimas, distancias, ubicación
   de la cuba y del portafusibles, posiciones sobre el poste)
6. Describir las **protecciones asociadas** y el **esquema de puesta a tierra**
   (pletina colectora, pararrayos, conexión al cable de tierra de la LAC)
7. Relacionar la NAE 400 con la **NAE 111** (cable de tierra/retorno), la serie
   **ET 03.364** y el **RD 337/2014 (ITC-RAT)**

---

## 2. RESUMEN EJECUTIVO

La NAE 400 especifica los requisitos de **montaje, ubicación y conexionado** de los
**transformadores de tensión aéreos** para las acometidas a instalaciones asociadas
de la Red Ferroviaria de Interés General (RFIG) gestionada por Adif y Adif AV. Estos
transformadores se instalan en **postes o estructuras portantes de la línea aérea de
contacto (LAC) en corriente alterna**, en sistemas de **2×25 kV o 1×25 kV**.

El CT aéreo toma la energía directamente del **feeder de −25 kV** o de la **catenaria**
(25 kV / 27,5 kV) y la transforma a **220 V** (secundario a 240 V nominales) para
alimentar servicios que no son de tracción: calefacción de agujas, alumbrado de
túneles, casetas de comunicaciones móviles (BTS/BTO), casetas técnicas de
señalización (PCA, PICV) y edificios técnicos con PLO de telecomando.

| Característica | Valor |
|----------------|-------|
| Sistema de alimentación | CA 1×25 kV o 2×25 kV (RFIG) |
| Tensión del primario | **27,5 kV / 50 Hz** (tomas −240, 0, +240 V en calefacción de agujas) |
| Tensión del secundario | **240 V** (servicio a 220 V) |
| Conexión del primario | **Monofásica en todo caso** |
| Refrigeración | **ONAN** (aceite, circulación natural) |
| Potencias habituales | 10 kVA (BTS) hasta **250 kVA máx.** (edificios técnicos) |
| Poste dedicado | Exclusivo del CT, metálico, 8,55 m (≤ edificios técnicos 9,45–12,45 m) |
| Altura partes AT no protegidas | Mínimo **5,0 m** sobre la base del poste |
| Altura mínima de la cuba | **3,0 m** sobre la base del poste |
| Protecciones | Seccionador unipolar 25 kV / 2500 A, fusible 36 kV, pararrayos ZnO 36 kV |
| Puesta a tierra | Pletina colectora + conexión al cable de tierra de la LAC (LA 110 / L110) |

> **Regla de proyecto:** para potencias superiores a **250 kVA** la instalación del
> transformador de servicios auxiliares se realizará **obligatoriamente en caseta**,
> con foso de recogida de aceite (nota a la Tabla 1 de la NAE 400).

---

## 3. QUÉ ES UN CT AÉREO Y PARA QUÉ SIRVE EN EL FERROCARRIL

Un **centro de transformación aéreo** es un conjunto formado por el transformador de
tensión y su aparamenta de protección y seccionamiento, montado **sobre un poste o
estructura portante de la LAC**. En él se desciende la tensión de la catenaria
(27,5 kV en primario) a baja tensión (240 V en secundario) para dar servicio a
consumidores no tractores de Adif.

La energía puede tomarse de dos orígenes (apartado 7.1):

- Del **feeder de −25 kV** (sistema 2×25 kV, autotransformador)
- De la **catenaria** de +25 kV (sistemas 1×25 kV y 2×25 kV)

El CT aéreo alimenta las siguientes **instalaciones asociadas** (apartados 1 y 3):

| Instalación asociada | Qué es | Notas |
|----------------------|--------|-------|
| **Calefacción de agujas** | Resistencia de caldeo de los desvíos para evitar hielo | Potencias 80/100/120 kVA |
| **Alumbrado de túneles** | Iluminación de recintos subterráneos | Alimentada desde CT sobre poste |
| **BTS** | Casetas de comunicaciones móviles de Adif (Telecommunications Services): estaciones base y repetidores de telefonía móvil | 10 kVA |
| **BTO** | Casetas de operador de telefonía móvil | 50 kVA |
| **Casetas técnicas de señalización** | **PCA**: puestos de acantonamiento automático · **PICV**: puestos intermedios de circuitos de vía | 200 kVA |
| **Edificios técnicos** | Alojan los **PLO** para telemandar y monitorizar el accionamiento del seccionador del transformador | Máx. 250 kVA; alimentación principal desde catenaria |

En todos los casos la conexión del **primario es monofásica**. El transformador
trabaja conectado a la **red de retorno de tracción**: el neutro del transformador,
tanto en el lado de alta como en el de baja, se conecta al circuito de retorno
(carril o cable de retorno) (apartado 7.2).

> El CT aéreo es una solución de bajo coste de obra y montaje frente a una caseta de
> transformación, adecuada para potencias moderadas y entornos de vía donde la
> ocupación del suelo debe minimizarse. Por encima de 250 kVA o cuando se requiere
> contención de aceite, la NAE 400 remite al montaje en caseta con foso.

---

## 4. ELEMENTOS DEL CT AÉREO

### 4.1. Elementos de la acometida (apartado 5)

La acometida de alta tensión a instalaciones asociadas se compone de:

- **Aparamenta de alta tensión** para la alimentación y conexión desde catenaria o
  feeder: **fusible, pararrayos de óxidos metálicos, seccionador con accionamiento
  manual o motorizado, y transformador**
- **Poste independiente de la catenaria**, soportes auxiliares y sus cimentaciones
- **Envolvente del accionamiento** y **protección de los circuitos de baja tensión**,
  colocados habitualmente en la parte inferior del poste, a **1 250 mm sobre el suelo**

Los **accionamientos motorizados** de los seccionadores deben estar preparados para
recibir y emitir los siguientes mandos y señales:

- Mando de **conexión / desconexión**
- Señal de **posición** del seccionador (conectado / desconectado)
- **Mando local** y preparación para el **sistema de mando a distancia**

### 4.2. Transformadores (apartado 4) — Tabla 1 de la NAE 400

| Acometida | Grupo conexión | Aislam./refrig. | Potencia (**) | Tensión primario (***) | Tensión secundario | Dimensiones (mm) (****) | Peso (kg) (****) |
|-----------|----------------|-----------------|---------------|-------------------------|--------------------|--------------------------|------------------|
| Calefacción de agujas | Monofásico | aceite · ONAN | **80/100/120 kVA** | 27,5 kV / 50 Hz · tomas −240, 0, +240 V | **240 V** | 850×800×1500 | 610–800 |
| BTS y detectores de CC | Monofásico | aceite · ONAN | **10 kVA** | 27,5 kV / 50 Hz | 240 V | 850×800×1500 | 500 |
| BTO | Monofásico | aceite · ONAN | **50 kVA** | 27,5 kV / 50 Hz | 240 V | 725×670×1360 | 420 |
| Casetas técnicas de señalización (*) | Monofásico | aceite · ONAN | **200 kVA** | 27,5 kV / 50 Hz | 240 V | 900×850×1600 | — |
| Edificios técnicos (*) | Monofásico | aceite · ONAN | **máx. 250 kVA** | 27,5 kV / 50 Hz | 240 V | 1210×800×1670 | 985 |

Notas de la Tabla 1:

- (*) Para potencias superiores a **250 kVA**, el transformador de servicios
  auxiliares se instala **obligatoriamente en caseta**, con **foso de recogida de aceite**
- (**) Potencias más habituales; la potencia será la requerida para cada caso concreto
- (***) Tensión nominal del sistema **25 kV**; tensión en el primario del transformador **27,5 kV**
- (****) Valores orientativos

### 4.3. Elementos complementarios (apartado 6)

| Elemento | Características |
|----------|-----------------|
| **Seccionador** | Unipolar, tensión nominal **25 kV c.a.**, corriente asignada **In = 2500 A**. Accionamiento manual o motorizado según proyecto. **Edificios técnicos: siempre motorizado**; en el resto, ambos tipos válidos |
| **Accionamiento (motorizado)** | Motor de **220 V c.a. / 50 Hz**, **par resistente nominal mínimo de 35 daNm** |
| **Pararrayos** | Descargador de **óxido metálico**, carcasa de **silicona**, tensión nominal **Uc = 36 kV** |
| **Fusible** | De instalación aérea, tensión asignada **Un = 36 kV**. La intensidad nominal se fija en el apartado 9.3. Debe incluir **portafusible** |

---

## 5. PROCESO DE MONTAJE PASO A PASO

### 5.1. Postes dedicados (apartado 8.1)

Los CT se ubican en un **poste dedicado exclusivamente a este servicio**, sobre
**silletas de fijación**, a una altura mínima suficiente para que las partes de alta
tensión no protegidas queden **por encima de 5,0 m** sobre la base del poste.

| Tipo de poste | Acometida | Potencia / uso |
|---------------|-----------|----------------|
| **X-3AV** | BTS, BTO, CT, calefacción de agujas, alumbrado de túneles | **≤ 100 kVA** |
| **X-5AV** | Acometidas generales | **≥ 100 kVA** |
| **XL-5AV** | Edificios técnicos | Necesidad de cruce de alimentación |
| **XLL-7AV** | Edificios técnicos | Cuando se requiere mayor altura |

- Postes de nuevo montaje: **8,55 m de altura**, salvo **edificios técnicos**, en los
  que se emplean postes **desde 9,45 m hasta 12,45 m** para realizar correctamente el
  cruce de la alimentación sobre las catenarias
- Preferiblemente **X-3AV** para calefacción de agujas, casetas de operación de
  telefonía y comunicaciones móviles (en algunos casos de calefacción de agujas se
  usan **X-5AV**)
- Los postes son **metálicos** y las dimensiones de los perfiles varían según los
  esfuerzos a soportar

### 5.2. Secuencia de montaje

1. **Cimentación y replanteo:** la instalación del poste debe permitir el
   mantenimiento del transformador desde un **vehículo de vía**; evitar su instalación
   en la misma perpendicular que el poste de catenaria respecto al eje de la vía,
   respetar el **gálibo de implantación de obstáculos** y no interferir con otras
   instalaciones (canalizaciones, arquetas, etc.)
2. **Izado y fijación del poste** sobre silletas, y aplomado según proyecto
3. **Izado de aparatos y conexionado eléctrico:** con la **grúa y cesta del vehículo**
   correspondiente, según las condiciones de ejecución; se utiliza una **eslinga
   textil** que no deteriore la pintura
4. **Montaje del transformador:** en la **cara del poste opuesta a la vía**; la parte
   inferior de la **cuba** queda a una altura **no inferior a 3 m** sobre la base del
   poste (si no se cumple, **cierre de protección**)
5. **Montaje del seccionador en cabeza de poste**, en la posición más favorable para
   su conexionado
6. **Ubicación de la envolvente del accionamiento y de la caja de baja tensión**, en
   la parte inferior del poste a **1 250 mm** sobre el suelo; el accionamiento del
   seccionador queda en **un lateral** y la caja de BT en **el otro lateral**
7. **Señalización:** carteles indicadores de peligro y señales de advertencia de
   riesgo eléctrico en los apoyos y en las cajas de baja tensión; medidas para evitar
   el **escalamiento**
8. **Conexionado de alta y baja tensión** y **puesta a tierra** (apartados 5.3 y 6)
9. **Verificación** de protecciones, enclavamientos y telecomando antes de la puesta
   en servicio

### 5.3. Conexionado y cableado (apartado 7.2)

- El **neutro del transformador**, tanto en el lado de baja como en el de alta, se
  conecta al **circuito de retorno de tracción** (carril y/o cable de retorno)
- **Calefacción de agujas, BTS y BTO:** conexiones desde el secundario del
  transformador bajo **un tubo** (generalmente **PVC o acero galvanizado**) por el
  interior del poste hasta el **armario de control de baja tensión**
- **Edificios técnicos:** conexiones desde el secundario bajo **2 tubos de acero
  galvanizado** por el interior del poste hasta el armario de control de BT. Además,
  **2 conjuntos de transmisión** para los seccionadores unipolares, ya que la acometida
  dispone de **dos seccionadores enclavados** que no pueden cerrarse a la vez para
  ponerse en paralelo

> **Orden de protección en el primario:** catenaria/feeder → seccionador unipolar →
> base portafusibles → pararrayos → borne primario del transformador. La parte móvil
> del seccionador se conecta al cable de −25 kV (2×25 kV) o de 25 kV (1×25 kV), y la
> parte fija, mediante **conexión flexible**, a la base portafusibles.

---

## 6. SEGURIDAD, DISTANCIAS Y PUESTA A TIERRA

### 6.1. Distancias y condiciones de seguridad (apartado 8.1.2)

| Magnitud | Valor mínimo |
|----------|--------------|
| Partes bajo tensión **no protegidas** contra contactos accidentales | **5,0 m** sobre la base del poste |
| Parte inferior de la **cuba del transformador** | **3,0 m** sobre la base del poste |
| Protecciones de BT / envolvente del accionamiento | A **1 250 mm** sobre el suelo (parte inferior del poste) |

Reglas adicionales:

- Si las alturas anteriores no se cumplen, se establece un **cierre de protección**
- La **base portafusibles nunca se colocará en el lado de la vía**
- El transformador va montado en la **cara del poste opuesta a la vía**
- Carteles de peligro, señales de advertencia de riesgo eléctrico y antiescalamiento
  en apoyos y cajas de BT
- El montaje debe respetar el **gálibo de implantación de obstáculos** y permitir el
  mantenimiento desde vehículo de vía

### 6.2. Protecciones asociadas (apartado 9)

**Seccionador (9.1):** se coloca en **cabeza de poste** en la posición más favorable.
La parte móvil se conecta al cable de **−25 kV** (2×25 kV) o de **25 kV** (1×25 kV) y
la parte fija, mediante conexión flexible, a la base portafusibles.

**Pararrayos (9.2):** sobre el transformador, en el herraje destinado a este fin. Se
conecta por un lado al **feeder o catenaria, lo más cerca posible del borne primario**
del transformador, y por el otro al **cable de tierra y a la toma de tierra**. Cada
pararrayos irá conectado a tierra con una **resistencia a la difusión menor de 10 Ω**.
Tipo óxido metálico, tensión nominal 36 kV.

**Fusible (9.3):** además de la tensión de red, el transformador limita principalmente
sus características. El fusible debe ser capaz de:

- **Resistir sin fusión intempestiva** la intensidad de cresta del arranque que
  acompaña a la conexión del transformador
- **Cortar las corrientes de defecto** a las bornas del secundario del transformador
- **Soportar** la intensidad en servicio continuo y las eventuales sobrecargas

Será el fabricante del transformador o el proyectista quien recomiende el fusible a
instalar. Debe incluir **cartucho portafusible**.

**Características asignadas del fusible (9.3.1):**

- Tensión asignada: **36 kV**, según **UNE-EN 60282** (Fusibles de alta tensión)
- Corriente asignada de la base fusible, según Tabla 2 (calibres seleccionados para
  instalaciones al aire libre con sobrecargas del transformador del 30 %):

| Tensión de servicio (kV) | Tensión asignada (kV) | 50 kVA | 75 kVA | 100 kVA | 125 kVA | 160 kVA | 200 kVA | 250 kVA |
|--------------------------|-----------------------|--------|--------|---------|---------|---------|---------|---------|
| 25 | 36 | 4 | 6,3 | 10 | 10 | 16 | 20 | 20 |

Aunque los calibres en **negrita** son los más apropiados, los demás valores
(6,3 / 10 / 16 / 20 / 25 A según el caso) también pueden proteger de forma adecuada
(nota de la Tabla 2).

### 6.3. Puesta a tierra (apartados 9.4 y 9.5)

- **Cable de tierra o retorno (9.4):** todos los postes van conectados al **cable de
  tierra de la LAC**, conductor de **aluminio-acero LA 110 (94ALL1/22ST1A)** o de
  **aluminio tipo L110 (117-AL1)**
- Si el poste del transformador está **alineado con los postes de catenaria**, la
  conexión al cable de tierra se realiza con **grapa de suspensión G36U**, a la altura
  correspondiente donde se encuentre el cable de tierra
- **Pletina colectora de tierras (9.5):** en el poste se instala una pletina colectora
  a la que se conectan **todas las masas metálicas** (bastidores de armarios, cuba del
  transformador, etc.) mediante **conductor de cobre aislado de 50 mm²** (o equivalente
  en aluminio), **0,6/1 kV**, según lo establecido en la **ITC-RAT 13**
- Se pondrá a tierra un **borne del bobinado primario y el secundario** del
  transformador de alimentación al sistema

---

## 7. RELACIÓN CON OTRAS NORMAS

| Norma | Relación con la NAE 400 |
|-------|-------------------------|
| **NAE 111** | «Montaje del cable de tierra/retorno de la LAC». La NAE 400 remite al cable de tierra de la LAC (LA 110 / L110) y a la grapa G36U; la NAE 111 fija el procedimiento de montaje de ese cable y de sus conexiones a los soportes y picas |
| **Serie ET 03.364** | Especificaciones técnicas de material de electrificación (conjuntos de poleas, material de LAC, etc.). Los postes tipo X-3AV / X-5AV / XL-5AV / XLL-7AV y la aparamenta de acometida se suministran y verifican conforme a las ET de la serie |
| **RD 337/2014 (ITC-RAT 01 a 23)** | Reglamento sobre condiciones técnicas y garantías de seguridad en instalaciones eléctricas de alta tensión. La NAE 400 cita expresamente la **ITC-RAT 13** para el conexionado de masas a la pletina colectora |
| **ADIF-PE-301-001-006-SC-521** | Cortes de tensión en líneas aéreas de contacto (25 kV c.a., 3 kV c.c., 1,5 kV c.c.), Rev. 1, mayo 2020. Aplicable a los trabajos de conexionado del CT sobre LAC en tensión |
| **UNE-EN 50125-2** | Condiciones ambientales del equipo: instalaciones eléctricas fijas ferroviarias |
| **UNE-EN 60076-1 / UNE-EN 50708-1-1** | Transformadores de potencia: generalidades y requisitos europeos adicionales |
| **UNE-EN IEC 60282-1 / UNE 21122** | Fusibles de alta tensión limitadores de corriente y guía de elección de fusibles para circuitos con transformadores |
| **NAE 107 y normas de diseño (NAE 300/301/302)** | Parámetros y tipologías de catenaria: el CT se deriva de la catenaria o del feeder con las distancias de aislamiento del sistema (Lecciones 1 y 2) |

> La NAE 400 **no deroga ningún documento normativo** (apartado 10) y entra en vigor en
> la fecha de su aprobación (apartado 11).

---

## 8. AUTOEVALUACIÓN

1. ¿Cuál es el objeto de la NAE 400 y en qué sistemas de electrificación se aplica?
2. ¿De qué dos orígenes puede alimentarse un CT aéreo en un sistema 2×25 kV?
3. ¿Qué instalaciones asociadas alimentan los CT aéreos? Cita al menos cinco.
4. ¿Qué significan las siglas BTS, BTO, PCA y PICV?
5. ¿Cuál es la conexión del primario del transformador y su tensión nominal? ¿Y la del secundario?
6. Indica las potencias habituales del transformador para calefacción de agujas, BTS, BTO, casetas técnicas y edificios técnicos.
7. ¿Qué ocurre si una instalación de servicios auxiliares necesita más de 250 kVA?
8. ¿Qué tensión y corriente asignadas tiene el seccionador unipolar de la acometida? ¿Cuándo debe ser motorizado?
9. ¿Qué tensión nominal tiene el pararrayos y de qué tipo es? ¿Cuál es la resistencia a la difusión máxima de su toma de tierra?
10. ¿Qué tensión asignada tienen los fusibles de la acometida y según qué norma UNE-EN?
11. ¿Qué tres capacidades debe tener el fusible frente al transformador?
12. Calcula el calibre de fusible más apropiado para un transformador de 100 kVA en una red de 25 kV (Tabla 2).
13. ¿Qué tipos de poste se emplean según la acometida y la potencia? Relaciona X-3AV, X-5AV, XL-5AV y XLL-7AV.
14. ¿Qué alturas de poste de nuevo montaje se emplean en general y en edificios técnicos? ¿Por qué esa diferencia?
15. ¿A qué alturas mínimas sobre la base del poste deben quedar las partes de AT no protegidas y la parte inferior de la cuba?
16. ¿En qué lado del poste se monta el transformador y dónde nunca se coloca la base portafusibles?
17. ¿Cómo se conectan los neutros del transformador en alta y en baja?
18. ¿Qué conductor de cobre se emplea para conectar las masas a la pletina colectora de tierras y según qué instrucción técnica?
19. ¿Qué función cumplen los dos seccionadores enclavados en la acometida de edificios técnicos?
20. ¿Qué normativa regula el montaje del cable de tierra/retorno y qué conductores se emplean (LA 110 / L110)?

---

## 9. REFERENCIAS

- **NAE 400** (1ª ed., jun 2024): apartados 1–12, Tablas 1–2, Anejo 1 (esquemas de
  montaje y conexiones)
- **NAE 111**: Montaje del cable de tierra/retorno de la LAC (Lección del módulo)
- **Serie ET 03.364**: especificaciones técnicas de material de electrificación (postes, aparamenta)
- **Real Decreto 337/2014, de 9 de mayo**: Reglamento de condiciones técnicas y
  garantías de seguridad en instalaciones eléctricas de alta tensión y sus ITC-RAT 01 a 23 (ITC-RAT 13: puesta a tierra)
- **ADIF-PE-301-001-006-SC-521** (Rev. 1, may 2020): Cortes de tensión en líneas aéreas de contacto
- **UNE-EN 50125-2**: condiciones ambientales para instalaciones eléctricas fijas ferroviarias
- **UNE 21122**: guía para la elección de fusibles de AT en circuitos con transformadores
- **UNE-EN IEC 60282-1**: fusibles de alta tensión, parte 1: limitadores de corriente
- **UNE-EN 60076-1**: transformadores de potencia, parte 1: generalidades
- **UNE-EN 50708-1-1**: transformadores de potencia, requisitos europeos adicionales
- **NAE 107 / NAE 300 / NAE 301 / NAE 302**: parámetros y diseño de la LAC (Lecciones 1 y 2)

---

*Lección 9: Centros de transformación aéreos para instalaciones asociadas — NAE 400.*
