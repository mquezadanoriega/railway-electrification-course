# MÓDULO 6 · LECCIÓN 1
# CASOS PRÁCTICOS DE DISEÑO DE ELECTRIFICACIÓN FERROVIARIA

## Cuatro casos resueltos que integran los Módulos 0 a 5

> **Enfoque:** cada decisión se justifica citando su documento normativo, siguiendo
> la pirámide de la lección del Módulo 0: Directiva (UE) 2016/797 → TSI ENE
> (Reg. (UE) 2023/1697) → Orden ministerial (FOM/1630/2015, TMA/135/2023) →
> NAE (diseño/montaje) → ET (material) → UNE-EN (ensayos).

---

## 1. RESULTADO DE APRENDIZAJE

Al terminar esta lección serás capaz de:

1. Calcular el **gálibo mecánico y eléctrico del pantógrafo** de un vehículo real
   con la metodología de la Instrucción Ferroviaria de Gálibos (FOM/1630/2015) y
   decidir si el gálibo es correcto para la infraestructura proyectada
2. Calcular la **caída de tensión de un cantón de alimentación en 3 kV CC** con la
   ley de Ohm y decidir su viabilidad según EN 50163 y NAE 107, proponiendo
   medidas de refuerzo justificadas
3. **Verificar un cantón contra la TSI ENE** (rangos de tensión y fuerza de
   contacto) y saber distinguir un límite permanente de uno excepcional
4. **Seleccionar el tipo de catenaria de 25 kV**, la línea de fuga del aislador y
   la separación entre subestaciones para una nueva línea de alta velocidad
5. **Integrar los Módulos 0 a 5** en una secuencia de diseño única y defendible
   ante una revisión de proyecto

---

## 2. CÓMO USAR ESTE MÓDULO

Este módulo es la **síntesis práctica** del curso. No introduce normativa nueva:
**integra** la vista en los Módulos 0 a 5. Se recomienda trabajarlo en este orden:

1. **Resuelve cada caso primero tú**, con papel y calculadora, antes de leer la
   resolución. Los datos de partida bastan para resolverlos.
2. **Compara con la resolución** y verifica cada fórmula y cada cita normativa.
3. **Consulta la lección de origen** cuando un valor parezca «de memoria»:
   cada dato usado está tomado de las lecciones 1 a 13 de los Módulos 1 a 5.

Los cuatro casos están **encadenados a propósito**:

| Caso | Integra | Resultado que alimenta |
|------|---------|------------------------|
| **1** · Gálibo del pantógrafo | Módulo 3 (gálibos) + NAE 107 | Define el espacio libre de la LAC (insumo del Caso 2) |
| **2** · Cantón de 3 kV CC | Módulo 1 (ley de Ohm) + Módulo 5 (SET-CC) | Fija la tensión en el pantógrafo (insumo del Caso 3) |
| **3** · Verificación ETI ENE | Módulo 4 (TSI ENE / IFE) + EN 50163 | Dictamina la interoperabilidad del cantón |
| **4** · Catenaria y aisladores 25 kV | Módulo 5 (NAE 107/300/301/302, ET 03.364) | Selección de materiales para una línea nueva |

> **Nota de contexto:** el trazado de los Casos 2 y 3 discurre por la **vía con
> desnivel y balasto** presentada en el Caso 1. El desnivel no interviene en el
> gálibo lateral del pantógrafo (Caso 1), pero sí condiciona la demanda de
> tracción: en las rampas el tren demanda la **punta de tracción** que se estudia
> en los Casos 2 y 3.

---

## 3. CASO 1 — GÁLIBO DE PANTÓGRAFO

### 3.1. Datos de partida

Se quiere electrificar una vía de ancho ibérico por la que circulará un tren de
**ancho nominal de caja 3.000 mm** con **pantógrafo de mesilla 1.950 mm**, en una
línea con **desnivel y balasto**. El sistema es **3 kV CC** y la catenaria prevista
es la **CA-160/3kV** (red convencional, 160 km/h). Se pide el **gálibo eléctrico**
y el **semigálibo del pantógrafo**.

| Parámetro | Valor | Origen normativo |
|-----------|-------|------------------|
| Ancho de mesilla del pantógrafo | 1.950 mm → **bw = 975 mm** | FOM/1630/2015, cuadro 3.5 (3 kV) |
| Vehículo | Ancho nominal 3.000 mm; longitud 26 m; distancia entre centros de bogies L = 19 m; batalla de bogie n = 3 m | Hipótesis del caso |
| Vía | Ancho ibérico, balasto (en mal estado según hipótesis de gálibo uniforme) | FOM/1630/2015, 3.10.7 |
| Curva de estudio | R = 600 m, insuficiencia de peralte I = 100 mm | Hipótesis del caso |
| Coeficiente de balanceo | **s'0 = 0,225**; altura del centro de balanceo h'c0 = 0,5 m | FOM/1630/2015, 3.10.4.2 |
| Altura de verificación máxima | **h'0 = 6,5 m** → **ep = epo = 0,170 m** | FOM/1630/2015, 3.10.4.2 |
| Altura de verificación mínima | **h'u = 5 m** → ep = epu = 0,110 m | FOM/1630/2015, 3.10.4.2 |
| Catenaria CA-160/3kV: altura del hilo | **hf = 5.300 mm** (nominal) | NAE 107, tabla 6 |
| Elevación del hilo por la fuerza F | **fs = 120 mm** (centro de vano, Fm y Vmáx) | FOM/1630/2015, cuadro 3.6 (CA-160) |
| Elevación por flexibilidad + desgaste | **fws + fwa = 70 mm** | FOM/1630/2015, cuadro 3.6 |
| Distancia de aislamiento 3 kV | Estática **150 mm** / dinámica **50 mm** | FOM/1630/2015, cuadro 3.7 · UNE-EN 50119 |
| Trocador aislado | **cw = 0** (línea nueva, trocadores no aislados) | FOM/1630/2015, 3.5.2 |
| Margen de aleatorios | **j' = 50 mm** (media cuadrática × K', K' = 1) | FOM/1630/2015, anejo 7 |

