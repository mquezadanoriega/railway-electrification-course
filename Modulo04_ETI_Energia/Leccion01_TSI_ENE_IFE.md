# MÓDULO 4 · LECCIÓN 1

# LA ETI DE ENERGÍA (TSI ENE) Y LA INSTRUCCIÓN FERROVIARIA DE ENERGÍA (IFE)

## Documento base

> **Reglamento (UE) 2023/1697 de la Comisión, de 10 de agosto de 2023**, relativo a la
> especificación técnica de interoperabilidad del subsistema «energía» del sistema
> ferroviario de la Unión Europea. Es la ETI de Energía (TSI ENE) vigente; sustituye al
> Reglamento (UE) 1301/2014, que es la versión que cita la IFE.
>
> **Orden TMA/135/2023, de 15 de febrero** (BOE n.º 42, 18/02/2023), por la que se aprueban
> la Instrucción ferroviaria para el proyecto y construcción del subsistema de
> infraestructura (IFI) y la Instrucción ferroviaria para el proyecto y construcción del
> subsistema de energía (IFE, anexo II), y se modifican la Orden FOM/1630/2015 (gálibos)
> y la Orden FOM/2015/2016 (Catálogo Oficial de Señales). Corregida por la **Orden
> TRM/608/2024, de 15 de abril** (BOE-A-2024-12377).
>
> **Real Decreto 929/2020, de 27 de octubre**, sobre seguridad operacional e
> interoperabilidad ferroviarias, que incorpora al derecho interno la **Directiva (UE)
> 2016/797, de 11 de mayo de 2016**, sobre la interoperabilidad del sistema ferroviario.

---

## 1. RESULTADO DE APRENDIZAJE

> Al terminar esta lección serás capaz de **describir qué es la ETI de Energía (TSI ENE)
> y qué parámetros regula el subsistema de energía**, y de **explicar cómo la Instrucción
> Ferroviaria de Energía (IFE) la desarrolla en España**: conocer su estructura normativa
> (libros y apéndices de la Orden TMA/135/2023), manejar los valores de diseño concretos
> que exige (tensiones admitidas, alturas del hilo de contacto, desviaciones, distancias
> de aislamiento, fuerzas de contacto) y situarla dentro de la jerarquía Directiva
> (UE) 2016/797 → RD 929/2020 → ETI → Instrucciones Ferroviarias → normas técnicas del
> administrador de infraestructuras (NAE de ADIF).

---

## 2. RESUMEN EJECUTIVO

La **ETI de Energía** es la especificación técnica de interoperabilidad que fija los
requisitos que debe cumplir el **subsistema de energía** —el sistema de electrificación,
las líneas aéreas de contacto y el equipo en tierra de medición de energía— para que las
líneas y los trenes sean interoperables en toda la Unión Europea. Sus parámetros se
apoyan en normas europeas de la serie **EN 501xx**: tensiones de tracción (**EN 50163**),
líneas aéreas de contacto (**EN 50119**), hilos de contacto (**EN 50149**), puesta a tierra
y circuito de retorno (**EN 50122-1/-2/-3**) y coordinación alimentación–material rodante
(**EN 50367 y EN 50388**).

En España, la ETI se **complementa con una Instrucción Ferroviaria nacional**: la **IFE**,
aprobada como **anexo II de la Orden TMA/135/2023**. La IFE contiene:

- El **libro segundo**, con las **normas nacionales** que la propia ETI remite al Estado
  miembro (hoy, únicamente la geometría de la LAC en pasos a nivel).
- El **libro tercero**, con las **instrucciones adicionales**: parámetros que **no están
  incluidos en la ETI** y que España exige para el diseño (tensiones admitidas, geometría
  de la LAC, distancias de aislamiento, fuerzas de contacto, túneles, talleres, lavaderos,
  cambiadores de ancho…), además de los módulos de evaluación de la conformidad y la
  estrategia de aplicación a líneas nuevas y existentes.

**Por qué importa:** un subsistema de energía no puede autorizarse a la entrada en
servicio solo por cumplir la ETI; en España debe cumplir **simultáneamente la ETI (verificada
por un organismo notificado) y la IFE (normas nacionales verificadas por un organismo
designado e instrucciones adicionales verificadas por el promotor)**. El diseñador de
catenarias y subestaciones debe manejar los dos textos a la vez.

---

## 3. MARCO EUROPEO: DIRECTIVA 2016/797 Y RD 929/2020

### 3.1 La Directiva (UE) 2016/797 y el sistema de ETI

La Directiva (UE) 2016/797 establece las condiciones que deben cumplirse para lograr la
interoperabilidad del sistema ferroviario dentro de la Unión: **el sistema ferroviario se
divide en subsistemas**, de los que son de naturaleza estructural la infraestructura, la
energía, el control-mando y señalización (en tierra y a bordo) y el material rodante. Para
cada subsistema se elabora una **Especificación Técnica de Interoperabilidad (ETI)**, que
fija los **parámetros básicos**, sus requisitos, las interfaces con otros subsistemas y los
procedimientos de evaluación de la conformidad.

