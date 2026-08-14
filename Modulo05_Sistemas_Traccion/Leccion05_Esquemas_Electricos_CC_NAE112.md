# MÓDULO 5 – LECCIÓN 5

# ESQUEMAS ELÉCTRICOS DE LA LÍNEA AÉREA DE CONTACTO EN CORRIENTE CONTINUA (NAE 112)

## Documento base

> **NAE 112** — «Esquemas eléctricos de línea aérea de contacto en corriente continua».
> 3ª edición: febrero 2022 **+M1: enero 2023**. Aprobada por el Comité de Normativa
> (reunión de 30 de enero de 2023). Redactada por el Grupo de Trabajo **GT-300 (Línea
> Aérea de Contacto)**. 27 páginas. Aplicable a las instalaciones de línea aérea de
> contacto (LAC) en corriente continua de Adif, tanto en 3 kV c.c. como en 1,5 kV c.c.

---

## 1. RESULTADO DE APRENDIZAJE

> Al terminar esta lección serás capaz de **leer, interpretar y elaborar el esquema
> eléctrico unifilar de una Línea Aérea de Contacto en corriente continua según la
> NAE 112**: sabrás qué elementos deben representarse y cuáles no, qué simbología y
> nomenclatura fija la norma para fíderes y seccionadores, cómo se reflejan las
> fuentes de suministro (subestaciones y puestas en paralelo) y los seccionamientos,
> y por qué este documento es la pieza clave para ejecutar cortes de tensión en la
> red de Adif.

---

## 2. RESUMEN EJECUTIVO

La **NAE 112** normaliza la representación gráfica de la LAC en corriente continua.
Su origen es operativo: para aplicar el procedimiento **ADIF-PE-301-001-006-SC-521**
de «Cortes de Tensión en Líneas Aéreas de Contacto alimentadas en 25 kV c.a., 3 kV
c.c. y 1,5 kV c.c.», el Responsable del Corte de Tensión necesita un esquema
eléctrico **actualizado, unívoco y con nomenclatura común** que le permita
identificar los elementos a maniobrar y redactar los telefonemas correspondientes.

La norma persigue tres objetivos:

- **Unificar el formato y contenido** de los esquemas eléctricos unifilares de las
  LAC de corriente continua, incluidas sus fuentes de alimentación.
- **Definir la nomenclatura** de los elementos eléctricos de corte y alimentación
  (fíderes, seccionadores, aisladores de sección, seccionamientos).
- **Fijar la simbología** a emplear en cada caso.

El esquema es **unifilar y funcional**: se dibuja la catenaria como línea continua
coloreada, los fíderes como líneas discontinuas de trazado distinto, y se codifican
los seccionadores con letras y números según su **función** en el esquema
(independientemente de sus características constructivas). No se representan los
elementos de sustentación (postes, ménsulas, pórticos), las protecciones pasivas
(pararrayos, autoválvulas, cable y pozos de tierra) ni, con carácter general, los
fíderes de refuerzo y el fíder negativo.

La norma también regula el **cajetín**, los **formatos** (CAD/DWG, PDF, A4/A3) y la
posibilidad de un **plano llave** (hoja 0) para esquemas de más de dos hojas.

---

## 3. ALCANCE Y ESTRUCTURA DE LA NORMA

### 3.1 Campo de aplicación

Será de aplicación en **cualquier instalación de LAC en corriente continua de Adif**,
tanto en electrificaciones de **3 kV c.c.** como de **1,5 kV c.c.**, incluidos los
tramos de frontera con otros sistemas (zonas de separación) y las alimentaciones a
instalaciones ajenas.

### 3.2 Estructura del documento

| Capítulo | Contenido |
|----------|-----------|
| 1–4 | Antecedentes, objeto, campo de aplicación y generalidades |
| 5 | Sistema de Línea Aérea de Contacto (catenaria, fíderes, seccionamientos, aisladores, seccionadores, agujas, cruzamientos, zonas de separación) |
| 6 | Fuentes de suministro y elementos de control (subestaciones, puestas en paralelo, telemando, detectores de tensión) |
| 7 | Elementos auxiliares (edificio de viajeros, talleres y depósitos, túneles) |
| 8 | Simbología |
| 9 | Formatos y soportes |
| 10–12 | Normativa derogada, entrada en vigor, normativa de referencia |
| Anejo 1 | Planos tipo («Esquema eléctrico LAC») |

