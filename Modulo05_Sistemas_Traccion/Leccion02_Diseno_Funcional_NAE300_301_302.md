# MÓDULO 5 · LECCIÓN 2
# DISEÑO FUNCIONAL DE CATENARIAS DE 3 kV: CA-160, CA-220, CA-160H y CA-200H

## NAE 300 · NAE 301 · NAE 302 — Las normas de diseño funcional de Adif

> **Documentos base:**
> - **NAE 300**, «Diseño funcional de la LAC tipo CA-160/3 kV. Parte 1: Memoria y
>   anejos I a IV», 2ª edición, junio 2024, 55 págs. (Partes 2.1 a 2.3, 3, 4 y 5).
> - **NAE 301**, «Diseño funcional de la LAC tipo CA-220/3 kV. Parte 1: Memoria y
>   anejos I a IV», 2ª edición, junio 2024, 56 págs.
> - **NAE 302**, «Diseño funcional de la LAC tipo CA-160H y CA-200H. Parte 1:
>   Memoria y anejos I a IV», 2ª edición, diciembre 2024, 85 págs.

---

## 1. RESULTADO DE APRENDIZAJE

Al terminar esta lección serás capaz de:

1. Entender la **arquitectura de la normativa de diseño**: NAE 107 define los parámetros,
   NAE 300/301/302 los **materializan por tipología de catenaria**
2. Fijar la **composición de conductores y tenses** de las cuatro familias de 3 kV
   (CA-160/3kV A y B, CA-220/3kV, CA-160H/3kV, CA-200H/3kV)
3. Dimensionar **vano, descentramiento, cantón de compensación y flecha** según el radio
   de vía y las condiciones de viento
4. Proyectar **seccionamientos de cantón y de lámina de aire**, y seleccionar **agujas
   aéreas** según el aparato de vía
5. Seleccionar **postes, macizos, ménsulas y brazos de atirantado** de catálogo
6. Diseñar **alimentación, retorno, pararrayos, tomas de tierra y protecciones avifauna**

---

## 2. RESUMEN EJECUTIVO

Mientras que la NAE 107 es el **diccionario** (qué es cada parámetro y cuánto vale),
las **NAE 300/301/302 son la guía de construcción**: definen, para **cada tipología de
catenaria**, la composición exacta de conductores, los tenses de montaje, los vanos
máximos según radio, las configuraciones de seccionamiento y aguja, los postes y
macizos, y las conexiones de alimentación y retorno.

Cada norma cubre **una familia de catenaria de 3 kV c.c.**, que es el sistema
histórico de la red convencional de Adif:

| Norma | Familia | Vmáx (km/h) | Sustentador | Hilos de contacto | Papel en la red |
|-------|---------|-------------|-------------|-------------------|-----------------|
| **NAE 300** | CA-160/3kV (Tipo A y B) | 160 | 150 mm² Cu ETP | 2×107 ó 2×120 mm² | Red convencional básica |
| **NAE 301** | CA-220/3kV | 200 | 185 mm² Cu ETP | 2×150 mm² CuAg0,1 | Líneas de mayor capacidad |
| **NAE 302** | CA-160H / CA-200H (híbridas) | 160 / 200 | 150 mm² Cu ETP | 2×120 mm² CuAg0,1 | **Transformables a 25 kV** |

> **Regla de oro:** las catenarias **híbridas (NAE 302)** se diseñan ya para 25 kV:
> los conductores no cambian al transformar; solo el aislamiento, las distancias y el
> feeder. Esto las convierte en la opción preferente cuando se prevé un futuro cambio
> de sistema (CA-160H/25kV y CA-200H/25kV).

> **Regla de composición:** una catenaria de 3 kV lleva **siempre dos hilos de
> contacto** (2×BC) y un sustentador de cobre. La CA-220 se distingue por sus
> secciones mayores (185 y 2×150 mm²) que le dan más capacidad de corriente.

---

## 3. NAE 300 — CA-160/3kV (Tipo A y Tipo B)

### 3.1. Composición de las catenarias (4.2.1) — Tabla 4

| Elemento | CA-160/3kV TIPO A | CA-160/3kV TIPO B |
|----------|-------------------|-------------------|
| **Sustentador** | 150 mm² Cu ETP · **1425 kgf (1397 daN)** | 150 mm² Cu ETP · **1425 kgf (1397 daN)** |
| **Hilos de contacto** | 2× BC-107 Cu ETP · **2×1050 kgf (1029 daN)** | 2× BC-120 CuAg0,1 · **2×1200 kgf (1177 daN)** |
| **Péndolas** | 25 mm² Cu flexible | 25 mm² Cu flexible |
| **Feeder de refuerzo** | Variable (según estudio eléctrico) | Variable |

- Generalmente **no hace falta feeder de refuerzo**, salvo rampas excesivas o gran
  distancia entre subestaciones.
- **No admite** configuraciones con un solo hilo de contacto ni sustentador de acero
  de 72 mm² (variantes históricas que solo se usan como referencia de mantenimiento).

### 3.2. Características geométricas y mecánicas (4.2.2)

**Altura de los hilos (Tabla 5):** nominal **5300 mm**, máxima **6000 mm**, mínima de
diseño según IFE 4.1.2.2.1.4 (depende del gálibo y de la altitud — tablas 6 y 7 con
GHE16, GEB16/GB, AF4.0/4.1, AF4.2, GEC16/GC).

**Temperatura de los conductores (Tabla 3):**

| Conductor | Máx. permanente | Máx. 30 min (pantógrafo en reposo) |
|-----------|-----------------|-------------------------------------|
| Sustentador Cu ETP | 80 ºC | — |
| Hilos Cu ETP | 80 ºC | 120 ºC |
| Hilos CuAg0,1 | 100 ºC | 150 ºC |

**Viento:** estructural **120 km/h (33,3 m/s)**; funcional (desviación del hilo) según
el mapa del Anejo I: **26 / 27 / 29 m/s** (retorno 10 años).

**Descentramiento (Tabla 10):**

| Situación | Descentramiento |
|-----------|-----------------|
| Recta y curva R ≥ 3100 m (Tipo A) / R ≥ 2650 m (Tipo B) | **+20 cm / −20 cm** |
| Curva (interior del arco) | **+20 cm / +20 cm** (hacia el exterior) |

> Criterio de signos: (+) hacia fuera del poste/pendolón; (−) hacia dentro. En
> estaciones en pórtico funicular o túnel con catenaria rígida, (+) hacia la derecha
> de la kilometración.

**Vano máximo (Tablas 11 y 12):**