El artículo 14 de la Directiva obliga a notificar a la Agencia Ferroviaria de la Unión
Europea (ERA) las normas nacionales que afectan a la interoperabilidad; este es el cauce
por el que la IFE fue notificada antes de su aprobación.

### 3.2 El RD 929/2020, transposición interna

El Real Decreto 929/2020, de 27 de octubre, incorpora la Directiva al ordenamiento
español. Para la ETI de Energía y la IFE son claves estos artículos:

| Artículo RD 929/2020 | Contenido relevante |
|----------------------|---------------------|
| Art. 74 y 75 | Los subsistemas deben ser conformes con las ETI y las normas nacionales; las **Instrucciones Ferroviarias** complementan las ETI con las especificaciones no incluidas en ellas |
| Art. 76 | El Ministro de Transportes, Movilidad y Agenda Urbana, **a propuesta de la AESF**, puede aprobar Instrucciones Ferroviarias (IF) que deben cumplir los subsistemas y componentes para obtener la autorización de entrada en servicio |
| Anexo XI | Requisitos esenciales que debe cumplir todo subsistema: **seguridad, fiabilidad y disponibilidad, salud, protección medioambiental y compatibilidad técnica** |
| Art. 86 | Procedimiento de **disconformidad** cuando el solicitante considere que el subsistema no puede cumplir una norma |
| Art. 87 y anexo XII | Declaración de verificación del subsistema y procedimiento CE |
| Art. 106 y 107 | **Autorización de entrada en servicio** del subsistema de energía (líneas nuevas, establecimientos, renovaciones y acondicionamientos) |
| Art. 117 | Expediente técnico y régimen de informes de verificación |
| Art. 119 | **Registro de Infraestructura**: contiene los parámetros de red del subsistema de energía (p. ej. tensión, corriente en reposo) |

### 3.3 De la ETI 1301/2014 a la ETI 2023/1697

La IFE, publicada en 2023, cita como ETI de Energía de aplicación el **Reglamento (UE)
1301/2014**, que era la versión vigente en el momento de su redacción. Posteriormente, el
**Reglamento (UE) 2023/1697** ha aprobado la nueva ETI de Energía, que **deroga y sustituye**
al Reglamento (UE) 1301/2014. La estructura de parámetros que maneja la IFE (alimentación
eléctrica, geometría de la LAC, protección contra choques eléctricos, túneles) se mantiene
esencialmente alineada con la nueva TSI ENE, por lo que la lectura conjunta de ambos
documentos sigue siendo válida.

---

## 4. LA TSI ENE: PARÁMETROS DEL SUBSISTEMA DE ENERGÍA

### 4.1 Alcance del subsistema de energía

La ETI de Energía define el subsistema de energía como el conjunto formado por el **sistema
de electrificación**, las **líneas aéreas de contacto** y el **equipo en tierra del sistema
de medición y tarificación del consumo de electricidad**. Comprende las **subestaciones**
(que transforman la alta tensión de red en la tensión de tracción), los **puestos de
seccionamiento o puestas en paralelo**, las **secciones de separación** (fases y sistemas),
el **sistema de la línea aérea de contacto (LAC)**, el **circuito de retorno** de la
corriente de tracción y los equipos de medida de energía.

### 4.2 Parámetros regulados por la TSI ENE

| Parámetro básico | Requisito / valor característico | Norma de apoyo |
|------------------|----------------------------------|----------------|
| **Tensión y frecuencia** | 25 kV c.a. 50 Hz: nominal 25 kV; permanente entre **17,5 y 27,5 kV**; admisible 19 kV (10 min) y 29 kV (2 min). 3 kV c.c.: nominal 3 kV; permanente entre **2 y 3,6 kV**; admisible 1 kV (2 min) y 3,9 kV (5 min). Frecuencia 50 Hz con margen 49–51 Hz | EN 50163 |
| **Capacidad de transporte de corriente** | Dimensionado por la corriente máxima de los trenes, el calentamiento de los conductores y las corrientes en reposo (trenes parados) | EN 50119 |
| **Factor de potencia y tensión útil media** | La instalación fija debe garantizar una tensión útil media que permita la explotación prevista | EN 50388 |
| **Frenado de recuperación** | El sistema debe admitir la devolución de energía a la LAC por los trenes | EN 50388 |
| **Calidad de la energía** | Límites de armónicos, sobretensiones y perturbaciones en sistemas de c.a. (coordinación subestación–tren) | EN 50388 |
| **Geometría de la LAC** | Altura nominal del hilo de contacto (típicamente 5,3 m), altura mínima y máxima de diseño, desviación lateral, gradientes | EN 50119 |
| **Sección de línea de contacto** | Hilo de contacto acanalado de cobre o aleación de cobre; secciones típicas 100, 120, 150 y 170 mm² | EN 50149 |
| **Calidad de la captación de corriente** | Fuerza de contacto media y desviación estándar; fuerza mínima positiva (sin pérdida de contacto); criterios de simulación y medición | EN 50317, EN 50318, EN 50367 |
| **Separación entre pantógrafos** | Distancia de diseño entre pantógrafos en servicio simultáneo | EN 50367 |
| **Secciones de separación de fases y de sistemas** | Zonas neutras entre fases del mismo sistema y entre sistemas distintos (c.a./c.c.); paso con pantógrafo bajado en la separación de sistemas | EN 50119, EN 50367 |
| **Puesta a tierra y circuito de retorno** | Medidas de protección contra choques eléctricos, corrientes vagabundas y circuitos de retorno de tracción | EN 50122-1, EN 50122-2, EN 50122-3 |
| **Pantógrafos (interfaz)** | Geometría del arco del pantógrafo (1600 y 1950 mm según la ETI de Locomotoras y Material Rodante de Viajeros) y gálibos mecánico cinemático y eléctrico | EN 50206-1 |
| **Protección contra choques eléctricos** | Zona de la LAC (OCLZ) y zona de captación de corriente (CCZ) definidas por parámetros X, Y, Z | EN 50122-1 |