### 3.3 Generalidades de representación

- Las **vías** se designan conforme a la **Consigna Serie A** de la estación
  (criterios de la **NAG 2-0-1.0**): «VIA 1», o «via1»/«v1» en esquemas complejos.
- Los **puntos kilométricos** se indican como «PK 123/456» o «123/456».
- Deben referenciarse **obligatoriamente con P.K.**: los **seccionadores de vía
  general**, el **edificio de viajeros**, el **PLO de seccionadores**, la
  **subestación de tracción** y la **puesta en paralelo**.
- **No deben incluirse** elementos ajenos a la instalación salvo que sean necesarios
  para los cortes de tensión o la explotación del sistema de energía. El único
  elemento de infraestructura de inclusión obligatoria es el **edificio de viajeros**;
  los **túneles**, **viaductos en saltos de carnero** y **talleres/depósitos**
  alimentados desde Adif son optativos.

---

## 4. TIPOS DE ESQUEMAS Y CONFIGURACIONES ELÉCTRICAS

La NAE 112 no publica «esquemas tipo» en el sentido de un catálogo cerrado, sino que
define los **elementos** con los que se compone todo esquema unifilar y las **reglas**
de representación. De su articulado se derivan las configuraciones que se describen a
continuación.

### 4.1 Esquema de alimentación (fuentes y fíderes)

Es el esquema básico del circuito **positivo**. Recoge:

- **Subestaciones de tracción (S/E)** y **puestas en paralelo (P/P)**, representadas
  de forma **simplificada**: solo el número y orden de las salidas de fíder en el
  pórtico (posición física real), sin aparamenta interna.
- **Fíderes de alimentación**, que parten de la S/E o de la P/P y alimentan
  independientemente tramos de catenaria. Se dibujan como **línea discontinua de
  punto y raya** del mismo color que los tramos que alimentan, enlazando la salida
  de fíder numerada de la S/E/P/P con el **seccionador de punta de fíder** designado
  igual que el fíder.
- **Seccionadores de punta de fíder (F)**, normalmente cerrados, que independizan
  eléctricamente el fíder de la catenaria.

La numeración de fíderes es la clave del esquema (apartado 6.2).

### 4.2 Esquema de seccionamiento longitudinal

Permite **abrir eléctricamente la catenaria a lo largo de la vía** para acotar el
tramo sin tensión:

- **Seccionamientos de lámina de aire**, instalados junto a las señales de entrada y
  salida de estación o en el centro de estas, que **separan eléctricamente** dos
  tramos de catenaria (a la vez que independizan mecánicamente los cantones). Sí se
  representan, con el símbolo normalizado.
- **Seccionadores de zona neutra (ZN)**, que combinados entre sí (ZN y ZNbis, en
  estaciones sin S/E) o con los de los seccionamientos de trayecto establecen la
  **«Zona Neutra de seguridad»** necesaria para ejecutar los cortes de tensión.
- Los **seccionamientos de cantón** (que mantienen la continuidad eléctrica mediante
  conexiones fijas) **no se representan**.

### 4.3 Esquema de seccionamiento transversal y puestas en paralelo

Permite **seccionar entre vías o grupos de vías** y **puentear** alimentaciones:

- **Seccionadores de puenteo (P)**, normalmente abiertos, instalados en los
  seccionamientos de lámina de aire donde existe subestación; unen eléctricamente,
  a través de catenaria, los circuitos alimentados por dos fíderes distintos.
  Funcionan como **bypass** de la S/E.
- **Seccionadores ordinarios (S)**, normalmente cerrados, ubicados en vías de
  estación entre los seccionamientos de entrada y salida; independizan vías
  secundarias, grupos de vías o vías generales sin afectar al resto de la estación.
- **Puestas en paralelo (P/P)**: instalaciones que conectan en paralelo la catenaria
  de dos o más vías mediante disyuntores extrarrápidos y seccionadores, **sin aportar
  energía exterior**. En el esquema solo se refleja qué fíderes están normalmente
  unidos a la misma barra e interconectados.

### 4.4 Esquemas especiales y de frontera de sistemas

- **Vías con tensión conmutable** (3 kV c.c. / 25 kV c.a. o 3 kV / 1,5 kV c.c.): se
  representan con trazo doble (línea continua de color en paralelo con línea
  discontinua gris) e indicación de texto («3 kV~25 kV», «3 kV-1,5 kV»).
