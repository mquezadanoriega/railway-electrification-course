# MÓDULO 5 · LECCIÓN 6

# ESQUEMAS ELÉCTRICOS DE LA LÍNEA AÉREA DE CONTACTO EN 25 KV C.A. (NAE 119)

## Documento base

| Referencia | Título | Edición | Páginas |
|------------|--------|---------|---------|
| NAE 119 | Esquemas eléctricos de línea aérea de contacto en 25 kV C.A. | 1ª edición, junio 2025 | 54 |

> La NAE 119 (1ª ed., junio 2025), elaborada por el Grupo de Trabajo **GT-300 · Línea Aérea de Contacto** y aprobada por el Comité de Normativa, **unifica el formato y el contenido de los esquemas eléctricos unifilares de las líneas aéreas de contacto de 25 kV c.a. 50 Hz** (valor de tensión permanente máximo **27,5 kV** según UNE-EN 50163), incluidas sus fuentes de alimentación. Define la **simbología y leyenda general** y la **nomenclatura de los elementos eléctricos de corte y alimentación**, de modo que el Responsable del Corte de Tensión pueda identificar inequívocamente los elementos a maniobrar y redactar correctamente los telefonemas.

---

## 1. RESULTADO DE APRENDIZAJE

> Al terminar esta lección serás capaz de **leer, interpretar y explotar un esquema eléctrico unifilar de línea aérea de contacto de 25 kV c.a. de Adif** conforme a la NAE 119: distinguir los sistemas de alimentación **1x25 kV y 2x25 kV**, identificar los **seccionamientos, zonas neutras, zonas de separación de sistemas y elementos de corte y protección**, descifrar la **nomenclatura normalizada** de cada seccionador, y comprender el **esquema de retorno y puesta a tierra** en corriente alterna. También sabrás situar la NAE 119 en el marco normativo de energía de Adif (NAE 112 para c.c., NAE 300/301/302 para LAC y ET de subestaciones 25 kV).

---

## 2. RESUMEN EJECUTIVO

Los **esquemas eléctricos unifilares** son la herramienta imprescindible para ejecutar los **cortes de tensión** en líneas alimentadas en 25 kV c.a., 3 kV c.c. y 1,5 kV c.c. (Procedimiento General ADIF-PE-301-001-006-SC-521). Sin un esquema actualizado que identifique los elementos a maniobrar, no es posible redactar con seguridad los telefonemas de corte y reposición.

La NAE 119 establece, para todo el ámbito de Adif y Adif AV:

- **Sistemas de electrificación:** coexistencia de dos sistemas en c.a.: **1x25 kV** (retorno por carriles y cable de retorno a tierra) y **2x25 kV** (con **feeder negativo** a −25 kV y **autotransformadores** intermedios y finales que reparten la corriente de retorno).
- **Un único lenguaje gráfico:** colores (catenaria en **negro**, feeder negativo en **rojo**, vías sin electrificar en gris discontinuo, 3 kV c.c. en naranja), símbolos normalizados y leyenda general.
- **Nomenclatura inequívoca de seccionadores:** punta de feeder de catenaria (**SE XXX-CX**), punta de feeder negativo (**SE XXX-FX**), autotransformador intermedio (**ATI XXX.X-FCX**), autotransformador final (**ATF XXX.X-FCX**), zona neutra (**SE/ATF XXX-ZNX**), puenteo de feeder negativo (**SE/ATF XXX-NX**), ordinarios (**XXX-SX**), pórtico de distribución (**EST-B1…BVn, BP12**), puesta en paralelo (**XXX-PXX**), vías secundarias (**XXX-SXX**) y servicios auxiliares (**XXX-(CT/PIC/PCA/ET/T/BTS/OP/DCC/DCO/DRC/EM/PB)N**).
- **Referenciación geográfica:** vías designadas según la Consigna Serie A y numeradas conforme a NAG 2-0-1.0; puntos kilométricos en formato **"PK 123+456"** o **"PK 123/456"**.
- **Formato de edición:** trazado en CAD compatible con **DWG**, publicación en **PDF**, impresión en **A4/A3**, con cajetín normalizado.

**Por qué importa:** el esquema eléctrico es el documento operativo que permite ejecutar cortes de tensión con seguridad, localizar averías y planificar la explotación. Una nomenclatura común evita interpretaciones erróneas entre los responsables de mantenimiento, los centros de control y los equipos de obra.

---

## 3. ALCANCE Y ESTRUCTURA DE LA NORMA

### 3.1 Objeto y campo de aplicación