### 4.3 Componentes de interoperabilidad

La TSI ENE designa los **componentes de interoperabilidad** del subsistema de energía (entre
ellos la **línea aérea de contacto**), que deben contar con **declaración CE de conformidad**
antes de ponerse en el mercado. Los módulos de evaluación y la verificación CE del
subsistema se aplican según lo dispuesto en la propia ETI y, en España, en los capítulos 5 y
6 del libro tercero de la IFE.

---

## 5. LA IFE (TMA/135/2023): ALCANCE Y ESTRUCTURA

### 5.1 Qué es y en qué se apoya

La **Instrucción Ferroviaria para el proyecto y construcción del subsistema de energía
(IFE)** es el documento que recoge, en España, las especificaciones técnicas que **junto con
las ETI** debe cumplir el subsistema de energía para su autorización de entrada en servicio
por la **Agencia Estatal de Seguridad Ferroviaria (AESF)**. Se dicta en desarrollo del
artículo 76 del RD 929/2020 y del artículo 68.2 de la Ley 38/2015 del Sector Ferroviario, y
fue elaborada por la AESF con consulta a administradores de infraestructuras, empresas
ferroviarias, fabricantes, poseedores y mantenedores.

### 5.2 Ámbito de aplicación

La IFE se aplica al **proyecto, construcción y mantenimiento** del subsistema de energía de
las líneas de la **Red Ferroviaria de Interés General** de ancho ibérico (1.668 mm), estándar
europeo (1.435 mm) y métrico (excepto la línea Cercedilla-Cotos), así como a las **interfaces**
con los subsistemas de material rodante, infraestructura, control-mando y señalización y
explotación y gestión del tráfico, y a la parte del subsistema funcional de mantenimiento
relativa al subsistema de energía. No es aplicable en líneas con explotación tranviaria.

Es de aplicación obligatoria a **subsistemas nuevos**, **acondicionamientos o mejoras** y
**renovaciones**, según se definen en el RD 929/2020, con independencia de que requieran o no
autorización de entrada en servicio. En las sustituciones en el marco del mantenimiento se
aplica salvo que el administrador de infraestructuras justifique su inviabilidad técnica o
económica.

### 5.3 Estructura del anexo II de la Orden

| Parte | Contenido |
|-------|-----------|
| **Libro primero** | Consideraciones generales: antecedentes legales, objeto, ámbito, componentes de interoperabilidad, verificación del subsistema, estrategia de implementación |
| **Libro segundo** | **Normas nacionales** en el ámbito de la Directiva (UE) 2016/797: hoy, únicamente la **geometría de la LAC en los pasos a nivel** (parámetro 4.2.9 de la ETI ENE) |
| **Libro tercero** | **Instrucciones adicionales** y otros aspectos: definición del subsistema de energía, requisitos esenciales, especificaciones funcionales y técnicas (cap. 4), interfaces, normas de explotación, plan de mantenimiento, competencias profesionales, seguridad y salud, registro de infraestructura, componentes de interoperabilidad (cap. 5), evaluación de la conformidad y verificación del subsistema (cap. 6) y aplicación de la Instrucción a líneas nuevas, existentes y túneles (cap. 7) |
| **Apéndices** | A: glosario; B: referencias normativas (B.1 reglamentación, B.2 normas UNE-EN); C: verificación de las instrucciones adicionales y normas nacionales (cuadro C de fases de evaluación); D: cuestiones pendientes; E: cálculo de la desviación lateral máxima; F: velocidad básica fundamental del viento; G: sección de separación de sistemas |

### 5.4 La corrección de errores (Orden TRM/608/2024)

La Orden TRM/608/2024, de 15 de abril (BOE de 19/06/2024), corrigió errores detectados en la
Orden TMA/135/2023. Afecta principalmente a la IFI (gálibos, trazado, túneles, apéndices),
pero también al anexo II (IFE): en el apartado **6.2.5 «Evaluación del plan de
mantenimiento»**, se reordena el texto para precisar que, en relación con el apartado
6.2.4.7 de la ETI de Energía, **el organismo notificado solo comprobará que el plan de
mantenimiento está completo**.