- **Zonas de Separación de Sistemas**: frontera entre la LAC de corriente continua
  (3 kV) y la de corriente alterna (25 kV). Aunque generalmente forman parte de la
  electrificación de c.a., **deben reflejarse en el esquema de c.c.** en tono gris,
  con sus seccionadores **ZS** numerados desde el lado de continua hacia el de
  alterna.
- **Zonas de Separación de Tensiones de continua**: separan catenarias de 3 kV c.c.
  de otras de 1,5 kV c.c. dentro de una misma estación (los retornos coinciden y los
  niveles de aislamiento son similares). La zona intermedia sin alimentación se
  representa en trazo continuo gris.
- **Fíder de continuidad**: conexión que puentea un tramo conmutable multitensión
  separado por seccionamientos de lámina de aire, para permitir la **alimentación en
  paralelo de subestaciones colaterales**; instalación excepcional que se rotula
  «FÍDER DE CONTINUIDAD».

### 4.5 Esquema del circuito de retorno

En corriente continua el retorno se realiza por los **carriles**, en paralelo con un
**fíder negativo** conectado a ellos. El fíder negativo **no se representa** en el
esquema eléctrico **salvo casos excepcionales** (negativo seccionable o conmutable en
sistemas multitensión), en cuyo caso se dibuja en un **esquema independiente** o como
**detalle diferenciado**, y se anota que no es un conductor activo aunque puede tener
diferencia de potencial con respecto a tierra.

---

## 5. ELEMENTOS REPRESENTADOS

| Elemento | Función en el esquema | ¿Se representa? | Clave de representación |
|----------|----------------------|------------------|--------------------------|
| Catenaria (sustentador + hilos de contacto) | Circuito positivo de alimentación al tren | **Sí, siempre** | Línea continua de color (azul vía par, rojo vía impar; otros colores salvo negro/gris para paquetes distintos) |
| Elementos de sustentación (postes, ménsulas, pórticos) | Soportan la LAC | **No** | — |
| Seccionamiento de cantón | Independiza mecánicamente cantones (mantiene continuidad eléctrica) | **No** | — |
| Seccionamiento de lámina de aire | Separa eléctricamente dos tramos | **Sí** | Símbolo normalizado, color del paquete eléctrico |
| Aislador de sección asimétrico | Independiza eléctricamente vías; el pantógrafo no pierde tensión | **Sí** | Símbolo normalizado + numeración correlativa por estación |
| Aislador de sección simétrico | Independiza eléctricamente; el pantógrafo pasa sin tensión | **Sí** | Símbolo normalizado (uso restringido: zonas de separación con espacio reducido, vías de talleres) |
| Fíder de alimentación | Alimenta tramos desde S/E o P/P | **Sí, obligatorio** | Línea discontinua de punto y raya, color del tramo alimentado |
| Fíder de acortamiento | Caso particular de fíder de alimentación que discurre fuera de la traza | **Sí** | Punto y raya + texto «ACORTAMIENTO» |
| Fíder de acompañamiento/refuerzo | Refuerza la sección del circuito positivo | **No, con carácter general** | Excepcional: raya y dos puntos + «FIDER DE REFUERZO» + anotación de riesgo |
| Fíder de continuidad | Puentea tramo conmutable multitensión; paralelo de subestaciones | **Sí (excepcional)** | Punto y raya + «FÍDER DE CONTINUIDAD» |
| Fíder negativo | Retorno de corriente en paralelo a los carriles | **No, salvo excepción** | Esquema independiente o detalle diferenciado |
| Seccionador de punta de fíder (F) | Independiza fíder y catenaria; NC | **Sí** | Letra F + nº del disyuntor extrarrápido |
| Seccionador de puenteo (P) | Une eléctricamente circuitos de dos fíderes; NA | **Sí** | Letra P + dos números separados por punto (p.ej. P1.5) |
| Seccionador de zona neutra (ZN) | Establece la Zona Neutra de seguridad para cortes de tensión | **Sí** | Letras ZN (+ bis), numeración por vía y lado de P.K. |
| Seccionador ordinario (S) | Independiza vías/grupos de vías en estación; NC | **Sí** | Letra S + dos números separados por punto (p.ej. S1.5, S5.3) |
| Seccionador especial (E) | Multipolar, condicionado, p.a.t. de emergencia en túnel, consumidores externos | **Sí** | Letra E + dos números (p.ej. E5.1) |
| Seccionador de Zona de Separación (ZS) | Seccionamiento en la frontera c.c./c.a. | **Sí** | Letras ZS + vía + correlativo (p.ej. ZS1.1); símbolo de c.a. |
| Disyuntor extrarrápido de S/E | Protección y salida de fíder | **Solo como número/orden de salidas** | No se dibuja su aparamenta interna; identifica al fíder |
| Pararrayos, autoválvulas, limitadores de tensión | Protección pasiva | **No** | No interfieren en la maniobra |
| Cable de tierra, pozos de tierra, conexiones equipotenciales | Protección pasiva | **No** | — |
| Subestación de tracción | Fuente de energía | **Sí (simplificada)** | «S/E NOMBRE» + P.K., lado de vía real, salidas de fíder |
| Puesta en paralelo | Pone en paralelo vías sin aportar energía | **Sí (simplificada)** | «P/P NOMBRE» + P.K., fíderes de barra interconectados |
| PLO de seccionadores | Mando a distancia de seccionadores | **Sí, obligatorio** | Doble rectángulo (telemando) o simple + «SOLO MANDO LOCAL» |
| Detector de tensión | Comprueba tensión en LAC/fíder; condiciona maniobras | **Solo excepcional** | Sistemas bitensión, seccionadores de p.a.t. de emergencia en túnel |
| Edificio de viajeros | Infraestructura singular de referencia | **Sí, obligatorio** | Símbolo propio + P.K., lado de vía real |
| Talleres y depósitos ajenos | Frontera con vías Adif / alimentaciones compartidas | **Opcional** | Línea punteada gris + texto descriptivo |
| Túneles | Puntos singulares, ≥ 1.000 m, catenaria rígida | **Opcional** | Línea punteada gris (nombre, P.K. de bocas, longitud) |
| Agujas aéreas | Paso del pantógrafo entre catenarias sin discontinuidad | **Sí (como referencia)** | Numeración del aparato de vía homólogo; sin símbolo específico |
| Cruzamiento / salto de carnero | Cruce de vías electrificadas al mismo nivel / elevado | **Sí** | Cruzamiento: punto de conexión eléctrica; salto: viaducto en punteado gris |