- **Objeto:** unificar el formato y contenido de los esquemas eléctricos **unifilares** de las LAC de **25 kV c.a. 50 Hz**, incluidas sus fuentes de alimentación, definiendo simbología, leyenda y nomenclatura de los elementos de corte y alimentación.
- **Campo de aplicación:** cualquier instalación de LAC de **corriente alterna de Adif** para electrificaciones en 25 kV, y todos los esquemas cuya elaboración se inicie a partir de su entrada en vigor.
- **Actualización:** los esquemas anteriores a la vigencia se actualizarán a lo dispuesto en esta NAE cuando se realicen actuaciones que impliquen su modificación o cuando se actualicen por otros motivos.

### 3.2 Estructura del documento

La norma se organiza en 12 apartados y 2 anejos:

| Apartado | Contenido |
|----------|-----------|
| 1–3 | Antecedentes, objeto, campo de aplicación |
| 4 | Sistemas de electrificación de c.a. (1x25 kV y 2x25 kV) |
| 5 | Generalidades (designación de vías, PK, referencias) |
| 6 | Sistema de LAC: catenaria, feeders, seccionamientos, aislamientos, seccionadores, agujas aéreas, escapes y breteles, PBA, PAET, cruzamientos, zonas de separación de sistemas, cambiadores de ancho, zonas neutras, SE, ATI, ATF, PLO, detectores de tensión |
| 7 | Elementos auxiliares (estaciones de viajeros, talleres y depósitos, túneles y viaductos) |
| 8 | Simbología |
| 9 | Formatos y soportes |
| 10–12 | Normativa derogada, disposiciones transitorias y entrada en vigor, normativa de referencia |
| Anejo I | Ejemplo y simbología Madrid-Sevilla |
| Anejo II | Planos |

### 3.3 Reglas generales de representación

- Las vías se designan como **"VIA 1"** (o "via1"/"v1" en estaciones complejas); la numeración se rige por la **NAG 2-0-1.0** y las vías por la Consigna Serie A de cada estación.
- Deben referenciarse con PK los **seccionadores**, edificio de viajeros, túneles y viaductos, PLO, subestaciones, centros de autotransformación intermedios y finales, equipos auxiliares (calefactores, ET, BTS, BTO…), pórticos de seccionadores, cambiadores de ancho/sistema y bocas de túneles.
- Solo se incluyen elementos de infraestructura **obligatorios**: subestación, autotransformadores y edificio de viajeros. Túneles, viaductos, andenes y talleres son optativos.
- Los **elementos de sustentación** (postes, ménsulas, pórticos rígidos) **no se representan**.
- Las **protecciones pasivas** (pararrayos de óxidos metálicos, cable de tierra, pozos/picas de tierra, conexiones equipotenciales) **no se incluyen** en el esquema: no interfieren en la maniobra ni en la explotación.

---

## 4. ESQUEMAS DE ALIMENTACIÓN EN 25 kV (1x25 Y 2x25)

### 4.1 Sistema 1x25 kV

- La **catenaria** se alimenta a **25 kV** en corriente alterna monofásica.
- El **circuito se cierra** a través de los **carriles** y del **cable de retorno**, que a su vez están **conectados a tierra**.
- Para evitar **desequilibrios en la red de distribución**, las **fases se van alternando en cada subestación**. Esto obliga a disponer **zonas neutras** (tramos no alimentados) en los puntos de cambio de fase, para evitar **cortocircuitos en la catenaria al paso del pantógrafo**.
- Es el sistema de la línea de Alta Velocidad **Madrid-Sevilla** (Anejo 1), caracterizado por la **ausencia de feeder negativo y de ATI/ATF**.

### 4.2 Sistema 2x25 kV

- Las subestaciones disponen de **transformadores monofásicos con salida bifásica**, con entrada en alta tensión y salida en **55 kV**.
- El secundario cuenta con **tres terminales**:
  - un terminal a la **catenaria**;
  - otro al **feeder negativo**;
  - la **toma central al carril de retorno**, conectado a tierra.
- Resultan tensiones de **27,5 kV y −27,5 kV** (en oposición de fase) en catenaria y feeder negativo respectivamente, con respecto a tierra. La tensión entre catenaria y feeder negativo es por tanto de **55 kV**.
- La principal diferencia frente a 1x25 kV es la existencia de **autotransformadores** instalados **a intervalos regulares entre subestaciones**, que **reparten la corriente de retorno** de modo que circule en su mayor parte por el **feeder negativo**. Al formar un sistema **bifásico de 55 kV** con la catenaria, se reducen las **pérdidas** y las **interferencias electromagnéticas**.

### 4.3 La catenaria en el esquema