| Altura de sistema | Vano máximo |
|-------------------|-------------|
| 1400 mm | 60 m |
| 853 mm | 45 m |
| 462 mm | 30 m |
| 263 mm | 20 m |

| Vano | CA-160 Tipo A (radio) | CA-160 Tipo B (radio) |
|------|----------------------|-----------------------|
| 60 m | Recta y R ≥ 3100 | Recta y R ≥ 2650 |
| 60 m | 3100 > R ≥ 1300 | 2650 > R ≥ 1150 |
| 55 m | 1300 > R ≥ 900 | 1150 > R ≥ 850 |
| 50 m | 900 > R ≥ 650 | 850 > R ≥ 625 |
| 45 m | 650 > R ≥ 500 | 625 > R ≥ 470 |
| 40 m | 500 > R ≥ 350 | 470 > R ≥ 340 |
| 35 m | 350 > R ≥ 250 | 340 > R ≥ 250 |
| 30 m | 250 > R ≥ 175 | 250 > R ≥ 210 |
| 25 m | 175 > R ≥ 150 | 210 > R ≥ 175 |

> Hipótesis: viento 29 m/s, nivel del mar, 5 ºC, pantógrafo 1950 mm, categoría de
> terreno 2. Con alturas de sistema < 1400 mm, la péndola equipotencial mínima será
> de 250 mm.

**Diferencia de vanos consecutivos (Tabla 13):** trayecto **10 m** · agujas **5 m** ·
seccionamientos **1 m** (se replantean simétricos, tol. ±1 m en vanos de elevación).

**Cantón de compensación (4.2.2.6, Tabla 14):**

| Longitud media de vanos en curva | Nº máx. de vanos por cantón |
|----------------------------------|-----------------------------|
| 50 < L ≤ 60 | 20 |
| 45 < L ≤ 50 | 22 |
| 35 < L ≤ 45 | 24 |
| 30 < L ≤ 35 | 26 |
| 25 < L ≤ 30 | 28 |
| L ≤ 25 | 30 |

- Recta: **1200 m máx.** (= 20 vanos de 60 m). En curva, según la tabla anterior.
- Cantones ≤ 600 m: compensación en un solo extremo (sentido de la circulación),
  ampliable excepcionalmente a 700 m justificando el rango de regulación.
- Punto fijo en la mitad; latiguillos de punto fijo si la diferencia de semicantones
  > 20 % (a ambos lados) o si la rasante > 5 ‰ (solo en el lado más bajo).

**Flecha de los hilos (Tabla 15):** **0,6 ‰** → flecha (mm) = 0,6·L/1000; con vano de
60 m → máx. **36 mm**.

**Gálibo de postes (Tabla 16):**

| Situación | Distancia poste–carril | Tolerancia |
|-----------|------------------------|------------|
| Recta o exterior de curva | 1,90 m | +20 / −20 cm |
| Interior de curva R > 300 m | 1,90 m | +20 / −10 cm |
| Interior de curva R < 300 m | 2,10 m | +20 / −10 cm |

**Postes en entrevías (Tabla 17):**

| Distancia entre ejes de vías | Tipo de postes |
|------------------------------|----------------|
| D ≥ 6,00 m | Cualquiera |
| 6,00 > D ≥ 5,70 m | X y PG1 |
| 5,70 > D ≥ 5,20 m | Solo PG1 |

En andenes: gálibo de **5 m** (si el andén lo permite).

**Seccionamientos (Tabla 18):** Lámina de Aire **300 mm** (mínimo) · Cantón **250 mm**
(reducible a 200 mm). Elevación mínima de semieje: **250 mm**. Seccionamientos de
**3 vanos** (sin eje) o **4 vanos** (con eje); 5+ vanos solo si vanos < 25 m o R < 300 m.

**Agujas aéreas (Tabla 23):**

| Situación | Tipo de aguja |
|-----------|---------------|
| Vía general + vía desviada / escape / secundaria | Tangencial P-90 · Cruzada P-50 |
| Vía secundaria + vía secundaria | Cruzada P-50 |

Preferencia en vías generales: **tangencial P-90** (referencia NAE 115).

**Tensiones de regulación (Tablas 25 y 26):** tolerancia del tense y peso ± 5 %.

| Elemento | Tipo A | Tipo B |
|----------|--------|--------|
| Sustentador 150 mm² | 1425 kgf · razón 1:5 (285 kg) / 1:3 (475 kg) | ídem |
| Hilos 2× | 2×1050 kgf · 1:5 (420 kg) | 2×1200 kgf · 1:5 (480 kg) |

> Tense real = peso contrapeso × razón de poleas × rendimiento (0,95).

### 3.3. Parámetros dinámicos (4.2.3)

| Parámetro | Tipo A | Tipo B |
|-----------|--------|--------|
| **S0** (elevación en brazo de atirantado, 2 pantógrafos) | 67 mm | 61 mm |
| **fs** a Vmáx / V=0 (elevación en vano) | 98 / 85 mm | 89 / 80 mm |

> Espacio libre de elevación de los brazos: **150 mm**, verificándose 2·S0 < 150 mm.

### 3.4. Criterios de aislamiento (4.2.4)

**3 kV:** estática **150 mm** · dinámica **50 mm** (fase–tierra).

**Aisladores de 3 kV:**

| Parámetro | Riesgo bajo/moderado | Riesgo elevado |
|-----------|----------------------|----------------|
| Línea de fuga | ≥ 300 mm | ≥ 400 mm |
| Impulso rayo en seco | 95 kV | 120 kV |
| Frecuencia industrial bajo lluvia | 38 kV | 38 kV |

### 3.5. Componentes y alimentación

- **Postes (Tabla 32):** vía general **X2B / X2BA**; anclaje de seccionamiento **Z1**;
  semieje, eje y aguja **X3 / X3A**.
- **Macizos (Tabla 52):** Z1 ALG 8.463 daN·m; Z2 9.882; Z3 11.454; Z4 13.073;
  Z5 15.018; Z5bis 23.798; Z6bis 33.053; Z6E 30.293 daN·m.
- **Alimentación en estación con subestación:** feeder por vía general con **2 cables
  de Cu 235 mm²** o **2 de LA-380 (337-AL1/44-ST1A)**, conectado por seccionador.
- **Alimentación en trayecto:** feeders desde la subestación; conexión feeder→sustentador
  cada ~**300 m** con 2× Cu flexible 95 mm².
- **Retorno (Tabla 49):** cables aislados 0,6/1 kV de 150/185/235/300 mm²; conexión
  entre vías **1100 mm²**; al pozo de negativos **1100 mm²** (1×6000 kW) o
  **2200 mm²** (2×6000 kW, con simultaneidad −20 %). La sección del retorno será ≥ a
  la suma de los feeders de acometida.