---

## 6. REQUISITOS CONCRETOS DE LA IFE PARA EL DISEÑO

> Todos los valores de este capítulo proceden directamente del anexo II de la Orden
> TMA/135/2023 (texto extraído del BOE). Son límites para verificación; la IFE advierte de
> que **no deben aplicarse como valores habituales de diseño**, sino que el diseño debe
> quedar dentro de esos límites.

### 6.1 Sistema de alimentación (tensiones y frecuencia)

- **Regla general:** las líneas nuevas y la electrificación nueva de las existentes se
  proyectarán con **25 kV c.a. 50 Hz**, con alimentación **1 × 25 kV o 2 × 25 kV** (con
  centros de autotransformación), eligiendo uno u otro sistema mediante estudio
  técnico-económico que tenga en cuenta aspectos medioambientales.
- **3 kV c.c.:** solo se admite una electrificación nueva en **tramos de longitud reducida
  que sean prolongación de redes existentes**, debidamente justificada y autorizada por el
  administrador de infraestructuras, y siempre que la catenaria de 3 kV c.c. se proyecte
  con elementos y parámetros que permitan su **posterior adaptación a 25 kV c.a.** (por
  ejemplo, distancias de aislamiento calculadas para 25 kV).
- **Límite por velocidad:** se admiten 25 kV c.a. 50 Hz y 3 kV c.c., **excepto en las
  líneas con v ≥ 250 km/h, en las que solo se admite 25 kV c.a. 50 Hz**.
- **Corriente en reposo (3 kV c.c.):** la LAC se diseñará para soportar **200 A por
  pantógrafo con el tren en reposo**, salvo que el Registro de Infraestructura fije un valor
  superior.
- **Frenado de recuperación:** en c.c. se analizará la viabilidad técnico-económica de
  instalar **equipos inversores** en las subestaciones de tracción de nueva instalación.
- **Armónicos:** los subsistemas de energía y material rodante deben trabajar sin
  interferencias, sin superar los límites del administrador (apartado 10 de la UNE-EN 50388).

### 6.2 Geometría de la línea aérea de contacto

| Descripción | v ≥ 250 km/h | v < 250 km/h |
|-------------|--------------|--------------|
| Altura nominal del hilo de contacto | 5.300 mm | 5.300 mm |
| Altura mínima de diseño (HCW d,mín) | 5.080 mm | Según el gálibo elegido (cálculos del apdo. 4.1.2.2.1.4) |
| Altura máxima de diseño (HCW d,máx) | 5.300 mm | 6.000 mm |
| Desviación lateral máxima admisible | 400 mm (pantógrafo 1600 mm); 550 mm (pantógrafo 1950 mm) | 400 mm / 550 mm según pantógrafo |

- La altura máxima (HCW máx) se obtiene sumando a la altura máxima de diseño las
  tolerancias a5–a8 (vía, pantógrafo, instalación, desgaste y temperatura).
- En pasos a nivel de líneas v < 250 km/h (norma nacional del libro segundo), la altura
  máxima del hilo **no puede ser mayor de 6,20 m**; si no se consigue la altura del cuadro
  2.1, se montarán **pórticos de limitación de altura** y se garantizará una **distancia de
  aislamiento vertical de 0,50 m** entre el punto más alto del vehículo de carretera
  (incluida la carga) y las partes activas.

### 6.3 Gradiente de la altura del hilo de contacto

La variación de altura del hilo se conseguirá con el menor gradiente posible, sin superar
los valores siguientes (ya incluyen tolerancias de montaje y medida):

| Velocidad (km/h) | Máximo gradiente | Máxima variación de gradiente |
|------------------|------------------|-------------------------------|
| 60 | 1/50 (20 ‰) | 1/100 (10 ‰) |
| 100 | 1/167 (6 ‰) | 1/333 (3 ‰) |
| 120 | 1/250 (4 ‰) | 1/500 (2 ‰) |
| 160 | 1/500 (2 ‰) | 1/1.000 (1 ‰) |
| 200 | 1/1.000 (1 ‰) | 1/2.000 (0,5 ‰) |
| > 250 | 1/2.500 (0,4 ‰) | 1/5.000 (0,2 ‰) |

Para velocidades entre 120 y 200 km/h, si no se pueden alcanzar estos valores, se cumplirán
al menos los de la tabla 12 de la UNE-EN 50119.

### 6.4 Tolerancias, cargas de hielo y altura mínima de diseño

- **Tolerancia vertical de la vía (a1):** 20 mm en vía balastada; 5 mm en vía en placa.
- **Tolerancia de montaje del hilo (a2):** 10 mm.
- La altura mínima de diseño se calcula por las **hipótesis estática y dinámica** por
  separado, adoptando la más restrictiva: HCW d,mín = máx (HCW d,mín,EST; HCW d,mín,DIN).