| Elemento | Representación |
|----------|----------------|
| Catenaria de vía general (25 kV) | Color **negro**, línea continua |
| Feeder negativo (−25 kV) | Color **rojo**, línea continua (cable no aislado) |
| Catenaria rígida | Línea continua **más gruesa**; en estaciones, distintos colores |
| Vías sin electrificar | Línea discontinua **gris** |
| Vías electrificadas en 3 kV c.c. | Trazos continuos **naranja** con indicación "3 kV c.c." |
| Vías ajenas a Adif | Trazos continuos **grises**, representación simplificada |
| Instalación en construcción | Símbolo específico de "En construcción" |
| Feeder de continuidad | Línea discontinua **de punto y raya**, con el texto "FEEDER DE CONTINUIDAD" |

La catenaria está formada por los conductores principales del circuito positivo: **sustentador, hilo de contacto y péndolas**. Los **feeders** son conductores auxiliares con funciones de **alimentación**, **refuerzo de sección** o **retorno**.

### 4.4 Tipos de feeders

| Tipo | Función | Representación |
|------|---------|----------------|
| **Feeder de alimentación positivo** | Alimenta la catenaria desde la SE o centros de autotransformación | Designación SE/ATI/ATF + nº + "C" |
| **Feeder de alimentación negativo** | Alimenta el feeder negativo que discurre paralelo a la vía, suspendido o en cabeza de poste | Designación SE/ATI/ATF + nº + "F" |
| **Feeder negativo (−25 kV)** | Retorno de corriente en 2x25 kV | Color rojo, suspendido o en cabeza mediante cadena de aisladores |
| **Feeder de acompañamiento o refuerzo** | Aumenta la sección del circuito positivo por capacidad de corriente o caída de tensión (típico en 1x25 kV) | **No se representa**: se conecta y desconecta siempre a la vez que la catenaria |
| **Feeder de continuidad** | Puentea un tramo conmutable multitensión separado por seccionamientos de lámina de aire; permite la alimentación en paralelo de subestaciones colaterales (instalación excepcional) | Línea discontinua de punto y raya con texto "FEEDER DE CONTINUIDAD" |

**Patrón de numeración de los feeders de alimentación** (ejemplo con SE 312):

| Designación | Criterio |
|-------------|----------|
| SE 312-C01 / SE 312-F01 | Vía impar, lado de menor PK |
| SE 312-C02 / SE 312-F02 | Vía par, lado de menor PK |
| SE 312-C03 / SE 312-F03 | Vía impar, lado de mayor PK |
| SE 312-C04 / SE 312-F04 | Vía par, lado de mayor PK |

> Nota: en el Anejo 1 (Madrid-Sevilla, 1x25 kV) los feeders se designan con la letra **J** (J7, J8, J17, J18, J4, J9) y un mismo feeder alimenta ambas vías.

---

## 5. SECCIONAMIENTOS, ZONAS NEUTRAS Y SEPARACIÓN DE FASES

### 5.1 Seccionamientos

El **seccionamiento** es el tramo de solape de catenaria que da continuidad mecánica y/o eléctrica al sustentador e hilos de contacto y mantiene estables los esfuerzos mecánicos ante las variaciones de temperatura, permitiendo alimentar a los pantógrafos sin interrupción.

| Tipo | Misión | Representación en esquema |
|------|--------|---------------------------|
| **De cantón** | Independizar mecánicamente dos cantones y permitir la regulación de tensiones con la temperatura; mantiene la **continuidad eléctrica** mediante conexiones fijas | **No se representa** |
| **De lámina de aire** | **Separar eléctricamente** dos tramos de catenaria a la vez que independiza mecánicamente los cantones | Símbolo específico en el esquema |

### 5.2 Aislamientos

- **Aislador de sección:** aparato montado en el hilo de contacto que independiza eléctricamente una vía o grupo de vías de una misma estación dando continuidad mecánica al paso del pantógrafo.
  - **Asimétrico:** el pantógrafo toma contacto con el otro patín antes de perder el primero; los tramos a cada lado quedan **momentáneamente interconectados y a la misma tensión**. Es el **más frecuente**.
  - **Simétrico:** el pantógrafo abandona un patín quedando momentáneamente sin tensión hasta alcanzar el otro; los tramos **no se interconectan**. Es **poco frecuente en 25 kV**.
  - Se numeran **correlativamente de menor a mayor PK**, comenzando una serie por cada estación.
- **Aislador de feeder negativo:** cadena de aisladores en el feeder negativo que **aisla eléctricamente dos tramos**.
- En general, los **aisladores o aislamientos intermedios no se representan**, salvo los aisladores de sección y el aislamiento intermedio del feeder negativo.

### 5.3 Zonas neutras (separación de fases)

