# MÓDULO 5 · LECCIÓN 7
# LÍNEA AÉREA DE CONTACTO EN VÍAS DE TRES CARRILES (NAE 117)

## Documento base

> **Documento base:** NAE 117, «Línea aérea de contacto para vías con tres carriles
> electrificadas en corriente continua», 3ª edición, diciembre 2024, 65 págs.
> Grupo de trabajo GT-300 · Propuesta: 5-dic-2024 · Aprobada por el Comité de
> Normativa (12-dic-2024). Deroga la NAE 117 2ª edición (feb 2022).
>
> La 3ª edición amplía los parámetros de diseño en situaciones puntuales (4.2),
> actualiza condiciones ambientales y normativa de referencia (5.1.1), corrige el
> máximo cambio de gradiente a 50 km/h (5.3), exige el replanteo simétrico de los
> seccionamientos (5.5), actualiza las tablas de vanos máximos y de seccionamientos
> de compensación con condiciones ambientales a 5 °C (6.3) e incorpora las
> referencias a la IFE (Orden TMA/135/2023) en distancias de aislamiento y gálibos.

---

## 1. RESULTADO DE APRENDIZAJE

Al terminar esta lección serás capaz de:

1. Explicar qué es una **vía de tres carriles** (anchos 1668 y 1435 mm) y qué
   papel juega el **cambiador de hilo** en la circulación en ancho estándar
2. Identificar las **tipologías de catenaria** que la norma admite sobre tres
   carriles (CA-160 Tipo A/B, CA-160H, CA-200H y CA-220 en 3 kV c.c.) y con qué
   pantógrafos es compatible cada una
3. Aplicar los **descentramientos** (±(250/134) mm, banda común de frotamiento
   de 384 mm) y los **vanos máximos** en función del radio y del pantógrafo
4. Conocer las reglas de **retorno y puesta a tierra** en c.c. y las **distancias
   de aislamiento** (150/50 mm y 270/150 mm) que fija la norma
5. Dimensionar **seccionamientos de compensación (200 mm)** y de **lámina de
   aire (300 mm)** sobre tres carriles
6. Replantear **agujas aéreas** (cruzadas y tangenciales) y la zona de
   **cambiador de hilo** con los puntos de aguja validados (P.30, P.30+140,
   P.50 y P.90)

---

## 2. RESUMEN EJECUTIVO

La NAE 117 es la norma **específica de Adif** para la Línea Aérea de Contacto
sobre **vías de tres carriles electrificadas en corriente continua a 3 kV**. No
define una tecnología nueva de catenaria: **solo fija los parámetros de diseño que
se ven afectados por la existencia de un tercer carril**, remitiendo a las normas
de diseño funcional de cada tipología (NAE 300/301/302) para todo lo demás.

Las ideas clave de la norma:

| Aspecto | Criterio NAE 117 |
|---------|------------------|
| **Sistema** | 3 kV c.c. (la 2ª ed. eliminó el 1,5 kV); anchos 1668 mm (ibérico) y 1435 mm (UIC) |
| **Tipologías** | CA-160 Tipo A/B, CA-160H, CA-200H, CA-220 (todas 3 kV) |
| **Pantógrafo** | Diseño para al menos 1950 mm (cuernos conductores); admisible 1600 mm |
| **Descentramiento** | ±(250/134) mm → banda común de frotamiento **384 mm** |
| **Altura nominal / máx.** | **5300 mm / 6000 mm** (mínima variable según IFE) |
| **Seccionamientos** | Compensación: calle **200 mm** · Lámina de aire: calle **300 mm** |
| **Aislamiento** | CA-160/CA-220: **150/50 mm** · CA-160H/CA-200H: **270/150 mm** |
| **Viento** | Estructural 120 km/h (33,3 m/s); funcional según mapa del Anejo 1 |

> **Regla general:** si hay contradicción entre la NAE 117 y la norma de diseño de
> la tecnología de catenaria, **prevalece la norma que define la tecnología**.

---

## 3. LA VÍA DE TRES CARRILES Y SU ELECTRIFICACIÓN (contexto)

### 3.1. Qué es una vía de tres carriles

Una vía de **tres carriles** permite la circulación simultánea de trenes de los dos
anchos de vía que conviven en la red de Adif:

- **Ancho ibérico (1668 mm):** la pareja de carriles separada 1668 mm.
- **Ancho estándar europeo (1435 mm, referido como «UIC» en la norma):** formado por
  uno de los carriles anteriores y un **tercer carril** adicional, separado 1435 mm.

De los tres carriles, uno es el **carril común** (participa en ambos anchos) y en
el lado opuesto quedan los **dos carriles del ancho ibérico**, que la norma
denomina **«carril doble»**. Por eso, al dimensionar la LAC, la posición relativa
del **carril común** (lado del poste o lado contrario) condiciona los signos de los
descentramientos.

> **Definición de la norma (gálibo de implantación de obstáculos):** «Para vías de
> tres carriles el gálibo será la envolvente definida por la combinación del gálibo
> considerado en cada ancho, teniendo en cuenta la posición del tercer carril».

### 3.2. El cambiador de hilo

Cuando dos trenes en ancho estándar circulan en sentidos opuestos por la misma
vía de tres carriles, el **carril común** debe poder pasar de un lado a otro de la
vía. Ese aparato de vía es el **cambiador de hilo**:

> **Definición de la norma:** «Es el aparato de vía cuyo funcionamiento y posición
> permite dar continuidad a la circulación de los trenes por ancho estándar europeo
> en vías de tres carriles, haciendo posible que el tercer hilo pase de situarse de
> un lado a otro en función del sentido de la marcha».

### 3.3. Cómo se electrifica en corriente continua

- Tensión de alimentación: **3 kV c.c.**. La NAE 117 **no es de aplicación a
  catenaria rígida ni a catenaria tranviaria**, y no contempla ya líneas de 1,5 kV.
- El pantógrafo de diseño es el de **1950 mm**, con la geometría de arco de las
  figuras **A.7 y B.2 de la UNE-EN 50367** y **cuernos conductores**. En líneas
  renovadas o acondicionadas se puede admitir, excepcionalmente y con justificación
  técnico-económica, el diseño con **cuernos aislantes**.
- Si además se quiere explotar con un pantógrafo de **1600 mm**, este debe cumplir
  la geometría de arco de la figura **A.6 de la UNE-EN 50367**.
- La norma **no exime del cumplimiento de la ETI del subsistema de energía**
  (Reglamento UE 1301/2014).

### 3.4. Aparatos de vía contemplados

La norma considera todos los desvíos instalados en tres carriles: a derecha o
izquierda, con salidas de la vía directa **en dos anchos** y de la desviada en dos
anchos, solo en ancho ibérico o solo en ancho estándar, y sus combinaciones
cruzadas (directa en un ancho y desviada en el otro).

---

## 4. CONFIGURACIÓN DE LA CATENARIA EN TRES CARRILES

### 4.1. Tipologías de catenaria aplicables (4.2)

| Catenaria | Compatible con pantógrafo 1950 mm | Compatible con pantógrafos 1950 y 1600 mm |
|-----------|:---:|:---:|
| **CA-160 Tipo A 3 kV** | Sí | — |
| **CA-160 Tipo B 3 kV** | Sí | Sí |
| **CA-160H 3 kV** | Sí | Sí |
| **CA-200H 3 kV** | Sí | Sí |
| **CA-220 3 kV** | Sí | Sí |

Si una tecnología no está en esta relación, es necesario **un estudio que
demuestre el cumplimiento de todos los parámetros** de la norma. Las normas de
diseño de referencia son la NAE 300 (CA-160 Tipo A y B), la NAE 302 (CA-160H y
CA-200H) y la NAE 301 (CA-220).

### 4.2. Conductores y tenses admisibles (6.1, tabla 8)

| Catenaria | Sustentador (sección · tense) | Hilo de contacto (sección · tense) |
|-----------|-------------------------------|-----------------------------------|
| **CA-160 Tipo A** | 150 mm² · 1425 kgf (1397 daN) | 2 × 107 mm² · 1050 kgf (1030 daN) |
| **CA-160 Tipo B** | 150 mm² · 1425 kgf (1397 daN) | 2 × 120 mm² · 1200 kgf (1177 daN) |
| **CA-160H** | 150 mm² · 1425 kgf (1397 daN) | 2 × 120 mm² · 1200 kgf (1177 daN) |
| **CA-200H** | 150 mm² · 1650 kgf (1618 daN) | 2 × 120 mm² · 1500 kgf (1471 daN) |
| **CA-220** | 185 mm² · 2475 kgf (2427 daN) | 2 × 150 mm² · 1875 kgf (1839 daN) |