---

## 6. SIMBOLOGÍA Y NUMERACIÓN

### 6.1 Reglas generales

- La **catenaria** se representa como **línea continua de color**: **azul** para la
  vía general **par** y **rojo** para la vía general **impar**. Distintos paquetes
  eléctricos pueden identificarse con otros colores, **excepto negro y gris**
  (reservados para vías no electrificadas, vías ajenas y sistemas de c.a.).
- En estaciones mixtas 3 kV/1,5 kV: las catenarias de **1,5 kV** en **verde** con el
  texto «1,5 kV» al principio y final de cada vía; las que pueden alimentarse
  indistintamente por 3 kV o 1,5 kV con **doble línea azul-verde o rojo-verde** y el
  texto «3 kV-1,5 kV».
- **Vías no electrificadas**: líneas discontinuas negras. **Vías ajenas a Adif**:
  trazos discontinuos en gris. **Vías en 25 kV c.a.**: trazos discontinuos grises con
  «~25 kV».
- Límites de catenaria: **vía en topera** (trazo corto perpendicular, sin símbolo),
  **alto a la tracción eléctrica** con o sin continuidad de catenaria (símbolo propio,
  con P.K. opcional).
- **Fíderes de alimentación**: línea discontinua de **punto y raya**, del color del
  tramo que alimenta, entre la salida de fíder de la S/E/P/P y el seccionador de
  punta de fíder del mismo número. **Fíder de refuerzo**: línea de **raya y dos
  puntos** + «FIDER DE REFUERZO». **Fíder de acortamiento**: punto y raya +
  «ACORTAMIENTO».

### 6.2 Numeración de fíderes de alimentación

Los fíderes se designan por **números indicadores asociados a las vías** que
alimentan:

| Número | Función |
|--------|---------|
| F1 | Vía general 1, exterior de estación, lado de menor P.K. |
| F2 | Vía general 2, exterior de estación, lado de menor P.K. |
| F3 | Vía general 1, exterior de estación, lado de mayor P.K. |
| F4 | Vía general 2, exterior de estación, lado de mayor P.K. |
| F5 | Vía general 1 y/o vías secundarias impares, interior de estación |
| F6 | Vía general 2 y/o vías secundarias pares, interior de estación |
| F7 | Reservado a vías generales impares en estaciones con bifurcación (si no, vía secundaria impar) |
| F8 | Reservado a vías generales pares en estaciones con bifurcación (si no, vía secundaria par) |
| F9, F10 | Otras derivaciones a vías secundarias (bases de tracción, clasificaciones, etc.) |