- **Pararrayos:** ≥ 1 por vía cada **2 cantones (~2,5 km)**; en zonas de especial
  incidencia, **1 por cantón y vía**, junto a puntos fijos (ET 03.364.156.4).
- **Cable de tierra:** LA-110 (94-AL1/22-ST1A) o L-110 (117-AL1); bajada a toma de
  tierra **cada 3 km** como máximo; **2 bajadas por cantón** en zonas especiales.
- **Toma de tierra:** **10 Ω** (mín. 6 picas; geometría en estrella si falta espacio);
  según incidencia de rayos y presencia de pica en el macizo (Tabla 50).
- **Protecciones:** viseras UNE-EN 50122-1 pto. 5.3 en pasos superiores; DLT tipo
  **VLD-F** en marquesinas; protección antiescalada y señales en postes de andenes.
- **Avifauna:** NAE 121 apdo. 7.1 (proyecto) y 7.2 (explotación); el conjunto de
  suspensión del feeder con **aislador suspendido (Ct17)** es el diseño más seguro.

---

## 4. NAE 301 — CA-220/3kV

### 4.1. Composición (4.2.1) — Tabla 4

| Elemento | Valor |
|----------|-------|
| **Sustentador** | 185 mm² Cu ETP · **2475 kgf (2428 daN)** |
| **Hilos de contacto** | 2× BC-150 CuAg0,1 · **2×1875 kgf (1839 daN)** |
| **Péndolas** | 25 mm² Cu flexible |
| **Feeder de refuerzo** | Generalmente necesario (según estudio eléctrico) |

> No admite tenses reducidos. Las variantes históricas de 3 kV sirven solo de
> referencia para mantenimiento. Temperatura: sustentador 80 ºC; hilos 100 ºC
> (150 ºC a 30 min).

### 4.2. Características geométricas y mecánicas (4.2.2)

**Altura de los hilos (Tabla 5):** nominal **5300 mm**, máxima **6000 mm**, mínima según
UNE-EN 50119 (tablas 6 a 9 por gálibo, altitud y cielo abierto/túnel). Pendiente
**±1 ‰**, variación **±0,5 ‰** a 220 km/h (IFE 4.1.2.2.1.3 para menores velocidades).
Altura de sistema **1400 mm**; tubo estabilizador **350–450 mm** (elevación ≥ 120 mm).

**Vano máximo (Tablas 12 y 13) — hipótesis 29 m/s, 0 m, 5 ºC, 961,04 N/m²:**

| Vano | CA-220/3kV (radio) | CA-220/3kV aislada 25 kV (radio) |
|------|--------------------|----------------------------------|
| 60 m | R ≥ 1700 | R ≥ 4000 |
| 60 m | 1700 > R ≥ 1100 | 4000 > R ≥ 1400 |
| 55 m | 1100 > R ≥ 950 | 1400 > R ≥ 1050 |
| 50 m | 950 > R ≥ 700 | 1050 > R ≥ 800 |
| 45 m | 700 > R ≥ 550 | 800 > R ≥ 600 |
| 40 m | 550 > R ≥ 400 | 600 > R ≥ 450 |
| 35 m | 400 > R ≥ 350 | 450 > R ≥ 350 |
| 30 m | 350 > R ≥ 300 | 350 > R ≥ 300 |
| 25 m | 300 > R ≥ 250 | 300 > R ≥ 250 |

> Si hay plan de transformación a 25 kV, se usan los valores de la segunda columna
> (compatibilidad con pantógrafo de 1600 mm).

**Descentramiento (Tablas 14 y 15):**

| Catenaria | R ≥ umbral | R < umbral |
|-----------|------------|------------|
| CA-220/3kV (umbral R=1700 m) | +20 / −20 cm | +20 / +20 cm |
| CA-220/3kV aislada 25 kV (umbral R=4000 m) | +20 / −20 cm | +20 / +20 cm |

**Diferencia de vanos consecutivos (Tabla 16):** trayecto 10 m · agujas 5 m ·
seccionamientos 1 m (simétricos).

**Cantón de compensación (Tabla 17):** recta **1200 m** (20 vanos de 60 m); en curva
igual tabla de vanos por cantón que la CA-160; cantones ≤ 600 m con compensación en un
solo extremo (hasta 700 m excepcional). Punto fijo central, con latiguillos en los
mismos casos que NAE 300.

**Flecha (Tabla 18):** **0,5 ‰** → flecha (mm) = 0,5·L/1000; vano 60 m → **30 mm**.

**Gálibo de postes (CA-220 aislada 25 kV):** distancia cara del poste–carril
**2,15 m ± 0,2 m** (≈ 3,2 m entre ejes en ancho ibérico); reducible a **1,90 ± 0,2 m**
con ménsulas especiales calculadas ad hoc.

**Seccionamientos (Tabla 19):** Lámina de Aire **400 mm** (reducible a 300 mm en 3 kV) ·
Cantón **250 mm** (reducible a 200 mm). Elevación de semieje ≥ **250 mm**; 3 vanos solo
en recta con vano ≥ **56 m** (evitar efecto tijera); 4 vanos en general; 5+ vanos si
vanos < 28 m o R < 450 m. Vanos máximos en seccionamiento: cantón 60 m (todos los
vientos); lámina de aire 50/53/55 m según viento 29/27/26 m/s (variante 25 kV).

**Agujas aéreas (Tabla 26):**

| Situación | Tipo de aguja |
|-----------|---------------|
| Vía general ≥ 200 km/h + vía desviada/escape | Tangencial P-90 |
| Vía general ≤ 160 km/h + vía desviada/escape | Tangencial P-90 · Cruzada P-50 |
| Vía general + vía secundaria | Tangencial P-90 · Cruzada P-50 |
| Vía secundaria + vía secundaria | Cruzada P-50 |

**Tensiones de regulación (Tablas 28 y 29):** tolerancia ± 5 %.

| Elemento | Tense | Razón 1:5 | Razón 1:3 |
|----------|-------|-----------|-----------|
| Sustentador 185 mm² | 2475 kgf (2428 daN) | 495 kg | 825 kg |
| Hilos 2×150 mm² | 2×1875 kgf (1839 daN) | 750 kg | — |

### 4.3. Parámetros dinámicos y aislamiento (4.2.3–4.2.4)

| Parámetro | CA-220/3kV | CA-220/3kV (aislada 25 kV) |
|-----------|------------|----------------------------|
| **S0** | 41 mm | — |
| **fs** Vmáx / V=0 | 42 / 30 mm | — |
| Aislamiento estático | 150 mm | 270 mm |
| Aislamiento dinámico | 50 mm | 150 mm |