### 4.3. Descentramiento y banda común de frotamiento (6.2, tabla 9)

El hilo debe mantenerse captable por el pantógrafo **cualquiera que sea el ancho
por el que circule el tren**. Para ello la norma fija un descentramiento único
referido preferentemente al **eje ibérico**:

| Trazado | Descentramientos máximos (mm) |
|---------|-------------------------------|
| **Recta** | 250 / 134 |
| **Curva** | 250 / 250 |

- En términos absolutos el descentramiento es **±(250/134) mm**, de forma que se
  genera una **banda común de frotamiento de 384 mm**.
- Los valores están referidos al eje ibérico con **poste en el lado del carril
  doble**; si el poste se ubica **junto al carril común**, se aplican los mismos
  valores absolutos **cambiados de signo**.
- En curva los valores son máximos y deben ajustarse al radio según las tablas de
  vano del apartado 6.3.
- Debe verificarse que el esfuerzo radial alcanza el rendimiento esperado en el
  brazo de atirantado; en caso contrario se modifica el descentramiento máximo.
- En algunas electrificaciones ya realizadas coexiste el descentramiento
  **±(200/80) mm**, para el que la norma también facilita vanos máximos.

### 4.4. Vano máximo (6.3)

El vano máximo depende de la **tipología**, del **radio de curva**, del
**descentramiento en los dos apoyos** (dᵢ, dᵢ₊₁) y del **pantógrafo** considerado.

> **Condiciones de cálculo de las tablas:** viento de referencia **29 m/s**, altitud
> **0 m**, temperatura **5 °C**, categoría de terreno **2**. Para un proyecto
> concreto el valor máximo de los vanos se calcula con las condiciones ambientales
> más desfavorables de la línea (los vanos pueden tener que reducirse).

**Vano máximo compatible con pantógrafos de 1950 y 1600 mm (resumen):**

| Catenaria | Descentr. | Recta / radio alto | Vano (m) según radio (valores de referencia) |
|-----------|-----------|--------------------|---------------------------------------------|
| CA-160 Tipo B y CA-160H | ±(250/135) | 54 m (R ≥ 15000) | 54/50/45/40/35/30/25 según radio ≥ 15000 → ≥ 200 |
| CA-160 Tipo B y CA-160H | ±(200/80) | 55 m (R ≥ 14000) | 55/50/45/40/35/30/25 según radio ≥ 14000 → ≥ 225 |
| CA-200H | ±(250/135) | 60 m (R ≥ 16000) | 60/55/50/45/40/35/30/25 según radio ≥ 16000 → ≥ 230 |
| CA-200H | ±(200/80) | 60 m (R ≥ 10000) | 60/55/50/45/40/35/30/25 según radio ≥ 10000 → ≥ 230 |
| CA-220 | ±(250/135) | 60 m (R ≥ 10000) | 60/55/50/45/40/35/30/25 según radio ≥ 10000 → ≥ 270 |
| CA-220 | ±(200/80) | 60 m (R ≥ 7000) | 60/55/50/45/40/35/30/25 según radio ≥ 7000 → ≥ 270 |

**Vano máximo compatible solo con pantógrafo de 1950 mm (resumen):**

| Catenaria | Descentr. | Recta / radio alto | Vano (m) según radio |
|-----------|-----------|--------------------|----------------------|
| CA-160 Tipo A | ±(250/135) | 60 m (R ≥ 6000) | 60/55/50/45/40/35/30 según radio ≥ 6000 → ≥ 200 |
| CA-160 Tipo B y CA-160H | ±(250/135) | 60 m (R ≥ 4500) | 60/55/50/45/40/35/30 según radio ≥ 4500 → ≥ 210 |
| CA-200H | ±(250/135) | 60 m (R ≥ 2500) | 60/55/50/45/40/35/30 según radio ≥ 2500 → ≥ 250 |
| CA-220 | ±(250/135) | 60 m (R ≥ 2300) | 60/55/50/45/40/35/30 según radio ≥ 2300 → ≥ 325 |