**Desdoblamiento de vías generales** (subíndices):

| Fíder | Función |
|-------|---------|
| F11, F21, F31, … | Vía impar, lado de menor P.K. |
| F12, F22, F32, … | Vía par, lado de menor P.K. |
| F13, F23, F33, … | Vía impar, lado de mayor P.K. |
| F14, F24, F34, … | Vía par, lado de mayor P.K. |

**Ejemplo real de la norma (estación con 4 vías generales):**

- Fíderes de trayecto lado menor P.K.: **F1, F2, F11 y F12**.
- Fíderes de estación: **F5, F6, F15 y F16**.
- Fíderes de trayecto lado mayor P.K.: **F3, F4, F13 y F14**.

**Criterios de coherencia:** se procurará la **correlación de paridad** entre vías y
fíderes y que la **numeración creciente** de fíderes sea coherente con la
kilometración de la línea. Si no es posible (p. ej. red de ancho métrico) se añade
una anotación en el esquema. Se admite numeración alternativa justificada (p. ej. si
la S/E solo dispone de cinco disyuntores y precisa dos fíderes de estación, se
subdivide el **F5 en F51 y F52**).

### 6.3 Numeración de seccionadores

| Tipo | Regla | Ejemplos |
|------|-------|----------|
| Punta de fíder (F) | Letra F + nº del disyuntor extrarrápido | F1, F2, F7 |
| Punta de fíder en cascada | Nombre del fíder + sufijo «bis» para el más próximo a la S/E | F7, F7bis |
| Punta de fíder en derivación | Fíder + punto + vía alimentada | F7.3, F7.4 |
| Puenteo (P) | Letra P + fíder de trayecto + punto + fíder de estación/colateral | P1.5 (puentea F1 y F5) |
| Zona neutra, sin S/E | ZN / ZNbis; numeración por vía (par/impar) y lado de P.K. | ZN1, ZN1bis, ZN2, ZN2bis (menor P.K.); ZN3…ZN4bis (mayor P.K.) |
| Zona neutra, con S/E o P/P | ZN + número del fíder de la vía general | ZN1 (por el F1), ZN3 (por el F3) |
| Ordinario, sin S/E | S + vía general de la que se alimenta + punto + primera vía alimentada | S1.5 (alimenta la vía 5 desde la vía 1) |
| Ordinario, con S/E o P/P | S + nº del fíder + punto + primera vía alimentada | S5.3 (alimenta la vía 3 desde el fíder 5) |
| Ordinario en grandes estaciones | Tercer número (más cercano al punto de alimentación = .1) o sufijo «bis» | S5.10.1, S5.10.2 / S5.10, S5.10bis |
| Especial (E) | Letra E + fíder o vía general + punto + correlativo | E5.1 (alimentación externa desde el F5) |
| Zona de Separación (ZS) | Letras ZS + nº de vía + punto + correlativo, desde el lado de continua | ZS1.1, ZS1.2, ZS2.1, ZS2.2 |
| Estaciones multitensión | Prefijo acrónimo de estación + cifra (1 = 1,5 kV; 3 = 3 kV) + guion + designación | OV3-ZN1, OV1-ZN1 (Oviedo); GB3-S1.2, GI1-F1 (Gijón) |

**Reglas de P.K. en seccionadores:**

- Todos los seccionadores de **vía general** (ZN, P, F o S) se identifican
  **obligatoriamente** con su P.K.
- Si dos seccionadores de la misma función están **enfrentados en vías contiguas**
  (p. ej. ZN1 y ZN2, P1.5 y P2.6), basta con el P.K. de uno de ellos.
- En vías de **apartado o clasificación**, sin riesgo de error, puede omitirse el P.K.

**Posición normal de explotación:** los seccionadores se representan en su posición
normal, que por defecto es **Normalmente Cerrado (NC)** salvo los de **puenteo**
(**Normalmente Abierto, NA**). Si el estado no corresponde a lo normal o su función no
está clara, se indica **NC/NA** junto al símbolo.

### 6.4 Otros elementos numerados