**Aisladores (Tabla 33):**

| Parámetro | 3 kV | 3 kV riesgo elevado | 25 kV |
|-----------|------|---------------------|-------|
| Línea de fuga | ≥ 300 mm | ≥ 400 mm | ≥ 1200 mm (PD4A, grupo II) |
| Impulso rayo en seco | 90 kV | 120 kV | 200 kV |
| Frecuencia industrial bajo lluvia | 38 kV | 38 kV | 95 kV |

> Excepcionalmente se admiten aisladores de 900 mm de fuga, solo en zonas no
> contaminadas y fuera de túnel.

### 4.4. Componentes (4.3)

- **Postes de vía general (Tabla 34):** XR2 (1 ménsula), XR3 (1 ménsula + feeder en
  estaciones con subestación), XR4 (doble ménsula), XR4E (doble ménsula + seccionador
  / anclaje), XR5 (triple ménsula), Z2 / Z2A (anclaje).
- **Postes de anclaje (Tabla 35):** Z5bis, Z6 (anclaje vías generales), XGA (anclaje
  sin tirante).
- **Postes de estación (Tabla 36):** Z1 (anclaje + doble ménsula + compensación
  independiente, altura < 1,40 m), Z2 (doble ménsula < 1,40 m), Z2A (doble ménsula
  ≥ 1,40 m), Z3 (tres ménsulas, agujas), L y R (pórticos tipo B y C).
- **Entrevías (Tabla 37):** D ≥ 6,00 cualquier poste; 6,00 > D ≥ 5,70 X y PG1;
  5,70 > D ≥ 5,20 solo PG1.
- **Ménsulas (Tablas 38–39):** cuerpos CCM T11A–T11D (Ø 60,3 mm, espesor 3,2/8,2/10,2/
  12,2 mm); tirantes CTT (tracción) o CCM (compresión).
- **Tubos estabilizadores (Tablas 40–41):** TEA1–TEA4 y CSA tipo A–D (Ø 42,4 mm,
  espesor 2,6/4,0/7,1/8,8 mm).
- **Brazos de atirantado (Tablas 45–48):** recta B150/B151/B152 (L 1000/900/1150 mm);
  curva B160/B161/B162; seccionamiento B170 (compensación, 1450), B171 (eje, 1300),
  B172 (lámina de aire, 1400); aguja tangencial B180 (P-90, 1650 mm).
- **Péndolas:** equipotenciales por parejas Co6 (≥ 25 cm); Co7 de varilla en túneles
  (< 25 cm). Cálculo según NAE 116 (Anejo II de la norma).

### 4.5. Alimentación, retorno y protecciones (4.4–4.6)

Idénticos criterios generales que en NAE 300, con las particularidades:

- **Conexiones en seccionamientos de compensación:** conjuntos **CCAS** con 2× Cu
  flexible 150 mm².
- **Conexión de aguja:** conjunto **Ct8-4** en el vano de elevación.
- **Pararrayos:** 1 cada 2 cantones (~2,5 km); 1 por cantón en zonas de especial
  impacto. Conexión a cable de tierra con grapa **G41**; postes/herrajes con grapas
  **G36/G39**.
- **Avifauna (Tabla 51):** sustituir Ct12-1/Ct13-1/Ct14-1 por **Ct17** (aislador
  suspendido) en zonas de riesgo.

### 4.6. Anejos de diseño de la CA-220 (datos de referencia)

**Anejo II — Distribución de péndolas por parejas (CA-220, vías generales):**
pendolado equipotencial por parejas (interior del par 0,50 m). La 1ª péndola a
~5,0–5,4 m del apoyo. La distancia entre parejas se ajusta con el vano. Extracto
(la tabla completa va de 60 a 20 m, en pasos de 0,5 m):

| Vano (m) | Nº péndolas | Nº parejas | 1ª péndola (m) | Interior par (m) | Entre parejas (m) |
|----------|-------------|------------|----------------|------------------|-------------------|
| 60,00 | 16 | 8 | 5,25 | 0,50 | 6,50 |
| 55,00 | 16 | 8 | 5,20 | 0,50 | 5,80 |
| 54,00 | 14 | 7 | 5,15 | 0,50 | 6,70 |
| 50,00 | 14 | 7 | 5,25 | 0,50 | 6,00 |
| 47,50 | 14 | 7 | 5,20 | 0,50 | 5,60 |
| 47,00 | 12 | 6 | 5,25 | 0,50 | 6,70 |
| 42,00 | 12 | 6 | 5,25 | 0,50 | 5,70 |
| 40,00 | 12 | 6 | 5,25 | 0,50 | 5,30 |
| 39,50 | 10 | 5 | 5,30 | 0,50 | 6,60 |
| 38,00 | 10 | 5 | 5,15 | 0,50 | 6,30 |
| 35,00 | 10 | 5 | 5,25 | 0,50 | 5,50 |
| 33,00 | 10 | 5 | 5,25 | 0,50 | 5,00 |
| 32,50 | 8 | 4 | 5,20 | 0,50 | 6,70 |
| 30,00 | 8 | 4 | 5,15 | 0,50 | 5,90 |
| 28,00 | 8 | 4 | 5,20 | 0,50 | 5,20 |
| 26,00 | 8 | 4 | 5,10 | 0,50 | 4,60 |
| 25,00 | 6 | 3 | 5,25 | 0,50 | 6,50 |
| 23,00 | 6 | 3 | 5,15 | 0,50 | 5,60 |
| 21,00 | 6 | 3 | 4,85 | 0,50 | 4,90 |
| 20,00 | 6 | 3 | 4,75 | 0,50 | 4,50 |

> El cálculo del pendolado se realiza según **NAE 116**; esta tabla es la referencia
> ya calculada para la CA-220/3kV en vías generales. Para alturas de sistema < 1400 mm
> la péndola equipotencial mínima será de **250 mm** (Co7 de varilla en túneles).

**Anejo III — Selección de cimentaciones (CA-220):**
calculadas para terreno tipo: **C₀ = 6 daN/m³, H = 12 m, γt = 1400 daN/m³,
tanα = 0,005, σlat = 1 daN/cm²** (dimensiones en NAE 106). Columna **M+** = vuelco
hacia la vía (habitual); **M−** = vuelco al lado contrario.