- La catenaria en c.a. está **dividida en tramos eléctricos**; para evitar desequilibrios en la red, las **fases se van alternando** en los diferentes tramos.
- La **zona neutra** es una zona **sin tensión**, situada **frente a las subestaciones y a los ATF**, formada por **dos seccionamientos de lámina de aire** suficientemente distanciados para que un tren **no pueda cortocircuitar las distintas fases** al paso del pantógrafo. El tren circula por ella **sin tracción eléctrica**.
- En el esquema puede indicarse la **longitud de la zona neutra** (en metros) en una nota adicional, calculada según el apartado **6.2.4.2.5 de la Instrucción Ferroviaria de Energía**; **no coincide** con la distancia entre seccionadores (diferencia entre los PK de los seccionadores que la delimitan).
- La zona neutra puede estar **desplazada** respecto al pórtico de seccionadores de la SE o ATF, debiéndose tener en cuenta la ubicación de los seccionadores **N1/N2** frente a los **ZNX**.

### 5.4 Zonas de separación de sistemas (3 kV c.c. / 25 kV c.a.)

- Montaje especial de **aisladores de sección y seccionadores** que separa un trayecto alimentado en **corriente continua (3 kV)** de otro en **corriente alterna (25 kV)**.
- Se componen de una **doble zona neutra**, generalmente formada por **4 aisladores de sección asimétricos**, que forman **tres zonas aisladas entre sí y sin tensión**, con el **punto central puesto a tierra**. En espacios reducidos se pueden emplear **aisladores simétricos** (zona de tipo corto, 2 aisladores).
- Si la longitud supera los **8 metros**, se pueden disponer **seccionadores de puenteo** de los aisladores de sección más externos.
- Designación: código de tres letras del tramo + guion + "**ZS**" + número de vía + número correlativo desde el lado de continua hacia el de alterna (**ZS1.1, ZS1.2, ZS2.1, ZS2.2…**).
- Los **cambiadores de ancho** (ibérico 1.668 mm ↔ UIC 1.435 mm) suelen llevar asociada una zona de separación de sistemas, representándose también el edificio del cambiador.

### 5.5 Agujas aéreas, escapes y breteles

- Las **agujas aéreas** permiten el paso de las circulaciones con pantógrafo entre dos catenarias de un desvío, cruzamiento o escape sin discontinuidad en la alimentación. Generalmente disponen de conexiones eléctricas fijas (misma tensión que las catenarias que forman) y se identifican como **puntos de referencia** para detección de averías o trabajos, con numeración equivalente al aparato de vía homólogo y sin símbolo específico.
- Los **escapes y breteles** entre vías generales o vías de distinto subsector eléctrico se aíslan con **aislador de sección** cuando la entrevía lo permite y las condiciones de explotación lo requieran.
- **Puesto de banalización (PBA):** se denomina "PBA" + nombre característico del tramo + PK.
- **PAET:** se denomina "PAET" + nombre característico del tramo + PK.
- **Cruzamientos y saltos de carnero:** en el cruzamiento al mismo nivel se marca el punto de conexión eléctrica; en el salto de carnero se representa el viaducto con línea ligeramente más fina.

---

## 6. ELEMENTOS DE PROTECCIÓN Y CONTROL

### 6.1 El seccionador en la NAE 119

El **seccionador** es el aparato dotado de cuchilla cuya apertura **interrumpe la continuidad eléctrica** entre dos tramos separados por un seccionamiento de lámina de aire, aislador de sección o aislador de feeder negativo, y cuyo cierre **da continuidad al circuito**. Se maniobra:
- **Manual** (palanca o manivela), o
- **Motorizado y generalmente telemandado**.

Reglas de representación:
- Se representan en su **posición normal de funcionamiento**; las posiciones anómalas o provisionales requieren nota.
- **Unipolares:** alimentan un solo circuito (catenaria o feeder negativo −25 kV); trazo del color del circuito. En **1x25 kV siempre son unipolares**.
- **Bipolares:** alimentan simultáneamente catenaria (en negro) y feeder negativo (en rojo); maniobra simultánea de ambos circuitos. En **2x25 kV** pueden instalarse unipolares o bipolares según función.
- Llevan el **PK del apoyo** donde van montados (o del pórtico). Si el seccionador corta una zona alejada, se añade el **PK de la lámina de aire**.

### 6.2 Tipos de seccionadores y nomenclatura normalizada