> Los tramos de radio alto admiten descentramientos tipo recta (250/−135); según
> disminuye el radio se pasa a descentramientos 250/0 y 250/250. Las tablas 10 a
> 19 de la norma dan el valor exacto de dᵢ y dᵢ₊₁ para cada intervalo de radio.
>
> **Excepciones admitidas (4.2):** vano máximo mayor en casos singulares si se
> justifica el cumplimiento de la desviación lateral por viento; radio mínimo si el
> conjunto de atirantado soporta el tense radial hasta **400 daN**; altura de
> sistema inferior a 1400 mm siempre que la péndola equipotencial mínima sea de
> **250 mm** (excepcionalmente péndolas de varilla de longitud mínima de montaje).

### 4.5. Agujas aéreas (7)

La geometría de las agujas aéreas debe cumplir la **UNE-EN 50119 (5.11)** y la
**IFE (4.1.2.2.17)**. Requisitos generales:

- El hilo de contacto se mantiene **dentro de la zona de trabajo** definida en el
  anexo A de la UNE-EN 50367 y **no golpea ni se sitúa por debajo del trocador**
  del pantógrafo.
- **Agujas cruzadas:** en vía directa el hilo de la directa se mantiene dentro del
  rango de desviación máxima; el **primer contacto** del hilo de la desviada (punta
  y talón) debe producirse en el **mismo semipantógrafo** que el hilo de la directa
  (excepcionalmente en el otro, a un máximo de **5 cm del eje** del pantógrafo) y
  dentro de la zona de trabajo.
- **Agujas tangenciales:** en ningún caso el hilo de la vía desviada debe contactar
  con el pantógrafo al pasar por vía directa.
- Para velocidades superiores a **160 km/h** en vía general pueden usarse
  **péndolas cruzadas** para garantizar la elevación solidaria de los hilos.
- En la posición relativa pantógrafo–hilo se tiene en cuenta la dilatación de los
  conductores, la desviación lateral por viento, los esfuerzos dinámicos y la
  inclinación del pantógrafo.

**Tipologías validadas (tablas 40 y 41):**

| Pantógrafos | Tipología de aguja | Punto de aguja | Desvíos |
|-------------|--------------------|----------------|---------|
| 1950 + 1600 mm | **Cruzada** | **P. 30** | 190 m (0,11) y 250 m (0,11) |
| 1950 + 1600 mm | **Cruzada** | **P. 30 + 140** (*) | 500 m (0,071) |
| 1950 mm | **Cruzada** | **P. 50** | 190 m (0,11) |
| 1950 mm | **Tangencial** | **P. 90** | 250 m (0,11) y 500 m (0,071) |

(*) El segundo punto de aguja corresponde a un **poste auxiliar o poste llamada**.
El Anejo 1 de la norma desarrolla esquemas en planta de estas configuraciones,
con descentramientos referidos al eje ibérico en vía directa y desviada.

> **Regla:** en líneas compatibles con pantógrafos de 1950 y 1600 mm se instalan
> **agujas cruzadas** con carácter general. Las **tangenciales** se reservan para
> desvíos operados únicamente con el pantógrafo de **1950 mm**.

### 4.6. Cambiadores de hilo: reglas de replanteo (6.4)

- Se replantean los postes para que el **centro geométrico del cambiador de hilo**
  quede lo más cerca posible del **centro del vano**.
- Siempre que sea posible, **no se replantea un seccionamiento sobre un cambiador
  de hilo**.
- Se adecúan los descentramientos a cada lado del cambiador según el apartado 6.2
  en función de la posición del carril común.

### 4.7. Variación de altura y transiciones (5.3, tabla 3)

La altura debe ser lo más constante posible. En túneles, pasos superiores o pasos
a nivel la transición se realiza con pendientes referidas al plano de la vía:

| Velocidad (km/h) | Máximo gradiente | Máximo cambio de gradiente |
|------------------|------------------|----------------------------|
| 50 | 1/40 (25 ‰) | 1/80 (12,5 ‰) |
| 60 | 1/50 (20 ‰) | 1/100 (10 ‰) |
| 100 | 1/167 (6 ‰) | 1/333 (3 ‰) |
| 120 | 1/250 (4 ‰) | 1/500 (2 ‰) |
| 160 | 1/500 (2 ‰) | 1/1000 (1 ‰) |
| 200 | 1/1000 (1 ‰) | 1/2000 (0,5 ‰) |
| 250 | 1/1000 (1 ‰) | 1/2000 (0,5 ‰) |