| Poste | MLS (daN·m) | H poste (m) | Desmonte rect/circ | Terraplén M+ / M− / circ | Armadura | Esperas Ø |
|-------|-------------|-------------|--------------------|--------------------------|----------|-----------|
| XR2 | 6.829 | 7,74 | d5 / Cd1 | t8 / t9 / Ct1 | ARM-2 | 25 |
| XR3 | 8.074 | 7,74 | d6 / Cd2 | t9 / t10 / Ct2 | ARM-2 | 25 |
| XR4 | 9.420 | 7,74 | d8 / Cd2 | t10 / t11 / Ct3 | ARM-2 | 25 |
| XR4E | 8.528 | 8,55 | d7 / Cd2 | t9 / t10 / Ct2 | ARM-2 | 25 |
| XR5 | 10.911 | 7,74 | d8 / Cd4 | t11 / t12 / Ct3 | ARM-2 | 25 |
| Z1 | 7.590 | 8,75 | d6 / Cd1 | t8 / t9 / Ct2 | ARM-2 | 25 |
| Z2 | 8.858 | 8,75 | d7 / Cd2 | t9 / t10 / Ct2 | ARM-2 | 25 |
| Z3 | 10.263 | 8,75 | d8 / Cd2 | t10 / t11 / Ct3 | ARM-2 | 25 |
| Z4 | 11.709 | 8,75 | d9 / Cd6 | t11 / t12 / Ct4 | ARM-4 | 40 |
| Z5 | 13.441 | 8,75 | d10 / Cd6 | t13 / t13 / Ct6 | ARM-4 | 40 |
| Z1 ALG | 8.463 | 9,25 | d7 / Cd3 | t9 / t10 / ct6 | ARM-3 | 32 |
| Z2 ALG | 9.882 | 9,25 | d8 / Cd3 | t10 / t11 / ct6 | ARM-3 | 32 |
| Z3 ALG | 11.454 | 9,25 | d8 / Cd3 | t11 / t12 / ct6 | ARM-3 | 32 |
| Z4 ALG | 13.073 | 9,25 | d9 / Cd6 | t12 / t13 / Ct6 | ARM-4 | 40 |
| Z5 ALG | 15.018 | 9,25 | d10 / Cd7 | t13 / t14 / Ct6 | ARM-4 | 40 |
| Z5bis | 23.798 | 10,25 | d15 / Cd7 | t19 / t16 / Ct7 | ARM-4 | 40 |
| Z6bis | 33.053 | 10,25 | d20 / Cd8 | t19 / t20 / Ct8 | ARM-4 | 40 |
| Z6E | 30.293 | 10,25 | d18 / Cd8 | t18 / t19 / Ct8 | ARM-4 | 40 |

| Poste PG1 | MLS (daN·m) | H poste (m) | Desmonte rect/circ | Terraplén M+ / M− / circ | Armadura | Esperas Ø |
|-----------|-------------|-------------|--------------------|--------------------------|----------|-----------|
| PG1 240 | 5.400 | 8,75 | d4 / Cd1 | t6 / t7 / Ct1 | ARM-2 | 25 |
| PG1 260 | 7.100 | 8,75 | d5 / Cd1 | t8 / t9 / Ct2 | ARM-2 | 25 |
| PG1 280 | 9.200 | 8,75 | d7 / Cd2 | t10 / t10 / Ct3 | ARM-2 | 25 |
| PG1 300 | 12.000 | 8,75 | d9 / Cd6 | t12 / t12 / Ct4 | ARM-4 | 40 |
| PG1 340 | 15.000 | 10,25 | d10 / Cd6 | t13 / t14 / Ct6 | ARM-4 | 40 |
| PG1 360 | 17.700 | 10,25 | d11 / Cd6 | t14 / t14 / Ct6 | ARM-4 | 40 |
| PG1 400 | 23.600 | 10,25 | d15 / Cd7 | t15 / t16 / Ct7 | ARM-4 | 40 |
| PG1 450 | 32.700 | 10,25 | d20 / Cd8 | t19 / t20 / Ct8 | ARM-4 | 40 |

### 4.7. CUÁNDO SE REQUIERE CÁLCULO ESPECÍFICO (poste, macizo, pendolado)

> **Principio del proyecto tipo Adif:** las NAE 300/301/302 **ya han calculado** postes,
> macizos, vanos y pendolado para las hipótesis del proyecto tipo. El diseñador **elige de
> catálogo** y **no recalcula**. El **cálculo específico** (que el alumno debe saber
> **identificar**, no necesariamente ejecutar) es obligatorio cuando:

| # | Situación | Consecuencia en el proyecto |
|---|-----------|-----------------------------|
| 1 | **Momento solicitante > MLS** del poste de catálogo más potente de la familia (p. ej. > 33.053 daN·m de la Z6bis, o > 23.798 de la Z5bis en configuraciones no tabuladas) | Poste **especial** con cálculo de esfuerzos y macizo propio |
| 2 | **Terreno distinto** de las hipótesis de los anejos III (C₀ = 6 daN/m³, H = 12 m, γt = 1400 daN/m³, tanα = 0,005, σlat = 1 daN/cm²) | Recálculo del macizo (NAE 106) o cimentación especial |
| 3 | **Vano o radio fuera de tabla** (apoyos por condicionantes del trazado, agujas en curvas de radio pequeño, seccionamientos de 5+ vanos) | Justificación con **cálculo de desviación lateral** (IFE apéndice E) y verificación de captación |
| 4 | **Altura del hilo fuera de rango** (pasos inferiores, túneles con altura reducida) | Recálculo de pendolado según NAE 116 y verificación de gálibo |
| 5 | **Pantógrafo distinto** de la hipótesis (1950 mm en híbridas si no hay plan de transformación; mesilla de 1600 mm) | Verificación de desviación lateral y descentramiento (IFE 4.1.2.2.1.2) |
| 6 | **Péndolas**: las tablas de distribución son de referencia; cada caso particular (vanos fuera de tabla, pendientes, agujas) requiere **cálculo específico según NAE 116** | Cálculo de péndolas y reparto en el proyecto |
| 7 | **Atirantado con tensión radial > 250 daN** (límite del conjunto de atirantado estándar) | Justificación de atirantado de hasta 400 daN o soporte especial |
| 8 | **Carga de hielo, altitud o viento** fuera de las hipótesis (altitud > 1.500 m, mapa de viento 29 m/s superado, túneles con Ktun) | Recálculo de vanos, tenses y macizos (IFE 4.1.2.2.1.4) |
| 9 | **Reutilización de postes/cimentaciones existentes** en renovación o acondicionamiento | Comprobación estructural y de gálibo con los parámetros actuales |
| 10 | **Estructuras especiales** (pórticos sobre varias vías, brazos de atirantado sobre puentes, catenaria rígida en túneles) | Cálculo propio de la estructura según su ET (03.364.101.0, 102.8…) |