- **Cargas de hielo** sobre sustentador/otros cables y sobre hilos de contacto:

| Altitud sobre el nivel del mar | Carga en sustentador y otros cables (N/m) | Carga en hilos de contacto (N/m) |
|--------------------------------|--------------------------------------------|----------------------------------|
| 0–499 m | 0 | 0 |
| 500–1.000 m | 3,5 | 1,75 |
| 1.001–1.500 m | 7 | 3,5 |
| > 1.500 m | 15 | 7,5 |

En túneles se puede aplicar el coeficiente corrector **Ktun** (de 0,2 a 1,0) según la
longitud del túnel y la altitud.

### 6.5 Fuerzas de contacto y calidad de la captación

- **Fuerza de contacto estática** (parámetro no incluido en la ETI): 25 kV c.a. **60 a 90 N**;
  3 kV c.c. **90 a 120 N**.
- **Fuerza de contacto media** (límite máximo en el cuadro 4.1.2.2.5.a):

| Sistema | Velocidad | Fuerza media máxima (N) |
|---------|-----------|--------------------------|
| 25 kV c.a. | v ≤ 200 km/h | 300 |
| 25 kV c.a. | 200 < v ≤ 320 km/h | 350 |
| 25 kV c.a. | v > 320 km/h | 400 |
| 3 kV c.c. | v ≤ 200 km/h | 300 |
| 3 kV c.c. | v > 200 km/h | 400 |

- La **fuerza de contacto mínima debe ser positiva** (no se admite pérdida de contacto). El
  criterio de calidad es que **Fm + 3σ ≤ valor máximo** y **Fm − 3σ > 0**; la desviación
  estándar máxima σmax = **0,3 · Fm**.
- **Espacio para la elevación del brazo de atirantado:** mínimo **2 · S0** (admisible
  1,5 · S0 si la elevación está físicamente limitada, según el apartado 5.10.2 de la
  UNE-EN 50119).
- Para componentes rígidos (p. ej. aisladores de sección) con v ≤ 200 km/h, la fuerza de
  contacto puede aumentar hasta **350 N**.

### 6.6 Pantógrafos y gálibos

- La LAC se diseñará al menos para los pantógrafos definidos en la ETI de Locomotoras y
  Material Rodante de Viajeros (Reglamento (UE) 1302/2014), apartados **4.2.8.2.9.2.1
  (arco de 1600 mm)** y **4.2.8.2.9.2.2 (arco de 1950 mm)**. En líneas renovadas o
  acondicionadas alimentadas en 3 kV c.c. basta con el de 1950 mm; en líneas de 25 kV c.a.
  deben admitirse ambos.
- **Ningún componente del subsistema de energía puede entrar en el gálibo mecánico
  cinemático del pantógrafo** salvo el hilo de contacto y el brazo de atirantado; los
  elementos conectados a tierra o a potencial distinto deben quedar además fuera del
  **gálibo eléctrico**.
- Los gálibos se determinan según la **Instrucción Ferroviaria de Gálibos (Orden
  FOM/1630/2015)**. Para el cálculo de la desviación lateral, el semiancho de la zona
  conductora del arco (bw,c) es: europantógrafo de 1600 mm → **600 mm**; de 1950 mm →
  **775 mm**; pantógrafo RENFE de 1950 mm → **755 mm**; pantógrafo RENFE de 1860 mm →
  **710 mm**.
- En líneas de 3 kV c.c. con futura transformación a 25 kV, el **gálibo eléctrico** debe
  calcularse con las distancias de aislamiento de 25 kV.

### 6.7 Secciones de separación de fases y de sistemas (zonas neutras)

- **Separación de fases:** se evitará instalarla en el interior de túneles, cerca de señales
  de parada, en curvas de radio reducido o en rampas pronunciadas; si resulta inevitable, se
  justificará con **simulaciones de marcha** (ningún tren detenido en la zona neutra) y, en
  túneles, con una evaluación del riesgo según los métodos comunes de seguridad (Reglamento
  de Ejecución (UE) 402/2013).
- **Separación de sistemas (c.a./c.c.):** el paso se realiza con **pantógrafo bajado e
  interruptores principales abiertos**, sin tocar el hilo de contacto; la sección debe
  eliminar los arcos por pantógrafo levantado de forma no intencionada (detectores de
  tensión, inductivos, de elevación del hilo, etc.). En el apéndice G la longitud total de la
  sección neutra debe cumplir **D ≤ 8 m**, y la puesta a tierra del punto central solo se
  realiza si uno de los dos sistemas es c.a. (conectándose a la tierra del sistema de c.a.
  cuando no estén interconectadas).
- **Distancias de aislamiento entre fases distintas (cuadro 4.1.2.2.12):**

| Tensión nominal | Diferencia de fase | Tensión relativa | Estática (mm) | Dinámica (mm) |
|-----------------|--------------------|------------------|---------------|---------------|
| 25 kV | 120° | 43,3 kV | 400 | 230 |
| 25 kV | 180° | 50 kV | 540 | 300 |