> Si hay varios pasos superiores próximos con gálibo reducido, se mantiene entre
> ellos la misma altura del hilo y las transiciones se hacen **solo antes del
> primero y después del último**. El paso de una altura de sistema a otra se
> realiza **intercalando las transiciones necesarias**, adecuando el vano para
> respetar las longitudes de péndola mínima.

---

## 5. RETORNO DE CORRIENTE Y PUESTA A TIERRA

### 5.1. Qué fija la NAE 117

La NAE 117 no desarrolla el circuito de retorno: **remite a las normas generales**.
Define únicamente las **distancias de aislamiento** de diseño y las condiciones de
retorno indirectas que afectan al tercer carril. Concretamente:

- Las distancias de aislamiento se calculan según la **UNE-EN 50119 (apdo. 5.1.3)**
  y la **IFE (apdo. 4.1.2.2.11)**.
- La seguridad eléctrica, la **puesta a tierra y el circuito de retorno** se rigen
  por la **UNE-EN 50122-1** («Seguridad eléctrica, puesta a tierra y circuito de
  retorno. Parte 1: Medidas de protección contra los choques eléctricos»).
- Los esquemas eléctricos unifilares de las instalaciones de c.c. —incluidos
  retorno y protecciones— se rigen por la **NAE 112** (véase el apartado 8).

### 5.2. Distancias de aislamiento (5.9, tabla 7)

| Tipo de catenaria | Estáticas (mm) | Dinámicas (mm) |
|-------------------|:--------------:|:--------------:|
| CA-160 y CA-220 | **150** | **50** |
| CA-160H y CA-200H | **270** | **150** |

> Valores «a modo informativo» para el diseño; los valores vinculantes son los de
> la UNE-EN 50119 (5.1.3) y la IFE (4.1.2.2.11), recogidos en cada norma de
> catenaria. Los valores mayores de las catenarias «H» responden a su carácter
> híbrido (preparadas también para 25 kV).

### 5.3. Consideraciones de explotación en tres carriles

Dado que la vía puede ser utilizada por trenes de ambos anchos sobre la misma
infraestructura, la comprobación de la **desviación lateral máxima del hilo de
contacto** debe hacerse **para cada par de carriles** (diseñado para utilizarse
como vía separada) que se vaya a evaluar (apdo. 5.10 de la NAE 117). La norma
remite, como mínimo, al apartado **4.2.9 de la ETI de Energía** y al
**4.1.2.2.1 de la IFE**.

En corriente continua el retorno se realiza por los **carriles de rodadura** (que
forman el circuito de retorno), de modo que el **tercer carril participa en el
retorno** según el ancho por el que circule el tren. Esto exige que los estudios de
**gálibo eléctrico** consideren la envolvente combinada de ambos anchos y la
posición del carril común:

- El estudio de gálibos se realiza con la metodología de la **UNE-EN 15273** y la
  **Instrucción Ferroviaria de Gálibos**, comprobando la compatibilidad de los
  pantógrafos habilitados sobre **ambos ejes de vía** (apdo. 5.11).
- Se cumple, como mínimo, el apartado **4.2.10 de la ETI de Energía** y el
  **4.1.2.2.2 de la IFE** (gálibo del pantógrafo).
- Las protecciones pasivas de la instalación (pararrayos/limitadores de tensión
  según UNE-EN 50526-1, cable de tierra, pozos de tierra y conexiones
  equipotenciales) forman parte del sistema de LAC y se reflejan en los esquemas
  de la NAE 112, aunque no aparecen en el esquema eléctrico por ser elementos
  pasivos.

> **Precisión:** la puesta a tierra de postes, macizos y estructuras se realiza
> conforme a la NAE 106 (cimentaciones) y a las normas de la tecnología de
> catenaria; en c.c., la medida poste–carril se hace con **cinta no conductora**
> para no perturbar el circuito de retorno (criterio general de la NAE 107).

---

## 6. SECCIONAMIENTO Y PROTECCIONES

### 6.1. Cantón de compensación mecánica (5.6, tabla 6)

- **Punto fijo en la mitad del cantón**, aunque los semicantones pueden ser
  asimétricos en trazados en curva con vanos heterogéneos.
- Por defecto el conjunto de punto fijo se realiza **solo en el sustentador**. Se
  montan **latiguillos de punto fijo** entre sustentador e hilo de contacto cuando:
  - La diferencia de longitud entre los semicantones supera el **20 %** → latiguillos
    **a ambos lados** del punto fijo.
  - La pendiente de la rasante supera **5 milésimas** → un **solo latiguillo en el
    lado más bajo** de la vía.