**Regla de oro:** mientras el proyecto se mantiene dentro de las hipótesis del proyecto
tipo (radio ≥ mínimo tabulado, vano ≤ máximo, terreno tipo, pantógrafo y viento de la
tabla), la elección de poste/macizo es **de catálogo** (tabla anterior). Al primer caso
que se desvía de esas hipótesis, el diseño funcional se convierte en **cálculo específico**
y el proyecto debe incorporar su **memoria de cálculo justificativa**.

**Anejo IV — Configuraciones de seccionamiento (cómo se leen las tablas):**
las tablas del Anejo IV (SC y SLA, vientos 26 y 27 m/s) dan, para cada **radio y
rango de vano**, el tipo de seccionamiento (3 o 4 vanos), el patrón de
descentramiento de las **dos catenarias** en los semiejes (**Cat1** y **Cat2**, en
cm) y la **elevación del semieje e** (en m). Hipótesis: altitud 0 m, altura del hilo
5300 mm, pantógrafo 1950 mm, terreno categoría 2. SC → calle **250 mm** y
temperatura de cálculo **5 ºC**; SLA → calle **400 mm** y **0 ºC**.

Reglas de lectura:
- **3 vanos:** solo si el vano es ≥ 55 m (evita el "efecto tijera"); elevación del
  semieje 250 mm.
- **4 vanos (caso general):** elevación de semieje hasta **500 mm** en vanos ≤ 38 m;
  vanos de elevación adyacentes al eje iguales (tol. ±1 m).
- **`**`** en la tabla = limitado por la **tensión radial máxima del conjunto de
  atirantado (250 daN)**; se admite radio menor si se justifica un atirantado de
  hasta **400 daN**.
- Seccionamientos de **5+ vanos:** solo para vanos < 28 m o R < 450 m, si no es
  posible trasladarlos a un punto más favorable.
- **Ejemplo (Tabla 55, CA-220/3kV, viento 26 m/s):** R ≥ 2000 m con vanos 55–60 m →
  SC de 4 vanos, Cat1 +45/+7/+20, Cat2 +20/−18/−5, e = 0,5 m. En recta (R ≥ 20000)
  la tabla 23 permite 3 vanos con Cat1 +25/0, Cat2 0/−25, e = 0,25 m.

---

## 5. NAE 302 — CA-160H y CA-200H (híbridas)

### 5.1. Composición (4.2.1) — Tabla 4

| Elemento | CA-160H/3kV (= /25kV) | CA-200H/3kV (= /25kV) |
|----------|----------------------|----------------------|
| **Sustentador** | 150 mm² Cu ETP · **1425 kgf (1397 daN)** | 150 mm² Cu ETP · **1650 kgf (1617 daN)** |
| **Hilos de contacto** | 2× BC-120 CuAg0,1 · **2×1200 kgf (1177 daN)** | 2× BC-120 CuAg0,1 · **2×1500 kgf (1470 daN)** |
| **Péndolas** | Cu 25 mm² flexible | Cu 25 mm² flexible |
| **Cable de tierra/retorno** | LA-110 (94-AL1/22-ST1A) | LA-110 |
| **Feeder negativo** | LA-280 (242-AL1/39-ST1A) solo en 2×25 kV | Solo en 2×25 kV |
| **Feeder de refuerzo** | Generalmente no necesario (según estudio) | Generalmente necesario a 200 km/h |

**Claves del diseño híbrido:**
- Al transformar de 3 kV a 25 kV **no se cambian los conductores** (se mantienen los
  dos hilos de contacto). Solo si se pasa a **2×25 kV** se añade feeder negativo.
- **Desgaste máximo admitido del hilo: 30 %.** Carga mínima de rotura del hilo:
  4074 kgf → coeficiente de seguridad **2,43** (CA-160H, tense 1200 kgf) y **1,94**
  (CA-200H, tense 1500 kgf), con rendimiento 0,95.

### 5.2. Características geométricas y mecánicas (4.2.2)

**Altura de los hilos (Tabla 5):** nominal **5300 mm**, máxima **6000 mm**, mínima según
IFE 4.1.2.2.1.4. **Importante:** si se prevé explotación futura en 25 kV, el proyecto
debe respetar ya las alturas mínimas de la variante 25 kV.

**Pendiente (Tablas 10–11):**

| Catenaria | Pendiente máx. | Variación de pendiente |
|-----------|----------------|------------------------|
| CA-160H | ±2 ‰ | ±1 ‰ |
| CA-200H | ±1 ‰ | ±0,5 ‰ |

**Altura de sistema:** **1400 mm**; tubo estabilizador 350–450 mm (elevación ≥ 120 mm).

**Descentramiento (Tablas 13–14):**

| Radio | CA-160H | CA-200H |
|-------|---------|---------|
| R ≥ 26500 / 5000 | +20 / −20 cm | +20 / −20 cm |
| 26500 > R ≥ 12000 | +10 / −10 cm | — |
| 12000 > R ≥ 5000 | 0 / +10 cm | — |
| 5000 > R ≥ 3500 | 0 / +20 cm | — |
| 3500 > R ≥ 2500 | +15 / +15 cm | — |
| R < 2500 / 5000 | +20 / +20 cm | +20 / +20 cm |

> Hipótesis: viento 29 m/s, 0 m, 5 ºC, hilo a 5300 mm, pantógrafo **1600 mm**, terreno
> categoría 2. Los valores negativos corresponden a atirantados hacia el interior de la
> curva.

**Vano máximo (Tablas 15–18) — pantógrafo 1600 mm, viento 29 m/s:**

| Vano | CA-160H (radio) | CA-200H (radio) |
|------|-----------------|-----------------|
| 60 m | R ≥ 26500 | R ≥ 5000 |
| 60 m | 26500 > R ≥ 12000 | 5000 > R ≥ 2500 |
| 60 m | 12000 > R ≥ 5000 | 2500 > R ≥ 1750 |
| 60 m | 5000 > R ≥ 3500 | 1750 > R ≥ 1275 |
| 60 m | 3500 > R ≥ 2500 | — |
| 60 m | 2500 > R ≥ 1900 | — |
| 55 m | 1900 > R ≥ 1275 | — |
| 50 m | 1275 > R ≥ 950 | — |
| 45 m | 950 > R ≥ 675 | — |
| 40 m | 675 > R ≥ 475 | — |
| 35 m | 475 > R ≥ 350 | — |
| 30 m | 350 > R ≥ 250 | — |
| 25 m | 250 > R ≥ 180 | — |

> Excepcionalmente, si la CA-160H/3kV no está ligada a un plan de transformación, se
> pueden adoptar vanos menos restrictivos considerando solo el pantógrafo de 1950 mm.