### 6.8 Distancias de aislamiento a tierra y entre conductores

- Las distancias de aislamiento entre partes en tensión de la LAC y tierra cumplirán el
  **apartado 5.1.3 de la UNE-EN 50119**. En líneas nuevas de 3 kV c.c. se aplicarán las
  **distancias de c.a.** de la tabla 2 de la UNE-EN 50119 para prever el cambio a 25 kV.
- **Distancia entre conductores en paralelo** (cables desnudos de la LAC, distintos del hilo
  de contacto, sustentador y péndolas): será de aplicación el apartado **5.4.1 de la
  ITC-LAT 07 del RD 223/2008**, con la fórmula D = K·√F + L + K'·Dpp, con K = 0,6, K' = 0,75 y
  Dpp = **0,70 m** para conductores de fase de 25 kV (0,80 m si hay diferencia de fase de
  180°) y **0,10 m** para 3 kV c.c.

### 6.9 Protección contra choques eléctricos

Los parámetros que definen la **zona de la línea aérea de contacto (OCLZ)** y la **zona de
captación de corriente (CCZ)** de la UNE-EN 50122-1 se fijan en:

| Parámetro | Valor |
|-----------|-------|
| X (semibase de la OCLZ) | **5,0 m** |
| Y (semibase de la CCZ) | **2,0 m** |
| Z (distancia vertical HP–SH) | **1,5 m** |

En andenes, talleres y lugares similares, la zona se amplía al rectángulo OCLZP (X a ambos
lados del eje de la vía hasta el punto más alto de la LAC).

### 6.10 Suspensión y compensación

- Por encima de **100 km/h** se usará catenaria con **sustentador** (u otro sistema de
  suspensión); la catenaria sin sustentador solo se admite excepcionalmente en puntos
  singulares.
- **Hilos de contacto compensados** por encima de 100 km/h; **sustentador compensado** por
  encima de 120 km/h; **compensación independiente** de sustentador e hilo por encima de
  140 km/h.
- Se evitará ubicar los **elementos de compensación en el interior de los túneles**; si no
  es posible, la geometría y el volumen ocuparán el mínimo espacio en el entorno de los
  pasillos de evacuación definidos por la IFI.

### 6.11 Túneles, instalaciones auxiliares y cambio de ancho

- **Túneles:** se dispondrán **dispositivos de puesta a tierra de la LAC** en los puntos de
  acceso al túnel y cerca de las separaciones entre secciones, como instalaciones fijas
  accionadas manualmente y/o por telemando; en c.c. la conexión se hará **a tierra y al
  carril de retorno**. La ubicación de los seccionadores se reflejará en el **Plan de
  Autoprotección** del túnel.
- **Instalaciones de lavado bajo catenaria:** dispondrán de protección que impida la puesta
  en marcha del lavado mientras no se produzca la **puesta a tierra de la LAC**, mediante
  seccionador controlado a distancia **enclavado** con el dispositivo de puesta en marcha, y
  con avisos visuales y acústicos durante la reposición de tensión.
- **Talleres con acceso a zona de pantógrafos:** acceso condicionado a la puesta a tierra de
  la catenaria mediante un **sistema de llaves enclavadas** (caja de enclavamiento
  electromecánica): las llaves de acceso solo pueden extraerse si la catenaria está
  desconectada y puesta a tierra, y la llave de alimentación solo puede liberarse cuando
  todas las llaves de acceso están introducidas. Separación eléctrica con **doble
  aislamiento**.
- **Cambiadores de ancho:** la zona del cambiador se electrifica por ambos lados (con
  longitud suficiente en el lado sin electrificar para evitar el impacto del pantógrafo
  levantado); la catenaria del cambiador queda **aislada eléctricamente** de los tramos
  colaterales; si la alimentación es distinta, se instalarán señales de bajada y subida de
  pantógrafo; el aislador más próximo a la fachada del edificio estará a una **distancia
  mínima de 2 m**.

### 6.12 Evaluación de la conformidad y aplicación

- **Normas nacionales (libro segundo):** las verifica un **organismo designado**.
- **ETI (requisitos europeos):** los verifica un **organismo notificado** (declaración CE de
  verificación).
- **Instrucciones adicionales (cap. 4 del libro tercero):** las verifica el **promotor**, por
  medio de un organismo de certificación o de un organismo evaluador interno, en las fases de
  diseño y producción según el **cuadro C del apéndice C**; el informe se integra en el del
  artículo 117 del RD 929/2020.
- **Aplicación:** línea nueva y establecimiento de la electrificación requieren autorización
  de entrada en servicio (art. 106 RD 929/2020); en acondicionamientos y renovaciones, la
  AESF decide según el alcance (art. 107); la **sustitución en el marco del mantenimiento no
  requiere autorización** y, en líneas existentes sin renovar, puede aplicarse
  voluntariamente el procedimiento de **verificación IE** de la Recomendación 2014/881/UE.