- Equipos de compensación: **poleas** con compensación independiente para
  sustentador e hilos en cielo abierto; **tensor-muelle** en zonas de gálibo
  reducido o andenes de estación.
- Tipos de anclaje según longitud: cantón completo → **compensación independiente
  a ambos lados**; semicantón → **independiente + 1 no compensado**.
- La longitud máxima del cantón es la definida para cada tipo de catenaria en su
  norma de diseño, validada según la tecnología de compensación y la geometría.

### 6.2. Diferencia de longitud entre vanos consecutivos (5.5, tabla 5)

| Zona | Diferencia máx. |
|------|-----------------|
| Trayecto | **10 m** |
| Agujas | **5 m** |
| Seccionamientos | **1 m** (*) |

(*) Todos los seccionamientos se replantean **simétricos**. En los de 4 vanos, los
vanos de elevación adyacentes al eje se replantean iguales con tolerancia ±1 m; en
los de 5 vanos los vanos de elevación también son iguales (±1 m) y el vano central
difiere de los de elevación como máximo **5 m**.

### 6.3. Seccionamientos de compensación (6.3.3, tabla 20)

- **Calle entre catenarias: 200 mm** nominales, tolerancia **−0 / +20 mm**, medida en
  horizontal y mantenida en **todos los vanos** del seccionamiento. Valores
  superiores a la nominal son admisibles justificando la desviación lateral por
  viento; el mínimo es 200 mm (4.2).
- Construcción preferible: **3 vanos (sin eje)** o **4 vanos (con eje)**, simétricos
  y con vanos homogéneos.
- Calculados para **elevación del semieje de 250 mm**; se evita el replanteo con
  vanos inferiores a 25 m (28 m en CA-220) porque obligaría a 5 o más vanos.

**Vano máximo en seccionamientos de compensación:**

| Catenaria | Pantógrafos 1950+1600 (m) | Pantógrafo 1950 (m) |
|-----------|:---:|:---:|
| CA-160 Tipo A | — | 60 |
| CA-160 Tipo B y CA-160H | **45** | 60 |
| CA-200H | **51** | 60 |
| CA-220 | **53** | 60 |

> Los descentramientos de los esquemas de seccionamiento (Cat1 y Cat2 en las
> tablas 22-29) están referidos al **eje ibérico** y varían según el radio y el
> vano; las condiciones de cálculo son 29 m/s, altitud 0 m y 5 °C.

### 6.4. Seccionamientos de lámina de aire (6.3.4, tabla 30)

- **Calle entre catenarias: 300 mm** nominales, tolerancia **−0 / +20 mm**. Este valor
  nominal es válido **tanto para 3 kV como para futuras electrificaciones de
  25 kV** en catenarias híbridas. La zona neutra de cambio de fases en 25 kV queda
  **fuera del alcance** de esta norma.
- Calculados para **elevación del semieje de 350 mm**; se evita el replanteo con
  vanos inferiores a 25 m (28 m en CA-220).

**Vano máximo en seccionamientos de lámina de aire:**

| Catenaria | Pantógrafos 1950+1600 (m) | Pantógrafo 1950 (m) |
|-----------|:---:|:---:|
| CA-160 Tipo A | — | 54 |
| CA-160 Tipo B y CA-160H | **42** | 58 |
| CA-200H | **45** | 60 |
| CA-220 | **47** | 60 |

### 6.5. Protecciones

- La NAE 117 remite a la **UNE-EN 50526-1** para los **pararrayos y limitadores de
  tensión** en c.c.
- El seccionamiento eléctrico de la instalación (seccionadores, paquete eléctrico,
  seccionamientos de cantón y lámina de aire, aisladores de sección) se refleja en
  los **esquemas eléctricos de la NAE 112**, que fija la nomenclatura de los
  elementos de corte y alimentación y la simbología para los cortes de tensión
  (ADIF-PE-301-001-006-SC-521).

---

## 7. PARÁMETROS Y DATOS DE DISEÑO (datos reales de la norma)