| Tipo | Posición normal | Nomenclatura | Función |
|------|-----------------|--------------|---------|
| Punta de feeder de catenaria de SE | Cerrado | SE 312-C1 … C4 | Entre el feeder positivo y la catenaria; independiza ambos elementos |
| Punta de feeder negativo de SE | Cerrado | SE 312-F1 … F4 | Entre el feeder negativo y el feeder negativo de la SE; el número sigue al **disyuntor extrarrápido** de la SE |
| Autotransformador intermedio | Cerrado | ATI 312.3-FC1/FC2 (bipolar); ATI XXX.X-CX/FX (unipolar) | Independizar catenaria y feeder negativo del centro de autotransformación |
| Autotransformador final | Cerrado | ATF 302.1-FC1…FC4 | Independizar catenaria y feeder negativo del ATF; se colocan a ambos lados de la zona neutra |
| Zona neutra | Abierto | SE/ATF 302.1-ZN1…ZN4 | Unir eléctricamente la zona neutra con los trayectos, permitiendo su energización en emergencia |
| Puenteo de feeder negativo | Abierto | SE/ATF 302.1-N1/N2 | Independizar paquetes eléctricos del feeder negativo y permitir su puenteo en emergencia |
| Ordinarios de catenaria | Cerrado | XXX-S1 (p. ej. VRU-S1); en 2x25 kV XXX-SC1/SF1 | Independizar tramos de una misma vía o paquetes de vías; ante estaciones, bifurcaciones, cambiadores de ancho, PBA, PAET |
| Pórtico de distribución | — | EST-B1/B2 (a barras), EST-B3… (tramos sin andén), EST-BP12 (puenteo entre barras), EST-BV1/BV17-18 (vías con andén) | Alimentar vías secundarias desde las generales a través de un **embarrado de distribución**; se representa con rectángulo envolvente |
| Puesta en paralelo | — | ARC-P21 (bipolar); XXX-PCXX/PFXX (unipolar) | Conectar dos tramos de catenaria en paralelo |
| Alimentación a vías secundarias | Cerrado | MDC-S13, MDC-S512 | Alimentar una vía secundaria a través de una principal |
| Especiales | Según función | — | Multipolar, condicionado (asociado a detector de tensión), puesta a tierra de emergencia en túnel |
| Servicios auxiliares y externos | Según consumo | XXX-(CT/PIC/PCA/ET/T/BTS/OP/DCC/DCO/DRC/EM/PB)N; CA: XXX-CAN | Alimentar consumidores desde el feeder negativo (o catenaria si no existe) |

**Criterios de numeración destacados:**

- **Ordinarios (XXX-SX):** código de tres letras = nemónico del emplazamiento del **PLO** que los maniobra por telemando (único en cada línea o ámbito; puede coincidir con el nemónico del enclavamiento); el número crece correlativamente en orden de PK creciente, **impar en vías impares y par en vías pares** (ej. VRU-S1, PAET de Villarrubia de Santiago).
- **Puesta en paralelo bipolar (XXX-PXX):** el número de dos cifras indica las vías que conecta, siendo la primera la vía donde se ubica el seccionador (ej. ARC-P21, en la vía 2, conecta vías 1 y 2). En unipolar, primera cifra = vía principal y segunda = vía secundaria alimentada.
- **Vías secundarias (XXX-SXX):** el número comienza con la vía principal seguida de la vía secundaria (ej. MDC-S13, vía 1 alimenta vía 3).
- **ATF (XXX.X-FCX):** 1 = vía impar lado menor PK; 2 = vía par lado menor PK; 3 = vía impar lado mayor PK; 4 = vía par lado mayor PK.
- **Servicios auxiliares:** código de 3 letras + tipo de servicio + número de vía (ej. JBO-ET1, GAR-CT1, MEN-OP2, TIN-DCO2). Cuando un seccionador alimenta varios servicios se separan con guion (JBO-ET1-CT1). En iluminación de túnel se añade **A** (lado menor PK) o **B** (lado mayor PK): TUN-T1A. Los **calentadores de agujas** se designan **XXX-CAN** con N correlativo independiente de la vía (CHA-CA5). La alimentación a **edificios técnicos de señalización** se realiza **en redundancia**, con seccionadores **enclavados** para evitar alimentación simultánea por los dos puntos.

### 6.3 Seccionadores especiales

| Tipo | Característica |
|------|----------------|
| **Multipolar** | Al cierre interconecta un polo de entrada con dos polos de salida (o viceversa); a la apertura mantiene el aislamiento |
| **Condicionado** | Lleva asociado un **detector de tensión** que condiciona su maniobra a la apertura o al cierre |
| **Puesta a tierra de emergencia en túnel** | Mando a distancia; hace **equipotencial** una sección (catenaria, tierra y negativo) condicionando la maniobra a la **ausencia de tensión** y a la correcta verificación de la conexión a negativo, permitiendo la entrada de los servicios de emergencia |

### 6.4 Protecciones y control (síntesis)