- **Aisladores de sección**: numeración correlativa de menor a mayor P.K., con una
  serie que comienza en cada estación.
- **Agujas aéreas**: se designan con la numeración del **aparato de vía homólogo**
  (p. ej. escape entre vías generales con aparatos 3-4).
- **Salidas de fíder de S/E y P/P**: numeradas como los fíderes, incluso las
  subdivididas internamente (F5 → F51/F52).

---

## 7. CRITERIOS DE DISEÑO Y EJEMPLOS

### 7.1 Criterios generales de diseño del esquema

1. **Finalidad operativa:** el esquema debe permitir ejecutar cortes de tensión sin
   ambigüedad; por eso se prioriza la **claridad de las conexiones eléctricas** frente
   a la exactitud geométrica (p. ej. en la representación de los seccionadores de
   punta de fíder próximos a los de puenteo).
2. **Solo lo necesario:** se excluyen elementos ajenos y protecciones pasivas; el
   esquema es una herramienta de **maniobra y explotación**.
3. **Referencias geográficas:** P.K. obligatorios en seccionadores de vía general,
   edificio de viajeros, PLO, S/E y P/P; lado de vía real para estos últimos.
4. **Coherencia de nomenclatura:** paridad vía/fíder, numeración creciente con la
   kilometración, y coherencia con los **sinópticos del PLO y del Telemando de
   Energía** cuando son comunes a varios sistemas.
5. **Legibilidad y formato:** CAD compatible con DWG, publicación en PDF, tamaños
   A4/A3 con solape de hojas, plano llave (hoja 0) para más de dos hojas, y colores
   diferenciables también en impresión blanco y negro.

### 7.2 Ejemplo A — Línea de doble vía con subestación en estación

Para un esquema de doble vía general (vías 1 y 2) con S/E en la estación:

- **Catenarias:** vía 1 en **rojo** (impar), vía 2 en **azul** (par); líneas
  continuas desde los límites de electrificación (toperas o altos a la tracción).
- **Fíderes:** F1 (vía 1, lado menor P.K.), F2 (vía 2, lado menor P.K.), F3 (vía 1,
  lado mayor P.K.), F4 (vía 2, lado mayor P.K.), F5 (vía 1 y secundarias impares,
  interior), F6 (vía 2 y secundarias pares, interior). Cada uno sale del pórtico de la
  S/E en el orden físico real y llega a su **seccionador de punta de fíder**.
- **S/E:** se dibuja en el lado de vía real con «S/E NOMBRE» y su P.K.; solo salidas
  de fíder numeradas.
- **Seccionadores de zona neutra:** en los seccionamientos de lámina de aire de
  entrada/salida, denominados **ZN1/ZN1bis** (vía 1, lado menor P.K.), **ZN2/ZN2bis**
  (vía 2, lado menor P.K.), y **ZN3/ZN3bis, ZN4/ZN4bis** en el lado de mayor P.K.
  (Estaciones **con S/E**: la numeración sigue al fíder — ZN1 por el F1, etc.).
- **Puenteos:** en los seccionamientos donde está la S/E, **P1.5** (puentea F1 y F5),
  **P2.6** (puentea F2 y F6), etc., en posición NA.
- **Vías secundarias:** alimentadas con seccionadores ordinarios desde la vía
  general, p. ej. **S1.5** (alimenta la vía 5 desde la vía 1) o, con S/E, **S5.3**
  (vía 3 desde el fíder 5).

**Lógica de maniobra:** para aislar un tramo de trayecto se abre el ZNbis del lado
correspondiente; para alimentar una vía secundaria sin afectar a las generales se
abre su seccionador ordinario; el cierre de un puenteo (P) en la S/E deriva la
alimentación de un fíder a otro a través de catenaria sin usar el disyuntor del fíder
fallado.

### 7.3 Ejemplo B — Estación sin subestación ni puesta en paralelo

Cuando no hay S/E en la estación:

- Los fíderes de los **trayectos** (F1/F2, F3/F4) atraviesan la estación y se
  **puentean en las láminas de aire** mediante seccionadores de zona neutra en los
  extremos de los seccionamientos: el más próximo a la estación es **ZN** y el más
  alejado **ZNbis** (ZN1, ZN1bis, ZN2, ZN2bis por el lado de menor P.K.; ZN3,
  ZN3bis, ZN4, ZN4bis por el de mayor).