### 3.2. Método

El gálibo del pantógrafo se calcula en dos pasos (Módulo 3, lección 1):

1. **Gálibo mecánico** — distancia horizontal mínima del obstáculo al eje del
   pantógrafo y altura máxima ocupada por el pantógrafo en captación:

```
b_mec (interior) = bw + ep + S'i + qs'i + j'
b_mec (exterior) = bw + ep + S'a + qs'a + j'
h_pantógrafo     = hf + fs + fws + fwa
```

2. **Gálibo eléctrico** — se obtiene del mecánico añadiendo la **distancia de
   aislamiento** `belec` (cuadro 3.7) y descontando la proyección del trocador
   aislado `cw`:

```
b_elect = b_mec + belec − cw
h_elect = h_mec + belec
```

Reglas de aplicación (FOM/1630/2015, 3.5.2.1):

- En **curva**: `belec` **estática (150 mm)** en el **lado interior** y **dinámica
  (50 mm)** en el **lado exterior**.
- En **recta**: envolvente de (gálibo mecánico a Vmáx + dinámica) y (gálibo
  mecánico a V = 0 + estática).
- Los **salientes** por inscripción en curva de un vehículo con bogies se estiman
  con la geometría del vehículo:

```
S'i = (L² − n²) / (8R)        (saliente interior, centro del vehículo)
S'a = (a² − L²) / (8R)        (saliente exterior, extremos del vehículo)
```

- Los **cuasiestáticos** `qs'` se obtienen por el procedimiento de EN 15273-3 a
  partir de `s'0`, de la insuficiencia de peralte `I` y de la altura del punto de
  contacto. Con los datos del caso (s'0 = 0,225, I = 100 mm, punto de contacto a
  5,5 m) resulta **qs' = 75 mm**.