| Parámetro | Valor NAE 117 (3ª ed., dic 2024) |
|-----------|----------------------------------|
| Tensión de alimentación | **3 kV c.c.** (no aplica a 1,5 kV, ni a catenaria rígida o tranviaria) |
| Anchos de vía | **1668 mm (ibérico)** y **1435 mm (estándar europeo / UIC)** |
| Pantógrafo de diseño | **1950 mm** (UNE-EN 50367 figs. A.7 y B.2, cuernos conductores); excepcional 1600 mm (fig. A.6) |
| Temperatura ambiental mín. | **−15 °C** |
| Temperatura ambiental máx. | **+50 °C** (ajuste regional con datos AEMET 50 años y modelos de cambio climático) |
| Viento estructural | **120 km/h (33,3 m/s)** para postes, pórticos, etc. |
| Viento funcional | Metodología IFE 4.1.2.2.1.2, mapa del **Anejo 1**, corrección hasta retorno **10 años** |
| Altura mínima de diseño | **Variable** (según IFE 4.1.2.2.1.4 y UNE-EN 50119) |
| Altura nominal del hilo | **5300 mm** |
| Altura máxima de diseño | **6000 mm** (si no se alcanza en pasos a nivel → pórticos de protección) |
| Altura del sistema de catenaria | **1400 mm** nominal (trayectos y estaciones); variable en gálibo reducido y en seccionamientos |
| Diferencia de vanos (trayecto / agujas / seccionamientos) | **10 m / 5 m / 1 m** |
| Descentramiento | **±(250/134) mm** → banda común de frotamiento **384 mm**; en curva 250/250; (±(200/80) en electrificaciones existentes) |
| Distancia de aislamiento (CA-160 y CA-220) | Estática **150 mm** · Dinámica **50 mm** |
| Distancia de aislamiento (CA-160H y CA-200H) | Estática **270 mm** · Dinámica **150 mm** |
| Separación en seccionamiento de compensación | **200 mm** (tol. −0/+20 mm) |
| Separación en seccionamiento de lámina de aire | **300 mm** (tol. −0/+20 mm) |
| Vano máximo en trayecto (1950 mm) | Hasta **60 m** (según radio y tipología) |
| Vano máximo en compensación (1950+1600) | 45 / 51 / 53 m (CA-160B-H / CA-200H / CA-220) |
| Vano máximo en lámina de aire (1950+1600) | 42 / 45 / 47 m (CA-160B-H / CA-200H / CA-220) |
| Condiciones de cálculo de vanos | **29 m/s · altitud 0 m · 5 °C · categoría de terreno 2** |
| Elevación de semieje (compensación / lámina) | **250 mm / 350 mm** |
| Tense radial máximo del atirantado | Hasta **400 daN** (justificado) |
| Pendiente del hilo en transiciones | 50 km/h → 25 ‰ · 160 km/h → 2 ‰ · 200/250 km/h → 1 ‰ |
| Cambiador de hilo | Centro cerca del centro del vano; evitar seccionamiento sobre él |

---

## 8. COORDINACIÓN CON NAE 107/112 Y ET DE MATERIAL

### 8.1. Con la NAE 107 (parámetros de la LAC)

La NAE 107 define y mide los parámetros (altura, pendiente, vano, descentramiento,
gálibo de postes, cantón de compensación, distancias de aislamiento, elevación y
elasticidad). La NAE 117 **reutiliza esa definición** y solo particulariza los
valores afectados por el tercer carril (descentramiento ±(250/134), banda de
384 mm, distancias de aislamiento por tipología, etc.). En caso de contradicción
**prevalece la norma de la tecnología de catenaria** y, sobre el modo de medir,
la NAE 107.

### 8.2. Con la NAE 112 (esquemas eléctricos de LAC en c.c.)

La NAE 112 (3ª ed. + M1, ene 2023) fija el formato y contenido de los **esquemas
eléctricos unifilares** de la LAC en c.c. y la nomenclatura de los elementos de
corte y alimentación. En vías de tres carriles es la que da soporte documental al
seccionamiento descrito en el apartado 6: seccionadores de vía general (ZN, P, F,
S), puesta en paralelo, fíderes (de alimentación y de refuerzo), paquete
eléctrico, seccionamientos de cantón y lámina de aire, aisladores de sección y
protecciones pasivas (pararrayos, cable de tierra, pozos de tierra, conexiones
equipotenciales). En estaciones donde coexisten varias tensiones, la designación
de los seccionadores se distingue con un prefijo de tensión (1 para 1,5 kV y 3
para 3 kV).