**Cantón de compensación:** **1200 m** en recta (= 20 vanos de 60 m). Misma tabla de
vanos por cantón en curva. Elevación de semieje ≥ 250 mm.

**Seccionamientos:** configuraciones de cantón y de lámina de aire en Anejos; vanos
máximos en seccionamiento de cantón: **53 / 57 / 57 m** según viento 29 / 27 / 26 m/s
(CA-160H y CA-200H).

**Tensiones de regulación (Tablas 37–40):** tolerancia del tense y contrapeso **±2 %**.

| Elemento | CA-160H | CA-200H |
|----------|---------|---------|
| Sustentador 150 mm² | 1425 kgf · razón 1:3/1:5 (475/285 kg) | 1650 kgf · 1:3/1:5 (550/330 kg) |
| Hilos 2×120 mm² | 2×1200 kgf · 1:3/1:5 (800/480 kg) | 2×1500 kgf · 1:3/1:5 (1000/600 kg) |

### 5.3. Parámetros dinámicos (Tablas 41–42)

| Parámetro | CA-160H/3kV | CA-200H/3kV | CA-160H/25kV | CA-200H/25kV |
|-----------|-------------|-------------|--------------|--------------|
| **S0** | 60 mm | 55 mm | 34 mm | 35 mm |
| **fs** Vmáx / V=0 | 91 / 72 mm | 68 / 47 mm | 55 / 36 mm | 48 / 40 mm |

> Espacio libre de elevación: **120 mm**, verificándose **1,5·S0 < 120 mm** (más
> exigente que el 2·S0 de las catenarias clásicas).

### 5.4. Criterios de aislamiento (Tabla 43)

Las híbridas se diseñan con distancias de **25 kV**:

| Tipo | Estática | Dinámica |
|------|----------|----------|
| Fase–tierra | 270 mm | 150 mm |
| Fase–fase (desfase 120°) | 400 mm | 230 mm |
| Fase–fase (desfase 180°) | 540 mm | 300 mm |

> Excepción: si no hay plan inmediato de transformación, se admiten distancias de
> 3 kV (150 mm estática / 50 mm dinámica) en puntos singulares de replanteo difícil.

### 5.5. Postes y componentes (4.3.1)

- **Postes X-AV:** sección recta, dos UPN unidas por pletinas diagonales, altura libre
  **8,55–12,5 m**. Preferente en nuevas electrificaciones.
- **Postes XR/Z:** troncocónicos, dos UPN con presillas horizontales, altura libre
  **7,75–10,25 m** (solo admitidos en CA-160H, y para reaprovechamiento o restricciones
  de altura).
- Postes sometidos a torsión (semiejes, elevaciones de aguja) requieren **cartelas
  diagonales**; no se admiten postes de sección cerrada.
- Protección antiescalada o postes tipo HEB en zonas de vandalismo/paso de viajeros;
  galvanizado según ET 03.364.101.0 y UNE-EN ISO 1461.

---

## 6. TABLA MAESTRA — COMPARATIVA DE LAS CUATRO FAMILIAS DE 3 kV

| Parámetro | CA-160/3kV A | CA-160/3kV B | CA-220/3kV | CA-160H/3kV | CA-200H/3kV |
|-----------|--------------|--------------|------------|-------------|-------------|
| Norma | NAE 300 | NAE 300 | NAE 301 | NAE 302 | NAE 302 |
| Vmáx (km/h) | 160 | 160 | 200 | 160 | 200 |
| Pantógrafo (mm) | 1950 | 1950 | 1950 | 1600/1950 | 1600/1950 |
| Sustentador (mm² · kgf) | 150 · 1425 | 150 · 1425 | 185 · 2475 | 150 · 1425 | 150 · 1650 |
| Hilos (mm² · kgf) | 2×107 · 1050 | 2×120 · 1200 | 2×150 · 1875 | 2×120 · 1200 | 2×120 · 1500 |
| Altura nominal (mm) | 5300 | 5300 | 5300 | 5300 | 5300 |
| Altura sistema (mm) | 1400 | 1400 | 1400 | 1400 | 1400 |
| Flecha (‰) | 0,6 | 0,6 | 0,5 | 0,6 | 0,5 |
| Vano máx. (m) | 60 | 60 | 60 | 60 | 60 |
| S0 (mm) | 67 | 61 | 41 | 60 | 55 |
| fs (mm) | 98 | 89 | 42 | 91 | 68 |
| Aislam. estático/dinámico (mm) | 150/50 | 150/50 | 150/50 | 270/150 | 270/150 |
| Separación SLA / SC (mm) | 300 / 250 | 300 / 250 | 400 / 250 | (Anejo) | (Anejo) |
| Transformable a 25 kV | No | No | Aislada 25 kV | **Sí** | **Sí** |

> **Lectura de tendencias:** a mayor velocidad → sustentador e hilos más tensos y de
> mayor sección, menor flecha, menores S0/fs (mejor captación dinámica) y mayores
> separaciones de aislamiento. Las híbridas sacrifican S0/fs (más elevación dinámica)
> para poder mantener los conductores al transformar a 25 kV.

---

## 7. APLICACIÓN PRÁCTICA — SECUENCIA DE DISEÑO FUNCIONAL

Proceso para electrificar un tramo de red convencional en 3 kV:

1. **Fijar el sistema y la velocidad** (NAE 107 §4.1): 3 kV c.c., Vmáx → elegir la
   familia: ≤ 160 km/h → CA-160/3kV; 200 km/h → CA-220/3kV; con plan de futuro 25 kV →
   CA-160H o CA-200H (NAE 302).
2. **Verificar alturas** (NAE 300/301/302 §4.2.2.1): nominal 5300 mm; mínima de diseño
   según gálibo (GHE16, GEB16/GB, AF4.x, GEC16/GC), altitud y cielo abierto/túnel.
3. **Replantear vanos** (§4.2.2.5): vano máx. según radio (tablas de cada norma), con
   las hipótesis de viento (mapa Anejo I) y temperatura (5 ºC, AEMET). Respetar la
   diferencia máx. de vanos consecutivos.
4. **Fijar descentramientos** (§4.2.2.4): +20/−20 en recta; +20/+20 hacia el exterior
   en curva por debajo del radio umbral.
5. **Definir cantones de compensación** (§4.2.2.6): 1200 m en recta; nº de vanos según
   vano medio en curva; punto fijo central con latiguillos según criterios.
6. **Proyectar seccionamientos** (§4.2.2.7): de cantón (250 mm) y de lámina de aire
   (300–400 mm); 3 o 4 vanos según radio y elevación ≥ 250 mm.
7. **Diseñar agujas** (§4.2.2.8): tangencial P-90 en vías generales; cruzada P-50 en
   vías secundarias (NAE 115).