| Elemento | Naturaleza | Presencia en el esquema |
|----------|------------|-------------------------|
| **Seccionadores telecontrolados** | Maniobra motorizada gobernada desde un **PLO** conectado al **Sistema de Telemando de Energía** | Se representan con su símbolo; el PLO es de inclusión **obligatoria** (doble rectángulo si está conectado al Telemando; rectángulo simple con "SOLO MANDO LOCAL" si no) |
| **Disyuntores extrarrápidos de las cabinas de SE** | Protección de los feeders; la numeración de los seccionadores de punta de feeder negativo (SE XXX-FX) sigue el número del disyuntor | Se representan en el esquema; su **designación queda fuera del alcance** de la NAE 119 |
| **Pararrayos de óxidos metálicos** | Protección pasiva contra sobretensiones | **No se incluyen** en el esquema |
| **Cable de tierra, pozos/picas de tierra, conexiones equipotenciales** | Protección pasiva | **No se incluyen** en el esquema |
| **Detector de tensión** | Verifica la existencia de tensión en una sección de LAC o feeder; facilita al Telemando la verificación del estado de los seccionadores | Opcional; solo en circunstancias excepcionales (sistemas bi-tensión, seccionadores de puesta a tierra de emergencia en túneles). **No sirve para verificar la ausencia de tensión en un corte de tensión** |

> Nota (Anejo 1, Madrid-Sevilla): la simbología original de esta línea incluye seccionadores con accionamiento remoto controlado y no controlado en intensidades de **1000 A, 1700 A y 2000 A**, seccionadores con/sin contacto de puesta a tierra y accionamiento manual con llave triángulo. Estos elementos se mantienen como referencia para la línea mientras los esquemas no se adapten a la presente NAE.

---

## 7. PUESTA A TIERRA Y RETORNO EN CA

### 7.1 Retorno en 1x25 kV

- El circuito de tracción se cierra por **carriles y cable de retorno**, ambos **conectados a tierra**.
- Al no existir feeder negativo, la corriente de retorno circula por el carril y la tierra. El **feeder de acompañamiento o refuerzo** se emplea cuando la capacidad de corriente o la caída de tensión lo exigen.
- La **alternancia de fases** entre subestaciones hace imprescindibles las **zonas neutras** en los cambios de fase.

### 7.2 Retorno en 2x25 kV

- La **toma central** del secundario del transformador se conecta al **carril de retorno**, que está **conectado a tierra**.
- Los **autotransformadores intermedios (ATI)** se sitúan **a intervalos regulares entre subestaciones** y **reparten la corriente de retorno** para que circule en su mayor parte por el **feeder negativo (−25 kV)**.
- El **autotransformador final (ATF)** se sitúa **al final del tramo eléctrico**; reparte las corrientes de retorno y constituye el **final y el inicio de un nuevo tramo eléctrico**.
- Con el feeder negativo a −25 kV en oposición de fase se forma un sistema **bifásico de 55 kV** frente a la catenaria, reduciéndose **pérdidas e interferencias electromagnéticas**.

### 7.3 Elementos de tierra en el esquema

- El **feeder negativo** discurre suspendido o en cabeza de poste **mediante una cadena de elementos aisladores**, manteniéndolo aislado de tierra.
- El **aislamiento intermedio del feeder negativo** (cadena de aisladores) permite **aislar eléctricamente dos tramos** del feeder, lo que condiciona los **paquetes eléctricos** y los **seccionadores de puenteo N1/N2** en las zonas neutras.
- Los **seccionadores de puesta a tierra de emergencia en túnel** hacen **equipotencial** la catenaria, la tierra y el negativo antes de autorizar el acceso.
- Las **protecciones pasivas** de tierra (cable de tierra, picas, equipotenciales, pararrayos) son elementos que **no se representan** en el esquema eléctrico.

### 7.4 Criterio de diseño del retorno (lógica)

La NAE 119 no fija valores de diseño del retorno (resistencias, distancias entre ATI, secciones); su objetivo es la representación. La lógica de diseño que subyace es:

1. **Minimizar la corriente por carril/tierra** en 2x25 kV mediante ATI espaciados regularmente, reduciendo así la caída de tensión en el retorno y las interferencias.
2. **Garantizar la equipotencialidad** del retorno (carriles, cable de retorno y neutro del transformador a tierra).
3. **Segmentar** el feeder negativo en paquetes eléctricos separables en zona neutra (seccionadores N1/N2) para poder aislar tramos en trabajos sin desalimentar líneas completas.
4. **Verificar la ausencia de tensión** mediante los procedimientos de corte de tensión, nunca mediante detectores de tensión del esquema.

---

## 8. CRITERIOS DE DISEÑO Y RELACIÓN CON NAE 112 (CC), NAE 300/301/302 Y ET SSEE 25 KV