- Los **aleatorios** `j'` se combinan como **media cuadrática** multiplicada por
  `K'` (K' = 1 para el gálibo del pantógrafo, anejo 7).

### 3.3. Cálculo paso a paso

**Paso 1 — Salientes en la curva R = 600 m**

```
S'i = (19² − 3²) / (8 · 600) = 352 / 4.800 = 0,073 m ≈ 73 mm
S'a = (26² − 19²) / (8 · 600) = 315 / 4.800 = 0,066 m ≈ 66 mm
```

**Paso 2 — Semiancho del gálibo mecánico (a h'0 = 6,5 m, ep = 170 mm)**

```
Recta:          b_mec = 975 + 170 + 0 + 0 + 50 = 1.195 mm
Curva interior: b_mec = 975 + 170 + 73 + 75 + 50 = 1.343 mm
Curva exterior: b_mec = 975 + 170 + 66 + 75 + 50 = 1.336 mm
```

**Paso 3 — Gálibo eléctrico (3 kV, cw = 0)**

```
Recta:          b_elect = 1.195 + 150 − 0 = 1.345 mm
Curva interior: b_elect = 1.343 + 150 − 0 = 1.493 mm
Curva exterior: b_elect = 1.336 + 50 − 0  = 1.386 mm
```

> El **semigálibo eléctrico** es el valor de `b_elect`: **1.345 mm en recta** y
> **1.493 mm en el lado interior de la curva**. El **gálibo eléctrico** (anchura
> total) es la suma de ambos semianchos: ≈ **2.690 mm en recta**.

**Paso 4 — Alturas del gálibo**

```
h_mec   = hf + fs + fws + fwa = 5.300 + 120 + 70 = 5.490 mm
h_elect = h_mec + belec       = 5.490 + 150      = 5.640 mm
```

**Paso 5 — Verificación en la altura mínima h'u = 5 m**

Con ep = epu = 0,110 m (y el hilo a 5.000 mm de altura mínima de verificación):

```
b_mec (recta, h'u) = 975 + 110 + 50 = 1.135 mm  → menos restrictivo que a h'0
h_mec (h'u)        = 5.000 + 120 + 70 = 5.190 mm → h_elect = 5.340 mm ≤ 6.500 mm ✓
```

La verificación a **h'0 = 6,5 m es la dominante** (mayor ep y mayor hf), por lo
que el diseño se gobierna con ella.

### 3.4. Resultado

| Magnitud | Recta | Curva interior (R = 600 m) | Curva exterior |
|----------|-------|----------------------------|----------------|
| Semiancho mecánico `b_mec` | 1.195 mm | 1.343 mm | 1.336 mm |
| **Semigálibo eléctrico `b_elect`** | **1.345 mm** | **1.493 mm** | **1.386 mm** |
| Gálibo eléctrico (anchura total) | ≈ 2.690 mm | ≈ 2.879 mm | ≈ 2.879 mm |
| Altura del gálibo `h_elect` | **5.640 mm** | 5.640 mm | 5.640 mm |

### 3.5. Decisión de diseño

**El gálibo es CORRECTO.** Se comprueba contra los cuatro criterios que deciden
la validez:

1. **Altura máxima:** `h_elect = 5.640 mm ≤ h'0 = 6.500 mm` ✓ — el pantógrafo en
   captación no rebasa la altura de verificación en túneles y pasos inferiores.
2. **Anchura frente a la implantación:** el poste más próximo (a tierra) en ancho
   ibérico con GEB16 y ménsulas de celosía se sitúa a **3,00 m del eje de la vía**
   en recta y **3,20 m en curva** (NAE 107, tabla 10) ≫ 1.493 mm ✓ — la caja del
   tren (semiancho 1.500 mm) y el pantógrafo no alcanzan la estructura.
3. **Distancia de aislamiento:** cualquier obstáculo **no aislado** (poste,
   pórtico, muro de túnel) debe quedar a más de **150 mm** (estática) o **50 mm**
   (dinámica) de las partes en tensión del pantógrafo y de la catenaria ✓.
4. **Interoperabilidad:** el pantógrafo de **1.950 mm es el estándar admisible en
   3 kV** (bw = 975 mm, cuadro 3.5 y NAE 107 tabla 2), compatible con el gálibo
   de la línea definido por la TSI ENE ✓.

**Qué decide que el gálibo sea correcto o incorrecto (criterio general):**

- El gálibo es **correcto** si la envolvente eléctrica cabe dentro del espacio
  libre que deja la infraestructura (gálibo de implantación de obstáculos) **y**
  si las partes no aisladas del pantógrafo quedan a la distancia de aislamiento
  reglamentaria de los obstáculos no aislados.
- El gálibo es **incorrecto** si se produce alguno de estos incumplimientos:
  - `h_elect > h'0` (6,5 m): la instalación no pasa por túneles ni pasos
    superiores.
  - `b_elect` invade el gálibo de implantación (choca con postes, pórticos,
    pantallas antirruido o muros).
  - Un obstáculo no aislado queda a menos de `belec` de la catenaria.
  - El pantógrafo del vehículo supera el gálibo declarado de la línea
    (incompatibilidad de interoperabilidad).

**Medidas correctoras si no cumpliese:** reducir `hf` (dentro del rango de la
NAE 107: nominal 5.300 mm, máx. 6.000 mm), elegir una catenaria de menor `fs` (la
CA-220/3kV tiene fs = 42 mm frente a 120 mm de la CA-160), alejar la implantación
de postes, o — como último recurso — estrechar la mesilla (no admisible en 3 kV,
donde la de 1.600 mm está prohibida). Las distancias de aislamiento y la línea de
fuga del Caso 4 completan esta lógica para 25 kV.

---

## 4. CASO 2 — CANTÓN DE ALIMENTACIÓN EN 3 kV CC

### 4.1. Datos de partida

Sobre la línea del Caso 1 (3 kV CC), se estudia un **cantón de 15 km** alimentado
por una **subestación de tracción (SET) de CC**. En la **punta de tracción**
(rampa de máximo esfuerzo) un tren demanda **3.000 A** a **10 km** de la SET. La
resistencia de bucle (hilo + carril de retorno) es **0,18 Ω/km**.

| Parámetro | Valor | Origen normativo |
|-----------|-------|------------------|
| Tensión de la SET (barra de CC) | **3.300 V** | NAE 107, 4.1.1 (diseño Adif) · ET 03.359.104.1 |
| Tensión mínima de contacto (3 kV) | **2.000 V (Umin2)** | UNE-EN 50163 · NAE 107, tabla 1 |
| Tensión nominal | 3.000 V (Un); Umin1 = 3.000 V; Umax1 = 3.600 V | UNE-EN 50163 · NAE 107, tabla 1 |
| Corriente en punta de tracción | 3.000 A | Dato del caso |
| Distancia del tren a la SET | 10 km | Dato del caso |
| Resistencia de bucle | 0,18 Ω/km | Módulo 1, lección 1 (ejemplo resuelto) |

### 4.2. Método

En corriente continua la caída de tensión depende solo de la **resistencia** del
bucle (hilo + carril de retorno), sin componente reactiva:

```
ΔU = I · R_bucle · L
U_pantógrafo = U_SET − ΔU
```

El cantón es **viable** si en las condiciones más desfavorables se cumple
`U_pantógrafo ≥ Umin2 = 2.000 V`, es decir, si la caída no supera el margen:

```
ΔU_adm = U_SET − Umin2 = 3.300 − 2.000 = 1.300 V
```

### 4.3. Cálculo paso a paso

**Paso 1 — Caída de tensión en punta de tracción**

```
ΔU = I · R · L = 3.000 A · 0,18 Ω/km · 10 km = 5.400 V
U_pantógrafo = U_SET − ΔU = 3.300 − 5.400 = −2.100 V
```

La tensión resultante es **negativa**: la corriente de 3.000 A no puede recorrer
10 km con ese bucle. El cantón **NO es viable** en las condiciones dadas.

**Paso 2 — Comparación con el margen admisible**

```
ΔU = 5.400 V  >  ΔU_adm = 1.300 V   →  NO CUMPLE (EN 50163 / NAE 107)
```

**Paso 3 — Distancia y corriente límite**

```
Distancia máxima para 3.000 A:  L_máx = ΔU_adm / (I · R) = 1.300 / (3.000 · 0,18) = 2,41 km
Corriente máxima a 10 km:        I_máx = ΔU_adm / (R · L) = 1.300 / (0,18 · 10) = 722 A
```

La demanda (3.000 A) es **más de 4 veces** la corriente admisible a 10 km, y la
SET debería estar a **menos de 2,5 km** del tren para sostener la punta de
tracción con este bucle.

### 4.4. Resultado

| Magnitud | Valor | Verificación |
|----------|-------|--------------|
| Caída de tensión en punta | **5.400 V** | > 1.300 V admisibles |
| Tensión en el pantógrafo | **−2.100 V** | << 2.000 V (Umin2) |
| Distancia máxima SET–tren | **2,41 km** | cantón de 15 km imposible sin refuerzo |
| Corriente máxima a 10 km | **722 A** | demanda 3.000 A → inviable |
| **Viabilidad** | **INVIABLE** | exige medidas de refuerzo |

### 4.5. Decisión de diseño — dos soluciones

**Solución 1 — Más alimentación (refuerzo del cantón).** Se alimenta el cantón
**por ambos extremos** (puesta en paralelo de las SETs colaterales, coordinada por
el gestor de protecciones 3,3 kV de la ET 03.359.110.8) y se añade **feeder de
refuerzo** (2× Cu 235 mm², según NAE 300 §4.4) que reduce la resistencia del bucle
a la mitad (**0,09 Ω/km**):

```
Corriente repartida por el extremo más próximo:  I = 3.000 · (10/15) = 2.000 A a 5 km
Caída en el alimentador más cargado:             ΔU = 2.000 · 0,09 · 5 = 900 V
(La corriente por el extremo lejano es 1.000 A a 10 km → ΔU = 1.000 · 0,09 · 10 = 900 V,
 igual caída por ambos caminos, coherente con el paralelo.)
U_pantógrafo = 3.300 − 900 = 2.400 V ≥ 2.000 V   →  VIABLE ✓
```

**Solución 2 — Doble vía y acercamiento de la alimentación.** La punta de
tracción se alimenta de **las dos vías en paralelo** (cada una con su retorno
independiente), repartiendo la corriente a **1.500 A por vía**, y se alimenta
desde el **extremo más próximo** (5 km):

```
ΔU = I · R · L = 1.500 · 0,18 · 5 = 1.350 V  →  supera por poco el margen (1.300 V)
```

La doble vía sola se queda a 50 V del límite; se completa **con el feeder de
refuerzo** (0,09 Ω/km):

```
ΔU = 1.500 · 0,09 · 5 = 675 V  →  U_pantógrafo = 3.300 − 675 = 2.625 V ≥ 2.000 V  →  VIABLE ✓
```

**Variante de la Solución 2 — reducir la distancia.** La distancia límite de
2,41 km confirma la regla del Módulo 1 («la SET debe estar a < 3 km del punto de
máxima demanda»). Ubicar SETs (o puntos de puesta en paralelo seccionables) cada
**≤ 4,8 km** deja un peor caso de 2,4 km:

```
ΔU = 3.000 · 0,18 · 2,4 = 1.296 V < 1.300 V  →  VIABLE ✓ (margen mínimo, 4 V)
```

**Lectura final:** en la práctica de la red española las SETs de CC van cada
**12–20 km** (ET 03.359) y los picos se cubren **combinando** doble vía, feeders
de refuerzo y puesta en paralelo de SETs colaterales; una sola medida no basta
para sostener puntas de 3.000 A a gran distancia.

---

## 5. CASO 3 — VERIFICACIÓN ETI ENE

### 5.1. Datos de partida

Se verifica el mismo cantón del Caso 2 contra la **ETI de Energía (TSI ENE)**.
Como condición de explotación se toma la del cantón **reforzado con la Solución 1**
del Caso 2: tensión en el pantógrafo en punta de tracción **U = 2.400 V**.

| Parámetro | Valor | Origen normativo |
|-----------|-------|------------------|
| Tensión en el pantógrafo (punta, cantón reforzado) | **2.400 V** | Resultado del Caso 2 |
| Rango de funcionamiento 3 kV (TSI ENE / EN 50163) | **2.000 – 3.600 V** (Umin2–Umax1) | TSI ENE (Reg. (UE) 2023/1697) · EN 50163 |
| Tensión máxima transitoria 3 kV | 3.900 V (Umax2) | EN 50163 · NAE 107, tabla 1 |
| Tensión mínima permanente 3 kV | **3.000 V (Umin1)** | EN 50163 · NAE 107, tabla 1 |
| Fuerza de contacto media exigible | **60 – 90 N** | IFE (TMA/135/2023) · UNE-EN 50367 |

### 5.2. Método

La verificación de la TSI ENE se hace en dos planos:

1. **Tensión en el pantógrafo** — debe mantenerse dentro del rango de la EN 50163
   para el sistema (3 kV: 2.000–3.600 V en régimen, 3.900 V transitorio).
2. **Fuerza de contacto pantógrafo–hilo** — debe cumplir la estadística de la
   IFE/UNE-EN 50367 (media Fm en 60–90 N), verificada por auscultación.

### 5.3. Cálculo y verificación de la tensión

**Paso 1 — Límite absoluto (Umin2)**

```
U_pantógrafo = 2.400 V ≥ Umin2 = 2.000 V  →  CUMPLE el límite absoluto de la TSI ENE ✓
2.000 V ≤ 2.400 V ≤ 3.600 V               →  dentro del rango de funcionamiento ✓
```

**Paso 2 — Límite permanente (Umin1) — lectura crítica**

```
2.400 V < Umin1 = 3.000 V
```

La tensión de 2.400 V queda en la franja **«no permanente»** de la EN 50163
(entre Umin2 y Umin1). La TSI ENE admite ese valor **solo como condición
excepcional de corta duración** (punta de tracción en rampa), nunca como estado de
diseño sostenido. En régimen normal la tensión debe mantenerse por encima de
**3.000 V**.

```
Régimen normal: ΔU_normal ≤ 3.300 − 3.000 = 300 V  →  U ≥ 3.000 V ✓
```

**Paso 3 — Límite superior**

En vacío, la SET entrega 3.300 V por diseño (NAE 107, 4.1.1), por debajo de
Umax1 = 3.600 V y de Umax2 = 3.900 V ✓ — no hay riesgo de sobretensión permanente
en el pantógrafo.

### 5.4. Fuerza de contacto (comentario IFE / UNE-EN 50367)

Además de la tensión, la TSI ENE y la IFE exigen **calidad de captación**: la
**fuerza de contacto media Fm** del estadístico de auscultación debe estar en el
rango **60–90 N**:

- **Fm < 60 N** → riesgo de **pérdida de contacto** (arqueos, chispas en la
  mesilla y erosión del hilo).
- **Fm > 90 N** → **desgaste prematuro** de la pletina del pantógrafo y del hilo
  de contacto.

La fuerza media está ligada a la elevación `fs` del hilo (por eso la instrucción
de gálibos da `fs` por tipo de catenaria y fuerza, cuadro 3.6): en el Caso 1 se
usó `fs = 120 mm` para la CA-160 con Fm a Vmáx, valor coherente con este rango de
fuerzas.

**Nota de verificación práctica (NAE 107, 4.1.2):** para fijar la velocidad máxima
de diseño **no es obligatoria la auscultación dinámica hasta 160 km/h en CC** (la
CA-160/3kV del caso va a 160 km/h); basta la medición de la geometría de la LAC.
En líneas más rápidas (25 kV > 120 km/h o CC > 160 km/h) la verificación de Fm se
hace por auscultación dinámica según UNE-EN 50367.

### 5.5. Resultado

| Requisito | Exigencia TSI ENE / IFE | Valor calculado | Cumple |
|-----------|-------------------------|-----------------|--------|
| Tensión mínima absoluta | ≥ 2.000 V (Umin2) | 2.400 V | ✓ |
| Tensión mínima permanente | ≥ 3.000 V (Umin1) en régimen | 3.300 V (vacío) / 2.400 V (punta, excepcional) | ✓ (con matiz) |
| Tensión máxima | ≤ 3.600 V (Umax1) | 3.300 V | ✓ |
| Fuerza de contacto media | 60–90 N (Fm) | Verificar por auscultación | ✓ (diseño) |

**Conclusión:** el cantón reforzado **cumple la TSI ENE** (2.400 V dentro de
2.000–3.600 V). El matiz operativo: 2.400 V es un valor **excepcional de punta**;
si esa tensión se sostuviera en el tiempo, el diseño no cumpliría el régimen
permanente (≥ 3.000 V) y habría que volver a las medidas del Caso 2. La
verificación documental ante el órgano autorizador exige **justificar la duración**
de la condición de 2.400 V.

---

## 6. CASO 4 — SELECCIÓN DE CATENARIA Y AISLADORES PARA 25 kV

### 6.1. Datos de partida

Se proyecta una **nueva línea de alta velocidad a 200 km/h** electrificada en
**25 kV CA (50 Hz)**. Se pide:

1. Seleccionar el **tipo de catenaria** entre las del curso (CA-160, CA-220,
   CA-160H y CA-200H en sus versiones de 25 kV, fichas del Anejo 2 de la NAE 107 y
   normas NAE 300/301/302).
2. Justificar la **línea de fuga del aislador** con los valores de la ET 03.364
   presentes en el curso.
3. **Dimensionar la separación entre subestaciones** (rango 25 kV: 60–100 km).

| Parámetro | Valor | Origen normativo |
|-----------|-------|------------------|
| Sistema | 25 kV CA, 50 Hz (Un 25.000 V; Umin1 19.000; Umin2 17.500; Umax1 27.500; Umax2 29.000) | EN 50163 · NAE 107, tabla 1 |
| Velocidad máxima de proyecto | 200 km/h | Dato del caso |
| Tensión de diseño en la SET | 27.500 V | NAE 107, 4.1.1 (diseño Adif) |
| Potencia por tren (punta) | 6 MW, cosφ = 0,95 | Hipótesis del caso |
| Tráfico simultáneo de cálculo | 2 trenes | Hipótesis del caso |

### 6.2. Método — selección del tipo de catenaria

La secuencia de selección sigue la NAE 107 §7: fijar sistema → fijar Vmáx →
elegir tipología en las fichas del Anejo 2 → verificar gálibos, aislamiento y
parámetros dinámicos. Las fichas de 25 kV disponibles en el curso son:

| Catenaria | Vmáx (km/h) | Hilo de contacto | Sustentador | S0 (mm) | fs (mm) | Lámina F–T / F–F (mm) | Vano máx. (m) |
|-----------|-------------|------------------|-------------|---------|---------|------------------------|---------------|
| CA-200/25kV | 200 | 1× BC-120 CuAg0,1 (1545 daN) | Cu ETP 95 (1543 daN) | 46 | 78 | 300 / 400 | 60 |
| CA-220/25kV | 220 | 1× BC-150 CuAg0,1 (1837 daN) | Cu ETP 95 (1543 daN) | 43 | 77 | 450 / 450 | 60 |
| CA-160H/25kV | 160 | 2× BC-120 CuAg0,1 (1176 daN) | Cu ETP 150 (1397 daN) | 34 | 55 | 300 / 400 | 60 |
| **CA-200H/25kV** | **200** | **2× BC-120 CuAg0,1 (1470 daN)** | **Cu ETP 150 (1617 daN)** | **35** | **48** | **300 / 400** | **60** |

### 6.3. Cálculo — comparación y justificación

**Selección: CA-200H/25kV** (NAE 302, variante 25 kV). Justificación:

1. **Velocidad:** Vmáx de proyecto = 200 km/h, coincide exactamente con la
   CA-200H/25kV (y con la CA-200/25kV). La CA-160H (160 km/h) se queda corta; la
   CA-220/25kV (220 km/h) es válida pero de mayor exigencia mecánica.
2. **Diseño como 25 kV desde el origen:** la CA-200H/25kV está diseñada con
   distancias de aislamiento de 25 kV (estática 270 mm / dinámica 150 mm
   fase–tierra; 400/230 mm fase–fase a 120°) según NAE 302, sin necesidad de
   transformaciones posteriores.
3. **Doble hilo de contacto** (2×120 mm² CuAg0,1): mayor capacidad de corriente y
   redundancia de captación para una línea de altas prestaciones; la CA-200/25kV
   usa hilo único (1×120 mm²).
4. **Calidad de captación:** S0 = 35 mm y fs = 48 mm, los valores más favorables
   del rango de 200 km/h (frente a 46/78 de la CA-200/25kV): menos elevación del
   hilo en el brazo de atirantado y en el vano a 200 km/h.
5. **Geometría:** altura nominal 5.300 mm, altura de sistema 1400 mm, flecha
   0,5 ‰, vano máximo 60 m y descentramiento ±20 cm, compatibles con el gálibo
   del pantógrafo del Caso 1 (1950 mm admisible, igual que 1600 mm).
6. **Materiales:** ménsulas tubulares de aluminio y postes X-AV, la solución
   preferente de Adif para nuevas electrificaciones (NAE 302 §4.3.1).

**Por qué no las otras tres:**

- **CA-160** (familia NAE 300): catenaria clásica de 3 kV a 160 km/h; sin versión
  propia de nueva instalación a 200 km/h.
- **CA-160H/25kV:** híbrida pero limitada a 160 km/h → insuficiente para la línea
  proyectada.
- **CA-220/25kV:** apta (220 km/h), pero con hilo único 1×150 mm² y mayores
  tenses (1875 kgf); la CA-200H/25kV ofrece mejor dinámica (S0/fs) y doble hilo a
  igual velocidad de proyecto.

> **Nota:** para velocidades > 200 km/h el curso ofrece las catenarias de AV
> propias (C-350, SICAT H 1.0, EAC-350); quedan fuera de este caso, fijado a
> 200 km/h.

### 6.4. Línea de fuga del aislador (ET 03.364)

En 25 kV el aislamiento se dimensiona por **línea de fuga** según el nivel de
contaminación (grupo II, PD4A, propio de una línea de AV en servicio prolongado):

| Componente | Línea de fuga | Ensayos | Origen en el curso |
|-----------|---------------|---------|---------------------|
| **Aislador de catenaria (25 kV)** | **≥ 1.200 mm** (grupo II, PD4A) | Impulso rayo en seco **200 kV** (cresta); frecuencia industrial bajo lluvia **95 kV** (1 min) | NAE 301, tabla 33 (ET 03.364) |
| **Seccionador unipolar de catenaria** | **≥ 1.160 mm** (tipo C4-250 o superior) | Impulso a tierra 200 kV / entre partes 220 kV; industrial a tierra 95 kV / entre partes 110 kV | ET 03.364.150.7 |
| Excepción | 900 mm | Solo zonas **no contaminadas y fuera de túnel** | NAE 301, tabla 33 (nota) |

**Justificación:** a 25 kV la fuga exigida es de **1.200 mm** (≈ 48 mm/kV) frente
a los 300–400 mm del 3 kV. La longitud de fuga larga evita las **descargas
superficiales (tracking)** que provocan la contaminación (sal marina, polvo,
niebla y emisiones de la vía) y garantiza el nivel de aislamiento exigido por la
UNE-EN 50119 y la TSI ENE. El seccionador de catenaria cumple con el aislador
**C4-250** (fuga 1.160 mm) según la ET 03.364.150.7; la excepción de 900 mm solo
es admisible con justificación específica de no contaminación.

### 6.5. Separación entre subestaciones (25 kV)

El rango normativo del curso (Módulo 1, lección 1) es de **60–100 km** entre SETs
de 25 kV, frente a los 12–20 km de la CC. Se dimensiona con un cálculo de
orden de magnitud de caída de tensión:

**Datos de cálculo:**

```
Demanda simultánea: 2 trenes × 6 MW = 12 MW
I = P / (U · cosφ) = 12·10⁶ / (25.000 · 0,95) ≈ 505 A ≈ 500 A
Sistema 2×25 kV (autotransformador): X_ef ≈ 0,18 Ω/km (hipótesis de diseño)
  (en 1×25 kV la reactancia típica es X ≈ 0,35 Ω/km)
Alimentación por ambos extremos: 250 A por SET · distancia máx = L_SET / 2
Margen admisible: ΔU_adm = 27.500 − 25.000 = 2.500 V (mantener ≥ Un en régimen)
```

**Verificación de caída:**

```
L_SET = 100 km → ΔU = 250 · 0,18 · 50 = 2.250 V ≤ 2.500 V  →  ✓ (justo)
L_SET =  80 km → ΔU = 250 · 0,18 · 40 = 1.800 V ≤ 2.500 V  →  ✓ (adoptado)
L_SET =  60 km → ΔU = 250 · 0,18 · 30 = 1.350 V ≤ 2.500 V  →  ✓ (cómodo)
```

**Resultado adoptado: L_SET = 80 km** (dentro del rango 60–100 km del curso).

```
U_pantógrafo en el punto medio = 27.500 − 1.800 = 25.700 V
25.700 V ≥ 25.000 V (Un) ✓  y  17.500 ≤ 25.700 ≤ 27.500 (EN 50163) ✓
Para una línea de 240 km → 3 cantones de 80 km → 4 SETs
```

**Nota de proyecto:** el valor definitivo se cierra con el **estudio eléctrico**
del trazado (simulación de tráfico, perfil de rampas, régimen de frenado
regenerativo), siguiendo NAE 107 §4.1.1 y las ET 03.359.501 de subestaciones de
CA. La comprobación aquí presentada es la de orden de magnitud que permite fijar
el rango de partida (60–100 km) del Módulo 1.

---

## 7. TABLA RESUMEN DE DECISIONES Y NORMAS APLICADAS

| Caso | Decisión adoptada | Valores clave | Normativa aplicada |
|------|-------------------|---------------|--------------------|
| **1 · Gálibo de pantógrafo** | Gálibo **CORRECTO** | Semigálibo eléctrico 1.345 mm (recta) / 1.493 mm (curva interior); altura 5.640 mm ≤ 6.500 mm | Orden FOM/1630/2015 (3.5, cuadros 3.5–3.7, anejo 7) · UNE-EN 50119:2010 · NAE 107 (tabla 6, Anejo 2) · TSI ENE |
| **2 · Cantón de 3 kV CC** | **INVIABLE** en una sola vía → reforzar | ΔU = 5.400 V; L_máx = 2,41 km; solución adoptada ΔU = 900 V → U = 2.400 V | UNE-EN 50163 · NAE 107 (tabla 1) · NAE 300 §4.4 (feeders) · ET 03.359.104.1 y 03.359.110.8 · Módulo 1 (ley de Ohm) |
| **3 · Verificación ETI ENE** | **CUMPLE** (con matiz de duración) | U = 2.400 V ∈ [2.000; 3.600] V; 2.400 < Umin1 = 3.000 V → solo puntual; Fm 60–90 N | TSI ENE (Reg. (UE) 2023/1697) · EN 50163 · IFE (TMA/135/2023) · UNE-EN 50367 · NAE 107 §4.1.2 |
| **4 · Catenaria y aisladores 25 kV** | **CA-200H/25kV** · fuga **1.200 mm** · SET cada **80 km** | S0 = 35 mm, fs = 48 mm, doble hilo 2×120; aislador 200 kV impulso / 95 kV industrial; ΔU = 1.800 V a 80 km | NAE 107 (Anejo 2) · NAE 302 · NAE 301 (tabla 33) · ET 03.364.150.7 · ET 03.359.501 · EN 50163 · Módulo 1 (60–100 km) |

**Cadena de justificación de cada decisión (Módulo 0):** cada valor anterior se
defiende citando, en orden, el requisito europeo (TSI ENE), la instrucción
estatal (FOM/1630/2015, IFE TMA/135/2023), la norma de diseño de Adif (NAE 107 /
300 / 301 / 302), la especificación de material (ET 03.364 / 03.359) y la norma
UNE-EN de ensayo o referencia.

---

## 8. PREGUNTAS DE AUTOEVALUACIÓN

1. ¿Qué semiancho de mesilla `bw` corresponde a un pantógrafo de 1.950 mm en una
   línea de 3 kV, y por qué no se admite la mesilla de 1.600 mm en 3 kV?
2. Diferencia entre **gálibo mecánico** y **gálibo eléctrico** del pantógrafo.
   ¿A qué obstáculo se exige cada uno según su conexión eléctrica?
3. ¿Por qué en una curva la distancia de aislamiento **estática** se aplica en el
   lado **interior** y la **dinámica** en el exterior?
4. Calcula la caída de tensión de un tren de **2.400 A** a **8 km** de la SET con
   bucle de **0,2 Ω/km**. ¿Es viable con la SET a 3.300 V y mínimo de 2.000 V?
   *(Solución: ΔU = 2.400 · 0,2 · 8 = 3.840 V → U = −540 V → inviable.)*
5. ¿Qué representa **Umin2** de la EN 50163 para 3 kV (2.000 V) y cuál es su
   consecuencia práctica en el dimensionado del cantón?
6. El resultado del Caso 3 (U = 2.400 V) cumple el límite absoluto de la TSI ENE
   pero está por debajo de **Umin1 = 3.000 V**. ¿Por qué es admisible solo de
   forma puntual?
7. Rango de la **fuerza de contacto media** exigida por la IFE/UNE-EN 50367 y qué
   ocurre si Fm queda fuera de ese rango (bajo y alto).
8. ¿Por qué se selecciona la **CA-200H/25kV** y no la CA-160H ni la CA-220/25kV
   para una línea nueva a 200 km/h?
9. ¿Qué **línea de fuga** exige Adif para el aislador de catenaria de 25 kV
   (grupo II, PD4A) y qué excepción admite?
10. ¿Entre qué valores se separan las SETs en 25 kV y en 3 kV, y por qué el 25 kV
    permite distancias mucho mayores?

---

## 9. REFERENCIAS

- **Orden FOM/1630/2015** (Instrucción Ferroviaria de Gálibos, BOE-A-2015-8765):
  apartados 3.5, 3.5.1, 3.5.2, 3.10.4.2, 3.10.7; cuadros 3.5, 3.6, 3.7; anejo 7
- **TSI ENE (ETI de Energía)**: Reglamento (UE) 2023/1697, que actualiza el
  Reglamento (UE) 1301/2014 — rangos de tensión, gálibo del pantógrafo
- **Orden TMA/135/2023** (IFI + IFE): apartado 4.1.2.2.1.x — altura mínima de
  diseño, fuerza de contacto (60–90 N), gradiente y desviación lateral del hilo
- **UNE-EN 50163**: tensiones de alimentación de los sistemas de tracción
  (3 kV: 2.000–3.600 V; 25 kV: 17.500–27.500 V)
- **UNE-EN 50119:2010 / 2021**: línea aérea de contacto — distancias de
  aislamiento (cuadro 3.7), diseño y viento
- **UNE-EN 50367**: compatibilidad pantógrafo–LAC (auscultación dinámica)
- **EN 15273-3:2013**: gálibo de implantación de obstáculos (salientes,
  cuasiestáticos, aleatorios)
- **NAE 107** (2ª ed. + M1, ene 2024): parámetros de la LAC, tablas 1–12, Anejo 2
  (fichas de catenarias), §4.1.1 (tensiones de diseño), §4.1.2 (auscultación),
  §4.2.2.8 (gálibo del poste)
- **NAE 300** (CA-160/3kV) y **NAE 301** (CA-220/3kV): composición, vanos,
  seccionamientos, alimentación (feeders 2× Cu 235 mm²), retorno, aisladores
  (tabla 33: 25 kV → fuga ≥ 1.200 mm, impulso 200 kV, industrial 95 kV)
- **NAE 302** (CA-160H / CA-200H): diseño transformable a 25 kV, distancias de
  25 kV, postes X-AV, desgaste máximo del hilo 30 %
- **ET 03.364.150.7**: seccionadores unipolares de catenaria (aislador C4-250,
  fuga ≥ 1.160 mm; niveles 200/220 kV impulso, 95/110 kV industrial)
- **ET 03.359.104.1**: rectificadores 3,3 kV CC (3.000/6.000 kW, 12 pulsos)
- **ET 03.359.110.8**: gestor de protecciones 3,3 kV (coordinación de SETs
  colaterales y puesta en paralelo)
- **ET 03.359.501**: subestaciones de tracción de CA (25 kV)
- Módulos 1 a 5 de este curso (lecciones 1 a 13): fórmulas y valores de origen

---

*Fin del Módulo 6 · Lección 1. La lección cierra el curso: de la ley de Ohm al
gálibo del pantógrafo y a la selección de la catenaria de alta velocidad, toda
decisión se defiende con la pirámide normativa del Módulo 0.*