- La **Zona Neutra de seguridad** para el corte de tensión se forma cerrando/abriendo
  la combinación de estos ZN/ZNbis con los seccionadores de los seccionamientos de
  aire del trayecto, **sin necesidad de S/E en la dependencia**.

### 7.4 Ejemplo C — Estación con dos tensiones de alimentación

En estaciones donde conviven 3 kV y 1,5 kV (p. ej. ancho ibérico y ancho métrico):

- La catenaria de 1,5 kV se dibuja en **verde** con texto «1,5 kV»; la de 3 kV con la
  coloración normal (azul/rojo). Si una vía puede alimentarse indistintamente, doble
  línea azul-verde/rojo-verde con «3 kV-1,5 kV».
- Los seccionadores llevan el **prefijo de estación y tensión**: en Oviedo (nemónico
  «OV») → **OV3-ZN1** (3 kV) y **OV1-ZN1** (1,5 kV); en Gijón, con nemónicos distintos
  por ancho («GB» ibérico, «GI» métrico) → **GB3-S1.2** y **GI1-F1**.
- Entre ambas tensiones se representa una **Zona de Separación de Tensiones de
  continua** (pareja de aisladores simétricos o asimétricos con tramo corto intermedio
  sin alimentación y sin tierra, en gris).

### 7.5 Ejemplo D — Frontera de sistemas c.c./c.a.

El esquema de c.c. debe cerrarse en la **Zona de Separación de Sistemas**:

- Se dibuja en gris, con sus seccionadores **ZS1.1, ZS1.2, ZS2.1, ZS2.2…** numerados
  desde el lado de continua hacia el de alterna, usando el **símbolo de los esquemas
  de corriente alterna**.
- En los **cambiadores de ancho de vía** se representa además el edificio del
  cambiador.
- Si la zona de separación supera los ocho metros de longitud, podrán disponerse
  seccionadores de puenteo de los aisladores de sección más extremos (este extremo es
  diseño de c.a., pero condiciona el esquema de c.c.).

---

## 8. COORDINACIÓN CON OTRAS NORMAS

La NAE 112 no es un documento aislado: su aplicación se enmarca en el sistema
normativo de la electrificación ferroviaria de Adif.

| Norma / documento | Relación con NAE 112 |
|-------------------|----------------------|
| **NAG 2-0-1.0** (designación de vías y superestructura) | Cita expresa de la NAE 112: las vías se designan según la Consigna Serie A de cada estación siguiendo esta NAG |
| **ADIF-PE-301-001-006-SC-521** (cortes de tensión en LAC 25 kV c.a., 3 kV c.c. y 1,5 kV c.c.) | Justifica la existencia de la NAE 112: el esquema eléctrico actualizado es imprescindible para identificar los elementos a maniobrar y redactar los telefonemas |
| **NAE 107** (parámetros de la LAC) | Complementaria: mientras NAE 107 define los parámetros de diseño y cálculo de la catenaria (secciones, tensiones mecánicas, calibres), NAE 112 define **cómo se representan** esos circuitos en el esquema de explotación. El paquete eléctrico de NAE 112 (catenaria + fíder de acompañamiento energizados a la vez) debe ser coherente con las secciones y caídas de tensión calculadas según NAE 107 |
| **NAE 110 / NAE 111** (fíder de alimentación / circuito de retorno) | Los conductores que NAE 112 representa como **fíder de alimentación** y **fíder negativo** responden a las normas de cálculo e instalación de alimentación y retorno; NAE 112 fija solo su simbología, numeración y casos de representación |
| **NAE 300 / NAE 301** (diseño de LAC) | La propia norma es propuesta por el **GT-300 «Línea Aérea de Contacto»** (mismo grupo de trabajo del diseño de la LAC); los planos de diseño (NAE 300/301) deben ser coherentes con el esquema eléctrico de explotación que exige NAE 112 |
| **Consignas Serie A / RGD** | Fuente de los nemónicos de estación (prefijos de los seccionadores en estaciones multitensión) y de la designación de vías |
| **NAE 112 3ª ed. (feb. 2022)** | **Derogada** por la edición actual (+M1 ene. 2023), según su capítulo 10 |

---

## 9. AUTOEVALUACIÓN (10 preguntas)

**1.** ¿Cuál es el motivo operativo por el que Adif necesita un esquema eléctrico
actualizado de la LAC y una nomenclatura común?

**2.** ¿Qué dos tensiones de corriente continua cubre el campo de aplicación de la
NAE 112?