### 8.1 La NAE 119 en el marco normativo de energía

La NAE 119 es el documento **de representación** del sistema de 25 kV c.a.; convive con el resto del corpus normativo de energía de Adif:

| Documento | Papel frente a la NAE 119 |
|-----------|---------------------------|
| **NAE 112** (Esquemas eléctricos de LAC en c.c., 3ª ed. feb. 2022 + M1 ene. 2023) | Norma **hermana** para corriente continua; la NAE 119 se apoya en ella y está citada en su bibliografía. Aplica la misma lógica de esquemas unifilares, pero en 3 kV/1,5 kV c.c. con sus seccionamientos y zonas de separación |
| **NAE 300 / 301 / 302** (catenaria de c.a.) | Definen el **sistema de LAC en sí** (parámetros, materiales, montaje). La NAE 119 no las cita explícitamente, pero el sistema eléctrico que representa (catenaria, sustentador, péndolas, seccionamientos, aisladores) es el que diseñan estas normas |
| **ET de subestaciones 25 kV** | Dimensionan y especifican las **SE y sus cabinas** (transformadores, disyuntores extrarrápidos). La NAE 119 **representa** solo las salidas de feeder positivo y negativo de la SE en el esquema, dejando la designación de los elementos de cabina **fuera de su alcance** |
| **ADIF-PE-301-001-006-SC-521** (Cortes de tensión) | Es el **motivo de ser** de la NAE 119: el esquema eléctrico actualizado es imprescindible para que el Responsable del Corte identifique los elementos a maniobrar |
| **NAG 2-0-1.0** y Consignas Serie A | Rigen la **numeración de vías** usada en el esquema |
| **UNE-EN 50163** | Fija la **tensión permanente máxima** (27,5 kV) aplicable al sistema de 25 kV c.a. |

### 8.2 Criterios de diseño que debe soportar el esquema

Sin atribuir valores a la NAE 119, la coherencia del esquema exige que el diseñador verifique:

- **Continuidad de alimentación:** cada tramo eléctrico debe poder aislarse (seccionadores ordinarios, láminas de aire) y alimentarse desde más de un origen cuando la explotación lo exija (puestas en paralelo, feeder de continuidad).
- **Seguridad en maniobra:** posición normal abierta en elementos de emergencia (ZN, N1/N2) y cerrada en elementos de explotación normal (punta de feeder, ATI/ATF, ordinarios).
- **Compatibilidad de sistemas:** las **zonas de separación de sistemas** (doble zona neutra, punto central a tierra) y las **zonas neutras de cambio de fase** deben situarse donde un pantógrafo no pueda cortocircuitar fases distintas.
- **Redundancia de servicios críticos:** alimentación duplicada y enclavamiento para edificios técnicos de señalización.
- **Excepciones documentadas:** las instalaciones de gran criticidad (túneles con catenaria rígida, saltos de carnero, cambiadores de ancho) se representan con símbolos específicos y se referencian con PK para facilitar el corte de tensión.

### 8.3 Formatos y control documental

- Los esquemas se trazan en **CAD compatible con DWG** y se publican en **PDF**; tamaños **A4 y A3**; varias hojas **solapadas** sin pérdida de información.
- **Verificación previa a la publicación:** legibilidad en papel y pantalla; colores aptos también para impresión en **blanco y negro**.
- **Cajetín obligatorio:** Subdirección de Operaciones y Jefatura responsable del mantenimiento; delineante; responsable de electrificación que aprueba (con firma); fecha de aprobación en formato **DD-MM-AAAA**; número de versión; número de plano y total de hojas; título con "**L.A.C**", nombre de la línea y "**ESQUEMA ELÉCTRICO**".
- **Transitoriedad:** la norma no deroga ningún documento y entró en vigor en su fecha de aprobación (Comité de Normativa, 18 de junio de 2025).

---

## 9. AUTOEVALUACIÓN (10 preguntas)

**1.** ¿Cuáles son los dos sistemas de electrificación en corriente alterna a 25 kV que coexisten en la red de Adif y en qué se diferencian?

**2.** ¿Qué tensión existe entre la catenaria y el feeder negativo en el sistema 2x25 kV, y qué tensión tienen cada uno respecto a tierra?

**3.** ¿Por qué es necesario instalar zonas neutras en los puntos de cambio de fase?

**4.** ¿Cuál es la diferencia funcional entre un seccionamiento de cantón y un seccionamiento de lámina de aire, y cuál de ellos se representa en el esquema?

**5.** ¿Qué posición normal (abierto/cerrado) tienen los seccionadores de zona neutra (SE/ATF-ZNX) y los de puenteo de feeder negativo (SE/ATF-NX)?