### 8.3. Con las normas de diseño y las especificaciones de material (ET)

La NAE 117 **no define tecnología**: para cada tipología se aplica su norma de
diseño funcional y su cadena de especificaciones de material:

| Catenaria | Norma de diseño | Cadena ET / material (referencia) |
|-----------|-----------------|-----------------------------------|
| CA-160 Tipo A y B | NAE 300 (2ª ed., jun 2024) | Postes ET 03.364.101.0 · poleas ET 03.364.103.6 · sustentador ET 03.364.158.0 · hilo ranurado ET 03.364.291.9 |
| CA-220 | NAE 301 (2ª ed., jun 2024) | Ídem cadena CA-160 (secciones 185/2×150 mm²) |
| CA-160H / CA-200H | NAE 302 (1ª ed., ene 2022) | Ménsulas y pórticos de aluminio, equipos de compensación propios de las catenarias H |

Los **macizos de cimentación** de postes y anclajes se ejecutan según la
**NAE 106**. El pendolado y las agujas se ejecutan según la **NAE 116** y la
**NAE 115** (esta última complementada por las tipologías validadas del Anejo 1 de
la NAE 117). La verificación de compatibilidad pantógrafo–LAC se apoya en la
**UNE-EN 50367** y en la metodología de gálibo del pantógrafo de la **AESF
NT-03/2024**.

---

## 9. AUTOEVALUACIÓN (10 preguntas)

1. ¿Qué es una vía de tres carriles y qué función tiene el **cambiador de hilo**?
2. ¿Qué anchos de vía abarca la NAE 117 y a qué tensión se aplica?
3. Enumera las tipologías de catenaria compatibles con los pantógrafos de 1950 mm
   y con los de 1950 + 1600 mm.
4. ¿Qué descentramiento se fija en tres carriles y qué **banda común de
   frotamiento** genera?
5. ¿Cuál es la altura nominal del hilo, su altura máxima y la altura del sistema
   de catenaria en trayectos?
6. ¿Qué distancias de aislamiento (estática y dinámica) corresponden a la
   CA-220 y cuáles a la CA-160H?
7. ¿Qué «calle» (separación entre catenarias) y tolerancia tiene un seccionamiento
   de compensación? ¿Y uno de lámina de aire?
8. ¿Cuál es el vano máximo en seccionamientos de compensación de una CA-200H con
   pantógrafos de 1950 y 1600 mm? ¿Y en lámina de aire?
9. ¿Qué condiciones de cálculo (viento, altitud, temperatura, categoría de terreno)
   se emplean en las tablas de vanos de la norma?
10. ¿En qué punto de aguja se replantean las agujas cruzadas de un desvío de 500 m
    compatible con pantógrafos de 1950 y 1600 mm, y por qué?

---

## 10. REFERENCIAS

- **NAE 117** (3ª ed., dic 2024): «Línea aérea de contacto para vías con tres
  carriles electrificadas en corriente continua», 65 págs. (apdos. 1–10, tablas
  1–41, Anejos 1 y 2)
- **NAE 107** (2ª ed. + M1, 2024): definición y medida de parámetros de la LAC
- **NAE 112** (3ª ed. + M1, ene 2023): esquemas eléctricos de LAC en c.c.
- **NAE 300 / NAE 301 / NAE 302**: diseño funcional de CA-160 / CA-220 / CA-160H
  y CA-200H (ver Lección 2)
- **NAE 115**: agujas aéreas (ver Lección 4) · **NAE 116**: pendolado ·
  **NAE 106**: cimentaciones
- Reglamento (UE) 1301/2014 (ETI de Energía) · Orden TMA/135/2023 (IFE, IFI,
  Instrucción Ferroviaria de Gálibos)
- UNE-EN 50119:2021 (LAC) · UNE-EN 50122-1:2023 (seguridad, tierra y retorno) ·
  UNE-EN 50163 (tensiones de tracción) · UNE-EN 50367 (compatibilidad
  pantógrafo–LAC) · UNE-EN 15273 (gálibos) · UNE-EN 50526-1 (pararrayos c.c.)
- AESF NT-03/2024: metodología de cálculo del gálibo del pantógrafo

---

*Lección siguiente: retorno de corriente y puesta a tierra del sistema de
tracción en c.c. (UNE-EN 50122-1, NAE 112 y esquemas de seccionamiento).*