---

## 7. INTERFACES CON OTRAS ETI Y CON LAS NAE DE ADIF

### 7.1 Interfaces con otros subsistemas (apartado 4.2 de la IFE)

| Subsistema / ETI | Interfaces con el subsistema de energía |
|------------------|------------------------------------------|
| **Material rodante** (ETI 1302/2014; IF MR ALC-20) | Tensión y frecuencia, corriente máxima del tren, factor de potencia, corriente en reposo, frenado de recuperación, protección eléctrica del tren, geometría y gálibo del pantógrafo, fuerzas de contacto, material del frotador, circulación por secciones de separación |
| **Infraestructura** (IFI) | Gálibo del pantógrafo ↔ gálibo de implantación de obstáculos; sistemas de compensación ↔ pasillos de evacuación en túneles; electrificación ↔ instalaciones de cambio de ancho; lavado bajo catenaria ↔ instalaciones de limpieza exterior; postes en andenes ↔ anchura de andenes |
| **Control-mando y señalización** (ETI 2016/919) | Órdenes a los equipos del material rodante para las **secciones de separación de fases y de sistemas** |
| **Explotación y gestión del tráfico** (ETI 2019/773) | Compatibilidad de la ruta y composición del tren, preparación del libro de itinerarios (corriente máxima, secciones de separación) |
| **Seguridad en túneles** (ETI 1303/2014) | Segmentación y puesta a tierra de la LAC en túneles, procedimientos de desconexión y puesta a tierra |
| **Accesibilidad** (ETI 1300/2014) | Ubicación de los postes de electrificación en los andenes (anchura y borde de andenes) |

### 7.2 Relación con las NAE de ADIF

La **disposición adicional segunda de la Orden TMA/135/2023** obliga a los administradores
de infraestructuras a **adaptar sus sistemas de gestión de seguridad y su normativa técnica
interna** al contenido de las Instrucciones: presentación de un programa de adaptación en
**6 meses** y demostración de la adaptación en **24 meses** desde la entrada en vigor.

En ADIF, esa normativa técnica interna es el conjunto de **Normas y Recomendaciones técnicas
(NAE) y Especificaciones Técnicas (ET)** de la LAC (por ejemplo, las ET 03.364.xxx de
herrajes y fijaciones, la NAE 201 de grapas tipo cuña o las ET de catenarias, postes y
subestaciones). La jerarquía práctica en un proyecto es:

```
Directiva (UE) 2016/797 → RD 929/2020 → ETI de Energía (2023/1697)
                                        ↓ (complemento nacional)
                          IFE (anexo II Orden TMA/135/2023) + IFI + IF Gálibos
                                        ↓ (detalle de construcción)
                          NAE y ET de ADIF (adaptadas a la IFE)
```

Las NAE y ET no pueden contradecir a la ETI ni a la IFE; concretan soluciones constructivas
aceptadas por el administrador dentro de los límites que fija la Instrucción. Por eso un
proyecto de electrificación debe verificarse simultáneamente contra la IFE (límites de
diseño) y contra las NAE/ET (solución constructiva).

---

## 8. AUTOEVALUACIÓN (10 preguntas)

**1.** ¿Qué dos documentos normativos debe cumplir en España el subsistema de energía para su
autorización de entrada en servicio, y quién verifica cada uno?

**2.** ¿Qué tensiones de tracción admite la IFE y qué sistema se exige en las líneas de
v ≥ 250 km/h?

**3.** Según la EN 50163, ¿cuál es el rango de tensión permanente de un sistema de 25 kV c.a.
50 Hz y cuál el de 3 kV c.c.?

**4.** ¿Cuál es la altura nominal del hilo de contacto y la altura máxima de diseño en líneas
de v < 250 km/h según la IFE?

**5.** ¿Qué distancia de aislamiento vertical debe garantizarse en los pasos a nivel entre el
vehículo de carretera (con carga) y las partes activas de la LAC?

**6.** ¿Qué límite fija la IFE para la fuerza de contacto media en un sistema de 25 kV c.a. a
v = 350 km/h, y qué significa que la fuerza mínima deba ser positiva?

**7.** ¿Cómo debe realizarse el paso de un tren por una sección de separación de sistemas
c.a./c.c., y qué valor máximo de longitud D exige el apéndice G?

**8.** ¿Qué valores tienen los parámetros X, Y y Z de protección contra choques eléctricos?

**9.** ¿Qué sistema de enclavamiento exige la IFE para las instalaciones de talleres con
acceso a zona de pantógrafos?

**10.** ¿Qué obligación impone la disposición adicional segunda de la Orden TMA/135/2023 a los
administradores de infraestructuras respecto de su normativa técnica interna (NAE/ET)?

### Soluciones (respuestas cortas)

1. La **ETI de Energía** (verificada por el **organismo notificado**, declaración CE) y la
   **IFE** —sus **normas nacionales** (verificadas por el **organismo designado**) y sus
   **instrucciones adicionales** (verificadas por el **promotor**)—. El promotor emite la
   declaración de verificación del subsistema.