**3.** ¿Con qué color se representa la catenaria de la vía general par, y con cuál la
de la vía general impar?

**4.** ¿Qué elementos deben referenciarse obligatoriamente con su punto kilométrico?

**5.** ¿Por qué los fíderes de acompañamiento o refuerzo no se representan con
carácter general, y en qué casos excepcionales pueden incluirse?

**6.** ¿Qué diferencia hay entre un seccionamiento de cantón y un seccionamiento de
lámina de aire en cuanto a su representación en el esquema?

**7.** En una estación con subestación, ¿cómo se numera el seccionador de puenteo
P1.5 y qué fíderes pone en paralelo?

**8.** ¿Qué papel juegan los seccionadores ZN y ZNbis en una estación sin subestación?

**9.** En una estación multitensión (3 kV y 1,5 kV), ¿cómo se designan los
seccionadores de la estación de Oviedo según el ejemplo de la norma?

**10.** ¿Cuándo y cómo se representa el fíder negativo en el esquema eléctrico?

### Soluciones (respuestas cortas)

1. La ejecución correcta del procedimiento **ADIF-PE-301-001-006-SC-521** de cortes
   de tensión: el Responsable del Corte debe identificar sin ambigüedad los elementos
   a maniobrar y redactar los telefonemas.
2. **3 kV c.c. y 1,5 kV c.c.**
3. Vía general par en **azul**; vía general impar en **rojo**. (Otros colores, excepto
   negro y gris, para paquetes eléctricos distintos.)
4. Seccionadores de vía general, **edificio de viajeros**, **PLO de seccionadores**,
   **subestación de tracción** y **puesta en paralelo**.
5. Porque forman parte del **mismo paquete eléctrico** que la catenaria (se energizan
   y descargan a la vez). Excepcionalmente, cuando suponen singularidades con especial
   riesgo eléctrico: fíder **seccionable**, próximo a edificios ajenos o en postes
   independientes; se rotula «FIDER DE REFUERZO» y se añade anotación de peligro.
6. El **seccionamiento de cantón** mantiene la continuidad eléctrica mediante
   conexiones fijas y **no se representa**; el de **lámina de aire** separa
   eléctricamente dos tramos y **se representa** con su símbolo normalizado.
7. **P1.5** puentea los fíderes **F1** (trayecto) y **F5** (estación): el primer
   número es el fíder del trayecto y el segundo el de estación o colateral. Su
   posición normal es abierta (NA).
8. Permiten establecer la **Zona Neutra de seguridad** para los cortes de tensión:
   ZN es el más próximo a la estación y ZNbis el más alejado, en cada vía y a cada
   lado de la estación.
9. Con el prefijo del nemónico de la estación y la cifra de tensión: **OV3-…** para
   3 kV y **OV1-…** para 1,5 kV (p. ej. OV3-ZN1, OV1-ZN1).
10. Solo en casos excepcionales (negativo **seccionable o conmutable** en sistemas
    multitensión), en un **esquema independiente** del circuito positivo o como
    detalle diferenciado; no es un conductor activo con tensión, aunque puede tener
    diferencia de potencial con respecto a tierra.

---

## 10. REFERENCIAS

| Referencia | Título | Contenido integrado |
|------------|--------|---------------------|
| NAE 112 (3ª ed. + M1, ene. 2023) | Esquemas eléctricos de línea aérea de contacto en corriente continua | Todo el documento |
| NAG 2-0-1.0 | Designación de vías y componentes de la superestructura en la red | Sección 3 (designación de vías) |
| ADIF-PE-301-001-006-SC-521 | Cortes de tensión en líneas aéreas de contacto alimentadas en 25 kV c.a., 3 kV c.c. y 1,5 kV c.c. | Secciones 1–2, 4 (zona neutra de seguridad) |
| Consignas Serie A / RGD | Consultas de las consignas de estaciones | Secciones 3, 6.3 |
| NAE 107 | Parámetros de la LAC | Sección 8 (coordinación) |
| NAE 110 / NAE 111 | Fíder de alimentación / circuito de retorno | Secciones 4.5, 8 |
| NAE 300 / NAE 301 | Diseño de la LAC | Sección 8 (coordinación) |

---

*Lección 5 del Módulo 5 — esquemas eléctricos de la LAC en corriente continua según
la NAE 112 (3ª ed. + M1, enero 2023).*