8. **Seleccionar postes y macizos** (§4.3): por función (vía general, anclaje,
   seccionamiento, aguja, pórtico) y gálibo de entrevías/andenes.
9. **Diseñar alimentación y retorno** (§4.4): feeders de Cu 235 mm² o LA-380 desde la
   subestación; conexiones cada 300 m; retorno por carriles al negativo con secciones
   ≥ a la acometida.
10. **Proteger la instalación** (§4.5–4.6): pararrayos cada 2 cantones, cable de tierra
    LA-110, tomas de 10 Ω, viseras y DLT VLD-F, medidas de avifauna (NAE 121).

> **Ejemplo tipo:** línea de 200 km/h, sin previsión de 25 kV → **CA-220/3kV (NAE 301)**.
> Sustentador 185 mm² a 2475 kgf, hilos 2×150 mm² a 2×1875 kgf, vano 60 m en recta
> (R ≥ 1700), descentramiento +20/−20, cantón de 1200 m, separación de lámina de aire
> 400 mm, S0 = 41 mm, aislamiento 150/50 mm, postes XR2–XR5.

> **Ejemplo transformable:** línea de 160 km/h con electrificación futura a 25 kV →
> **CA-160H (NAE 302)**. Se diseñan ya las alturas mínimas de 25 kV y el aislamiento
> de 25 kV (270/150 mm); al transformar solo se cambian aisladores y se adapta el
> seccionamiento, sin tocar los conductores.

---

## 8. PREGUNTAS DE AUTOEVALUACIÓN

1. ¿Cuál es la composición (sustentador, hilos y tenses) de la CA-160/3kV Tipo A? ¿Y de la Tipo B?
2. ¿Por qué la CA-220/3kV necesita generalmente feeder de refuerzo y la CA-160 no?
3. ¿Qué es lo que distingue a una catenaria híbrida (NAE 302) y qué NO hay que cambiar al transformarla a 25 kV?
4. ¿Qué desgaste máximo admiten los hilos de las catenarias híbridas y qué coeficientes de seguridad resultan?
5. Altura nominal, máxima y mínima de diseño de los hilos en las cuatro familias de 3 kV.
6. ¿A qué velocidad se exigen pendientes de ±1 ‰ y variación de ±0,5 ‰? ¿Y ±2 ‰ con ±1 ‰?
7. Vano máximo en recta de la CA-160/3kV y vano máximo para R = 800 m en el Tipo A y en el Tipo B.
8. Vano máximo de la CA-220/3kV aislada a 25 kV para R = 1500 m. ¿Y si fuera de 3 kV?
9. Descentramiento en recta de la CA-160/3kV (umbral de radio por tipo) y en curva por debajo del umbral.
10. Descentramiento de la CA-160H para R = 10000 m y para R = 3000 m.
11. Longitud máxima del cantón de compensación en recta. ¿Cuántos vanos de 60 m son?
12. ¿Cuándo se montan latiguillos de punto fijo entre sustentador e hilo?
13. Flecha máxima de los hilos de la CA-160/3kV y de la CA-220/3kV con vano de 60 m.
14. Separación entre catenarias en un seccionamiento de lámina de aire (CA-160 y CA-220). ¿Y de cantón?
15. ¿Qué tipo de aguja aérea se emplea en una vía general de 200 km/h? ¿Y entre dos vías secundarias?
16. ¿Qué poste de la CA-220 se usa para anclaje de seccionamiento y cuál para semieje/aguja (CA-160)?
17. Momento admisible de los macizos Z1 ALG, Z2 y Z6bis (referencias de la CA-160).
18. Razones de regulación y contrapesos del sustentador de la CA-220 (1:5 y 1:3).
19. Valores de S0 y fs de la CA-160H/3kV, CA-200H/3kV, CA-160H/25kV y CA-200H/25kV.
20. Espacio libre de elevación de los brazos en la CA-160 (150 mm, 2·S0) y en las híbridas (120 mm, 1,5·S0). ¿Por qué es más exigente la híbrida?
21. Distancias de aislamiento fase–tierra y fase–fase (120° y 180°) de diseño en las catenarias híbridas.
22. Características eléctricas de un aislador de 3 kV en zona de riesgo elevado (fuga, impulso, industrial).
23. Sección del retorno al pozo de negativos para una subestación de 2×6000 kW en vía doble.
24. ¿Cada cuánto se instala pararrayos y cada cuánto se hace bajada del cable de tierra?
25. ¿Qué conjunto de suspensión del feeder es más seguro para la avifauna?

---

## 9. REFERENCIAS

- **NAE 300** (2ª ed., jun 2024): CA-160/3kV — composición (4.2.1), geometría y
  mecánica (4.2.2), dinámica (4.2.3), aislamiento (4.2.4), componentes (4.3),
  alimentación/retorno (4.4), protecciones (4.5–4.6), Anejos I–IV
- **NAE 301** (2ª ed., jun 2024): CA-220/3kV — misma estructura; gálibo de postes
  (2,15 m), seccionamientos, tensiones de regulación, postes XR/Z, brazos B150–B180
- **NAE 302** (2ª ed., dic 2024): CA-160H/CA-200H — conductores transformables,
  desgaste 30 %, distancias de 25 kV, postes X-AV
- NAE 107 (2ª ed.+M1): diccionario de parámetros y fichas del Anejo 2 (lección 1)
- NAE 106: ejecución de macizos de cimentación · NAE 115: agujas aéreas ·
  NAE 116: pendolado · NAE 121: protección de avifauna
- IFE (TMA/135/2023) 4.1.2.2.1.4: altura mínima de diseño; 4.1.2.2.1.3: gradiente
  del hilo; 4.1.2.2.1.2: desviación lateral por viento
- UNE-EN 50119:2021, UNE-EN 50163, UNE-EN 50367, UNE-EN 50122-1, UNE-EN 50125-2,
  UNE-EN 50526-1, UNE-EN 50182, UNE-EN 50149, UNE-EN 1991-1-4
- ET 03.364.156.4 (pararrayos), ET 03.364.101.0 (postes), ET 03.364.103.6 (poleas)
- ETI de Energía (Reg. UE 1301/2014); Instrucción Ferroviaria de Gálibos
  (FOM/1630/2015); R.D. 223/2008 (RLAT); R.D. 664/2015 (Reglamento de Circulación)

---

*Próxima lección: componentes de la LAC (ménsulas, brazos, péndolas, seccionadores,
pararrayos) — NAE 108/109/110 y especificaciones técnicas, o bien el diseño del
circuito de retorno y tomas de tierra (NAE 104/105).*