2. **25 kV c.a. 50 Hz** y **3 kV c.c.** (solo en tramos de longitud reducida, prolongación de
   redes existentes, justificados y autorizados). En líneas de **v ≥ 250 km/h solo se admite
   25 kV c.a. 50 Hz**.
3. 25 kV c.a.: entre **17,5 y 27,5 kV** en régimen permanente (con valores de corta duración
   de 19 kV/10 min y 29 kV/2 min). 3 kV c.c.: entre **2 y 3,6 kV** permanente (1 kV/2 min y
   3,9 kV/5 min como valores de corta duración). Frecuencia 49–51 Hz.
4. **Altura nominal de 5.300 mm** y **altura máxima de diseño de 6.000 mm** (la altura
   máxima no puede superar 6,20 m en pasos a nivel y casos singulares).
5. **0,50 m** entre el punto más alto del vehículo de carretera (incluida su carga) y las
   partes activas, garantizando además que la altura máxima del hilo no supere 6,20 m.
6. Para v > 320 km/h, **máximo 400 N**; la fuerza mínima debe ser **positiva** para asegurar
   que **no hay pérdida de contacto** entre pantógrafo e hilo (Fm − 3σ > 0).
7. Con el **pantógrafo bajado** y los **interruptores principales abiertos**, sin tocar el
   hilo de contacto. El apéndice G exige una longitud total de sección neutra **D ≤ 8 m**.
8. **X = 5,0 m**, **Y = 2,0 m** y **Z = 1,5 m** (UNE-EN 50122-1), que definen la zona de la
   LAC (OCLZ) y la zona de captación de corriente (CCZ).
9. Un **sistema de llaves enclavadas** (caja de enclavamiento electromecánica): las llaves de
   acceso a la zona de pantógrafos solo se liberan si la catenaria está **desconectada y
   puesta a tierra**, y la llave de alimentación solo puede liberarse cuando todas las llaves
   de acceso están introducidas; separación con **doble aislamiento**.
10. Adaptar sus **sistemas de gestión de seguridad y su normativa técnica interna (NAE/ET)**
    al contenido de las Instrucciones: presentar un programa de adaptación en **6 meses** y
    demostrar la adaptación en **24 meses** desde la entrada en vigor de la Orden.

---

## 9. REFERENCIAS

| Referencia | Título | Contenido integrado |
|------------|--------|---------------------|
| Reglamento (UE) 2023/1697 | ETI de Energía (TSI ENE) del sistema ferroviario de la Unión | Sección 4 |
| Reglamento (UE) 1301/2014 | ETI de Energía anterior, citada por la IFE | Secciones 3, 5 y 6 |
| Orden TMA/135/2023 (BOE-A-2023-4324) | IFI + IFE (anexo II) y modificación de gálibos y señales | Secciones 3, 5, 6 y 7 |
| Orden TRM/608/2024 (BOE-A-2024-12377) | Corrección de errores de la Orden TMA/135/2023 | Sección 5.4 |
| Real Decreto 929/2020 | Seguridad operacional e interoperabilidad ferroviarias | Sección 3 |
| Directiva (UE) 2016/797 | Interoperabilidad del sistema ferroviario de la UE | Sección 3 |
| Ley 38/2015 | Ley del Sector Ferroviario (art. 65 y 68.2) | Secciones 3 y 5 |
| UNE-EN 50163 | Tensiones de alimentación de las redes de tracción | Secciones 4 y 6 |
| UNE-EN 50119, 50149, 50122-1/-2/-3 | LAC, hilos de contacto, puesta a tierra y retorno | Secciones 4 y 6 |
| UNE-EN 50317, 50318, 50367, 50388 | Captación de corriente y coordinación alimentación–tren | Secciones 4 y 6 |
| Reglamento (UE) 1302/2014 | ETI de Locomotoras y Material Rodante de Viajeros (pantógrafos) | Secciones 4 y 6 |
| Reglamento (UE) 1303/2014 | ETI de Seguridad en Túneles Ferroviarios | Secciones 4 y 7 |
| Orden TMA/576/2020 (IF MR ALC-20) | Especificaciones de material rodante (interfaz) | Sección 7 |
| Orden FOM/1630/2015 | Instrucción Ferroviaria de Gálibos | Secciones 6 y 7 |
| RD 223/2008 (ITC-LAT 07) | Líneas eléctricas de alta tensión (distancias entre conductores) | Sección 6.8 |
| NAE y ET de ADIF | Normativa técnica interna del administrador (p. ej. ET 03.364.xxx, NAE 201) | Sección 7.2 |

---

*Lección 1 del Módulo 4 — la ETI de Energía (TSI ENE) y su desarrollo en España mediante la
Instrucción Ferroviaria de Energía (IFE). Contenido extraído del BOE-A-2023-4324 (Orden
TMA/135/2023) y BOE-A-2024-12377 (Orden TRM/608/2024).*