**6.** ¿Qué seccionadores se emplean siempre unipolares en 1x25 kV y qué representa el color rojo frente al negro en un seccionador bipolar?

**7.** ¿Cómo se designa un seccionador ordinario de catenaria y qué significan el código de tres letras y la paridad del número?

**8.** ¿Qué es una zona de separación de sistemas, de qué elementos se compone en su tipo largo y cuándo se permiten seccionadores de puenteo?

**9.** ¿Por qué los pararrayos, el cable de tierra y las picas no se representan en el esquema eléctrico?

**10.** ¿Qué información debe contener el cajetín de un esquema eléctrico publicado según la NAE 119?

### Soluciones (respuestas cortas)

1. El **1x25 kV** (catenaria a 25 kV, retorno por carriles y cable de retorno a tierra, sin feeder negativo ni autotransformadores) y el **2x25 kV** (transformador monofásico de salida bifásica de 55 kV, feeder negativo a −25 kV y autotransformadores intermedios y finales que reparten la corriente de retorno).
2. Cada conductor está a **27,5 kV** respecto a tierra, en **oposición de fase**, resultando **55 kV** entre catenaria y feeder negativo.
3. Para evitar **desequilibrios en la red de distribución**, las fases se alternan en cada subestación; las zonas neutras impiden que el pantógrafo **cortocircuite las distintas fases** en el punto de cambio.
4. El **de cantón** solo independiza mecánicamente y **mantiene la continuidad eléctrica** (no se representa); el **de lámina de aire** **separa eléctricamente** dos tramos y **se representa** con símbolo propio.
5. Ambos en **posición normal abierta**: los ZNX permiten energizar la zona neutra en emergencia y los NX permiten el puenteo del feeder negativo en emergencia.
6. En **1x25 kV siempre son unipolares** (no existe feeder negativo). En un bipolar, la **cuchilla negra** corresponde al lado de catenaria (25 kV) y la **roja** al feeder negativo (−25 kV), maniobrando ambos circuitos simultáneamente.
7. Con el patrón **XXX-SX** (ej. VRU-S1): el código de tres letras es el nemónico del **PLO** que los maniobra por telemando; el número es **impar en vías impares y par en vías pares**, creciendo en orden de PK.
8. Es un montaje de aisladores de sección y seccionadores que separa un tramo en **3 kV c.c.** de otro en **25 kV c.a.**; en su tipo largo usa **4 aisladores de sección asimétricos** formando tres zonas sin tensión con el **punto central puesto a tierra**. Si su longitud es **superior a 8 m**, se pueden disponer seccionadores de puenteo de los aisladores externos.
9. Son **protecciones pasivas** que no interfieren en la explotación ni en la maniobra del sistema, por lo que la NAE 119 excluye su representación del esquema.
10. Subdirección de Operaciones y Jefatura responsable; delineante; responsable de electrificación que aprueba (nombre y firma); fecha de aprobación (DD-MM-AAAA); versión; número de plano y total de hojas; título con "L.A.C", línea y "ESQUEMA ELÉCTRICO".

---

## 10. REFERENCIAS

| Referencia | Título | Contenido integrado |
|------------|--------|---------------------|
| NAE 119, 1ª ed. (jun. 2025) | Esquemas eléctricos de línea aérea de contacto en 25 kV C.A. | Toda la lección |
| ADIF-PE-301-001-006-SC-521, Rev. 1 (may. 2020) | Cortes de tensión en líneas aéreas de contacto alimentadas en 25 kV c.a., 3 kV c.c. y 1,5 kV c.c. | Antecedentes y objeto (sección 2) |
| NAE 112, 3ª ed. (feb. 2022) + M1 (ene. 2023) | Esquemas eléctricos de LAC en corriente continua | Marco normativo y relación (sección 8) |
| NAG 2-0-1.0 (jul. 2016 + erratum ene. 2017) | Designación de vías y componentes de la superestructura | Numeración de vías (sección 3) |
| UNE-EN 50163 | Tensiones de alimentación de los sistemas de tracción | Tensión máxima permanente 27,5 kV (secciones 2 y 4) |
| Instrucción Ferroviaria de Energía (apdo. 6.2.4.2.5) | Longitud de zonas neutras | Cálculo de longitud de ZN (sección 5) |
| Anejo 1 NAE 119 | Ejemplo y simbología Madrid-Sevilla | Sistema 1x25 kV, feeders J, seccionadores A/6/I y simbología original (secciones 4, 6) |
| Anejo 2 NAE 119 | Planos | Formatos y cajetín (sección 8) |

---

*Lección 6 del Módulo 5 — Sistemas de Tracción. Base normativa: NAE 119, 1ª edición, junio 2025.*
