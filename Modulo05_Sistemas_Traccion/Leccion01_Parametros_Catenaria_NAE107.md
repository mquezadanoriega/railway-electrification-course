# MÓDULO 5 · LECCIÓN 1
# LOS PARÁMETROS DE LA LÍNEA AÉREA DE CONTACTO (CATENARIA)

## NAE 107 — Definición y medida de parámetros de la LAC

> **Documento base:** NAE 107, «Definición y medida de parámetros de la Línea Aérea
> de Contacto (catenaria)», 2ª edición (ene 2023) + M1 (ene 2024), 53 págs.
> Grupo de trabajo GT-300 · Aprobada por el Comité de Normativa (24-ene-2024).
> Deroga la NAE 107 2ª ed. de enero 2023.

---

## 1. RESULTADO DE APRENDIZAJE

Al terminar esta lección serás capaz de:

1. Listar los **parámetros funcionales** que fijan el sistema de alimentación (tensión, velocidad, pantógrafos)
2. Definir y aplicar los **parámetros geométricos y mecánicos** de diseño (altura, pendiente, vano, descentramiento, gálibo del poste…)
3. Distinguir entre **distancia de aislamiento estática y dinámica**, y entre **fase–tierra** y **fase–fase**
4. Interpretar la **ficha de una catenaria** (Anejo 2) para seleccionar el tipo adecuado a una velocidad y sistema
5. Conocer dónde buscar cada dato de diseño dentro de la norma (apartado exacto)

---

## 2. RESUMEN EJECUTIVO

La NAE 107 es el **diccionario de la catenaria de Adif**: define cada parámetro, fija
sus valores de diseño y establece cómo se mide en campo. Es la norma que **interconecta**
todos los demás documentos: de ella salen los valores que se introducen en el diseño
(NAE 300/301/302), en los gálibos (FOM/1630/2015) y en la verificación (IFE / ETI ENE).

La norma organiza los parámetros en dos grandes familias:

| Familia | Qué define | Apartados |
|---------|-----------|-----------|
| **Funcionales** | Tensión, velocidad máxima, pantógrafos, condiciones ambientales | 4.1 |
| **De diseño** | Composición, geometría/mecánica, dinámica, aislamiento | 4.2 |

> **Regla de diseño:** la NAE 107 da los **valores nominales** (p. ej. vano máximo,
> altura del sistema, descentramiento). El caso concreto de cada línea se cierra con
> las **normas de diseño funcional** (NAE 300/301/302) y las **especificaciones de
> material** (ET 03.364.xxx).

---

## 3. DATOS CLAVE — PARÁMETROS FUNCIONALES (4.1)

### 3.1. Tensión de alimentación (4.1.1) — Tabla 1 y diseño Adif

| Sistema | Umin2 (V) | Umin1 (V) | Un (V) | Umax1 (V) | Umax2 (V) |
|---------|-----------|-----------|--------|-----------|-----------|
| CC 1,5 kV (valores medios) | 1000 | 1500 | **1500** | 1800 | 1950 |
| CC 3 kV (valores medios) | 2000 | 3000 | **3000** | 3600 | 3900 |
| CA 25 kV (valores eficaces) | 17500 | 19000 | **25000** | 27500 | 29000 |

> **Valores de diseño Adif (M1 ene 2024, apartado 4.1.1):** tensión permanente por
> diseño en salida de subestación = **3.300 V** (CC), **1.650 V** (CC 1,5 kV) y
> **27.500 V** (CA). Dentro de los rangos de la tabla 1 de UNE-EN 50163.

### 3.2. Velocidad máxima por diseño (4.1.2)

- Determina las **características geométricas del trazado** en proyecto.
- Se valida con **auscultación dinámica** verificando los requisitos de la **UNE-EN 50367**.
- **Excepción:** hasta **120 km/h en CA** y **160 km/h en CC** la velocidad máxima puede
  fijarse **sin auscultación dinámica**, mediante medición de la geometría de la LAC.

### 3.3. Pantógrafos admisibles (4.1.3) — Tabla 2

| Tipo de electrificación | Pantógrafos admisibles |
|-------------------------|------------------------|
| 3 kV | 1950 mm (*) |
| 3 kV transformable a 25 kV | 1950 mm + 1600 mm |
| 25 kV | 1950 mm + 1600 mm (excepcionalmente solo 1600 mm) |
| 1,5 kV | 1700 mm (excepcionalmente 1700 + 1950 mm) |

(*) Excepcionalmente se admiten pantógrafos de **1860 mm** (UNE-EN 50367).

Para cada pantógrafo admisible debe verificarse en diseño, proyecto y obra:
- Desviación lateral máxima de los hilos (UNE-EN 50119 y 50367)
- Diseño de agujas aéreas según desvío (NAE 115, NAE 117)
- Gálibo de implantación, mecánico y eléctrico (Instrucción de Gálibos / NAG 5-1-0.0)

### 3.4. Condiciones ambientales de diseño (4.1.4)

| Condición | Valor de diseño |
|-----------|-----------------|
| **Temperatura ambiente** (4.1.4.1) | mín. media **−15 ºC** · máx. media **+45 ºC** (ajuste regional con datos AEMET, 50 años) |
| **Temp. máx. conductores** (4.1.4.2) | ver tabla siguiente |
| **Viento estructural** (4.1.4.3) | **120 km/h (33,3 m/s)**, período de retorno 50 años, metodología UNE-EN 50119 apdo. 6 |
| **Viento funcional** (desviación lateral del hilo) | **26 / 27 / 29 m/s**, retorno 10 años, según zona (mapa Anejo I NAE 300/301/302); UNE-EN 50119 apdo. 6.2.4 y UNE-EN 50367 apdo. 4.2 |
| **Sobrecargas de hielo** (4.1.4.4) | según altitud, tabla siguiente |

**Temperatura máxima de los conductores (Tabla 4):**

| Tipo conductor | Máx. permanente | Máx. hasta 30 min (pantógrafo en reposo) |
|----------------|-----------------|------------------------------------------|
| Sustentador / feeder de Cu ETP | **80 ºC** | — |
| Sustentador de Bz II | **100 ºC** | — |
| Feeder de aluminio–acero | **80 ºC** | — |
| Hilo contacto Cu ETP | **100 ºC** | 120 ºC |
| Hilo contacto CuAg 0,1 | **100 ºC** | 150 ºC |
| Hilo contacto CuMg 0,5 | **100 ºC** | 150 ºC |

**Cargas de hielo por altitud (Tabla 5):**

| Altitud (m) | Hielo en sustentador y otros cables (N/m) | Hielo en hilos de contacto (N/m) |
|-------------|-------------------------------------------|----------------------------------|
| 0 – 499 | 0 | 0 |
| 500 – 1000 | 3,5 | 1,75 |
| 1001 – 1500 | 7 | 3,5 |
| > 1500 | 15 | 7,5 |

> Para estructuras solo se considera el hielo sobre conductores/cables (se desprecia el
> acumulado sobre las propias estructuras).

---

## 4. DATOS CLAVE — PARÁMETROS DE DISEÑO (4.2)

### 4.1. Composición de la catenaria (4.2.1)

La composición **debe ser única en un cantón** (excepción: vías secundarias o curvas de
radio reducido, con tense reducido). Define:

- **Sustentador:** sección (mm²), material, tense (kgf y daN)
- **Hilos de contacto:** nº de hilos, sección, ranura (B general, A excepcional) y forma
  (C circular, F ovalado/aplanado), material según UNE-EN 50149, tense
- **Péndolas:** sección, material, tipología (equipotencial de lazo, recta o varilla)
- **Péndola en Y** (falso sustentador): sección, material, tense

**Identificación de hilos (UNE-EN 50149):** ranuras en el lóbulo superior —
CuETP: ninguna · CuAg 0,1: dos · CuCd: una · CuMg: tres · CuSn: una.
Diámetros de hilo: 107 → 12,08–12,4 mm · 120 → 12,69–13,01 mm · 150 → 14,3–14,7 mm.

**Identificación de sustentadores (diámetro exterior D):** Bz-70 ≈ 10,5 mm ·
Cu-95 ≈ 12,6 mm · Cu-150 ≈ 15,7 mm · Cu-185 ≈ 17,6 mm.

### 4.2. Altura de los hilos de contacto (4.2.2.1) — Tabla 6

| | Ancho métrico (1,5 kV) | 3 kV y 25 kV (V ≤ 220) | 25 kV (V > 220) |
|---|---|---|---|
| **Altura nominal** | 4750 mm | **5300 mm** | 5300 mm |
| **Altura mínima de diseño** | Variable* | Variable* | **5080 mm** |
| **Altura máxima de diseño** | 5500 mm | **6000 mm** | 5300 mm |

(*) Cálculo con metodología UNE-EN 50119 y apartado **4.1.2.2.1.4 de la IFE**.
**Tolerancia de montaje: ±10 mm** (el sistema de medida no debe superar esta tolerancia).

### 4.3. Pendiente y variación de pendiente (4.2.2.2) — Tabla 7

| Velocidad (km/h) | Pendiente (‰) | Variación de pendiente (‰) |
|------------------|---------------|----------------------------|
| 50 | 25 | 12,5 |
| 60 | 20 | 10 |
| 100 | 6 | 3 |
| 120 | 4 | 2 |
| 160 | 2 | 1 |
| 200 | 1 | 0,5 |
| 250 | 1 | 0,5 |
| > 250 | 0,4 | 0,2 |

Si no se alcanzan: cumplir al menos los valores de la **tabla 12 de UNE-EN 50119**.
*(El término "gradiente" de UNE-EN 50119 equivale a "pendiente".)*

### 4.4. Altura del sistema de catenaria (4.2.2.3) — Tabla 8

| Zona | Altura nominal |
|------|----------------|
| Trayectos y estaciones | **1400 mm** |
| Seccionamientos | Variable (según tipología LAC) |
| Gálibo reducido (túneles, pasos superiores…) | Variable (según tipología LAC) |

Tolerancia general **±10 mm**. Las transiciones de altura se hacen intercalando
transiciones. Se adecúa el vano para respetar la longitud mínima de péndola.

### 4.5. Descentramiento (4.2.2.4) — Tabla 9

Criterio de signos: **+d** = hacia fuera del poste/pendolón · **−d** = hacia el poste/pendolón.
En pórticos funiculares y catenaria rígida: referencia = kilometración (derecha positiva).

| Trazado | Catenaria elástica ancho estándar | Catenaria elástica ancho mixto | Catenaria rígida |
|---------|----------------------------------|-------------------------------|------------------|
| Recta | **+20 / −20 cm** | **+25 / −13,4 cm** | +30 / −30 cm |
| Curva | **+20 / +20 cm** | **+25 / +25 cm** | +30 / +30 cm |

Tolerancia de medida: ±3 cm. En doble hilo se mide al intereje de los hilos.
> Para el caso concreto se recalcula con el vano máximo, radio, desplazamiento por
> viento y gálibo del pantógrafo. En curvas de radio elevado pueden admitirse
> descentramientos tipo recta.

### 4.6. Vano (4.2.2.5)

- Definición: distancia entre dos **puntos de atirantado** consecutivos.
- Vano máximo según tipo de catenaria: **entre 60 y 65 m**.
- Factores que lo reducen en un tramo: altura del sistema, radio de curva, tense,
  viento, gálibo del pantógrafo.
- Dos criterios de cálculo: **altura de catenaria y péndola mínima** (en centro de
  vano) y **desplazamiento lateral máximo del hilo** (descentramiento + vano + radio
  + gálibo; siempre > desplazamiento por viento).

### 4.7. Cantón de compensación mecánica (4.2.2.6)

- Longitud máxima: **1200 – 1320 m** según tipología; semicantones: **600 – 700 m**.
- Influida por: rango del equipo de compensación, fuerzas de giro de ménsula (nº de
  vanos, descentramiento, distancia poste-eje), tense según resistencia del conductor,
  dilatación del hilo por temperatura (longitud y ubicación de ménsulas, temperatura
  nominal de ajuste), radio de curva, viento, rango de temperatura, diseño del conjunto.

### 4.8. Flecha de los hilos de contacto (4.2.2.7)

- Definición: distancia vertical entre la línea virtual que une dos atirantados y la
  altura del hilo por debajo de ella.
- La **flecha inicial** es un parámetro de diseño (entrada al cálculo de péndolas, NAE 116)
  que compensa las diferentes elasticidades del atirantado y centro de vano.
- Flechas superiores a la inicial = **degradación** que debe corregirse.
- Valores por tipología: ver fichas (apartado 6).

### 4.9. Gálibo del poste (4.2.2.8) — Tabla 10

| Ancho de vía | Gálibo–tecnología LAC | Dist. poste–carril (m) | Dist. poste–eje vía (m) |
|--------------|-----------------------|------------------------|-------------------------|
| Ancho métrico | GEE10, ménsulas celosía CA-160 | Recta 1,70 / Curva 1,90 | Recta 2,50 / Curva 2,70 |
| Ancho ibérico | GEB16, ménsulas celosía CA-160 | Recta 1,90 / Curva 2,10 | Recta 3,00 / Curva 3,20 |
| Ancho ibérico | GEB16, ménsulas tubulares | 2,15 | 3,25 |
| Ancho ibérico | GEC16, ménsulas tubulares | 2,35 | 3,35 |
| Ancho estándar | GC, ménsulas tubulares | 2,35 | 3,35 |

- Valores **nominales de diseño** a respetar en proyectos y replanteos.
- Tolerancia total tras aplomar el poste: **+20 / −20 cm en recta** y **+20 / −10 cm en curva**.
- Medida: de cara interior del poste a cara exterior de la cabeza del carril, al nivel del
  plano medio de rodadura; **cinta no conductora en CC** (no ocupar el circuito de vía).
- Conversión a poste–eje vía: poste–carril + semiancho del poste + semiancho de vía +
  anchura de cabeza de carril (~70 mm).

### 4.10. Seccionamientos (4.2.2.9)

| Parámetro | Valor / criterio |
|-----------|------------------|
| Solape entre catenarias | **0 – 20 m** en estática (dinámica mayor); depende del tráfico |
| Separación entre catenarias | Distancia de aislamiento de la catenaria (normas de cada tipología) |
| Elevación en semieje | Fijada por diseño del vano (peso, tense, vano) y distancia de aislamiento del seccionamiento |

Tipos: **lámina de aire** (aislados; en CA: fase–tierra o **zona neutra** fase–fase) y
**de cantón** (eléctricamente unidos).

### 4.11. Punto de aguja (4.2.2.10)

- Lugar donde se ubica el poste/apoyo del montaje de la aguja aérea (NAE 115, NAE 117).
- Agujas cruzadas: entre **P30 y P50**; tangenciales: entre **P80 y P100**.
- P se mide como distancia (cm) entre caras del mismo lado de carriles homólogos
  (directa y desviada): p. ej. 90 cm → "aguja en el punto 90 (P-90)".

### 4.12. Tensiones de regulación mecánica (4.2.2.11)

- Sistemas: **poleas y contrapesos** o **muelles** lineales/helicoidales.
- Todos los valores de tense y peso admiten **tolerancia del 5 %**.

```
Tense real = Peso del conjunto de contrapesos × Razón de regulación de las poleas × Rendimiento
```

- Razón de regulación de poleas: **1:5 y 1:3**; rendimiento según ensayo de la
  ET 03.364.103.6. En equipos de muelle: placa de características.

---

## 5. DATOS CLAVE — PARÁMETROS DINÁMICOS Y DE AISLAMIENTO

### 5.1. Elevación dinámica en el brazo de atirantado, S0 (4.2.3.1)

- Elevación (calculada/simulada/medida) del hilo en un brazo de atirantado en condiciones
  normales, con el límite superior de Fm a Vmáx.
- Si el brazo limita físicamente la elevación: espacio admisible **1,5·S0** (UNE-EN 50119
  apdo. 5.10.2); en caso contrario hasta **2·S0**.
- Valor propio de cada tipología (ver fichas, apartado 6).

### 5.2. Elasticidad (4.2.3.2)

- mm/N: elevación del hilo por la fuerza del pantógrafo; estática a V=0.
- Debe ser **reducida y uniforme** a lo largo del vano.
- Para reducirla: **limitar la longitud del vano** y **aumentar el tense** de los conductores.

### 5.3. Distancias de aislamiento (4.2.4)

**5.3.1. Fase–tierra (4.2.4.1) — Tabla 11 (tabla 2 de UNE-EN 50119):**

| Tensión | Estática (mm) | Dinámica (mm) |
|---------|---------------|---------------|
| CC 1,5 kV | **100** | **50** |
| CC 3,0 kV | **150** | **50** |
| CA 25 kV | **270** | **150** |

Reglas de aplicación:
- Se aplican **desde el gálibo mecánico del pantógrafo** (apdo. 3.5.2 de la Instrucción de Gálibos).
- En curva: **estática en el lado interior**, **dinámica en el lado exterior** (3.5.2.1).
- En recta, estación o parada operacional: envolvente de (gálibo mecánico a Vmáx + dinámica)
  y (gálibo mecánico a V=0 + estática). Sin parada operacional: solo gálibo a Vmáx + dinámica.
- Feeder sobre paso superior: con apoyo → estática entre paso superior y feeder; sin apoyo →
  estática en reposo y dinámica con viento/presión del tren (Figs. 14–16).
- En seccionamientos de lámina de aire: todo punto entre catenarias debe garantizar la
  estática fase–tierra.

**5.3.2. Fase–fase en CA (4.2.4.2) — Tabla 12 (tabla 3 de UNE-EN 50119):**

| Tensión nominal (kV) | Desfase (º) | Tensión relativa (kV) | Estática (mm) | Dinámica (mm) |
|----------------------|-------------|-----------------------|---------------|---------------|
| 25 | 120 | 43,3 | **400** | 230 |
| 25 | 180 | 50 | **540** | 300 |

- En sistema con autotransformador: desfase **180°** entre feeder negativo (−25 kV) y LAC (+25 kV).
- **Diseño obligatorio:** en zonas neutras el desfase entre tensiones adyacentes **no debe
  superar 120°**, evitando un 180° entre las dos catenarias de una lámina de aire.
- Zona neutra: mantener **400 mm** estáticos en todo el desarrollo y en la elevación.
- En túneles y pasos superiores con feeder negativo desnudo: **540 mm** entre puntos +25 kV
  y el feeder −25 kV.

---

## 6. LAS FICHAS DE CATENARIAS (ANEJO 2)

Fichas de catenarias certificadas / en certificación / normalizadas. La composición es
**única en un cantón**. Se muestran las de diseño más comunes:

### 6.1. Tabla maestra — conductores y tense

| Catenaria | V (kV) | Vmax (km/h) | Pantógrafos (mm) | Hilo de contacto | Sustentador | Ménsula | Poste (dist. poste-carril / poste-eje vía) |
|-----------|--------|-------------|------------------|------------------|-------------|---------|---------------------------------------------|
| CA-160/3kV TIPO A | 3 | 160 | 1950 | BC-107 CuETP · 2×107 mm² · 1050 kgf (1029 daN) | Cu ETP 150 mm² · 1425 kgf (1397 daN) | Perfiles acero | X/Z · 1,90 / 3,00 (IB) |
| CA-160/3kV TIPO B | 3 | 160 | 1950 | BC-120 CuAg0,1 · 2×120 mm² · 1200 kgf (1176 daN) | Cu ETP 150 mm² · 1425 kgf (1397 daN) | Perfiles acero | X/Z · 1,90 / 3,00 (IB) |
| CA-160H/3kV | 3 | 160 | 1950 | BC-120 CuAg0,1 · 2×120 mm² · 1200 kgf (1176 daN) | Cu ETP 150 mm² · 1425 kgf (1397 daN) | Tubular aluminio | XR/Z/Z-AV · 2,15 / 3,25 (IB) |
| CA-200H/3kV | 3 | 200 | 1950 | BC-120 CuAg0,1 · 2×120 mm² · 1500 kgf (1470 daN) | Cu ETP 150 mm² · 1650 kgf (1618 daN) | Tubular aluminio | XR/Z/X-AV · 2,15 / 3,25 (IB) |
| CA-220/3kV | 3 | 200 | 1950 | BC-150 CuAg0,1 · 2×150 mm² · 1875 kgf (1839 daN) | Cu ETP 185 mm² · 2475 kgf (2428 daN) | Perfiles acero | XR/Z · 1,90 / 3,00 (IB) |
| CA-160/3kV TIPO AM | 1,5 | 160 | 1750 | BC-107 CuETP · 2×107 mm² · 1050 kgf (1029 daN) | Cu ETP 150 mm² · 1425 kgf (1397 daN) | Perfiles acero | X/Z · 1,70 / 2,50 (AM) |
| CA-200/25kV | 25 | 200 | 1600/1950 | BC-120 CuAg0,1 · **1×120 mm²** · 1575 kgf (1545 daN) | Cu ETP 95 mm² · 1575 kgf (1543 daN) | Tubular aluminio | X-AV · 2,15 / 3,25 |
| CA-220/25kV | 25 | 220 | 1600/1950 | BC-150 CuAg0,1 · **1×150 mm²** · 1875 kgf (1837 daN) | Cu ETP 95 mm² · 1575 kgf (1543 daN) | Tubular aluminio | X-AV · 2,15 / 3,25 |
| CA-160H/25kV | 25 | 160 | 1600/1950 | BC-120 CuAg0,1 · 2×120 mm² · 1200 kgf (1176 daN) | Cu ETP 150 mm² · 1425 kgf (1397 daN) | Tubular aluminio | XR/Z/Z-AV · 2,15 / 3,25 |
| CA-200H/25kV | 25 | 200 | 1600/1950 | BC-120 CuAg0,1 · 2×120 mm² · 1500 kgf (1470 daN) | Cu ETP 150 mm² · 1650 kgf (1617 daN) | Tubular aluminio | XR/Z/X-AV · 2,15 / 3,25 |
| C-350 | 25 | 350 | 1600/1950 | BC-150 **CuMg0,5** · 1×150 mm² · 3150 kgf (3087 daN) | Cu ETP 95 mm² · 1575 kgf (1543 daN) | Tubular aluminio | X-AV · 2,35 / 3,35 (AE) |
| C-350-TR-250 | 25 | 250 | 1600/1950 | BC-150 CuMg0,5 · 1×150 mm² · 2100 kgf (2058 daN) | Cu ETP 95 mm² · 1575 kgf (1543 daN) | Tubular aluminio | X-AV · 2,35 / 3,35 (AE) |
| C-350-TR-200 | 25 | 200 | 1600/1950 | BC-150 CuMg0,5 · 1×150 mm² · 1575 kgf (1543 daN) | Cu ETP 95 mm² · 1575 kgf (1543 daN) | Tubular aluminio | X-AV · 2,35 / 3,35 (AE) |
| SICAT H1.0 | 25 | 330 | 1600/1950 | AC-120 CuMg0,5 · 1×150 mm² · 2753 kgf (2700 daN) | Cu ETP 95 mm² · 2142 kgf (2100 daN) | Tubular aluminio | X-AV · 2,55 / 3,70 (AE) |

Péndolas típicas: equipotenciales por parejas CuETP 25 mm² (cat. 3 kV y H 25 kV);
equipotenciales de lazo Bz II 16 mm² (CA-200/220 25 kV y C-350). Péndola en Y (falso
sustentador) solo en C-350 (Bz II 35 mm², 18 m, 350 daN), C-350-TR-250 (308,7 daN) y
SICAT H1.0 (Bz II 25 mm², 22 m, 350 daN).

### 6.2. Tabla maestra — geometría, seccionamientos y dinámica

| Catenaria | Vano máx. (m) | Alt. sistema (mm) | Flecha (‰) | Descentr. (±cm) | Alt. nominal / máx. (mm) | Separ. comp. (mm) | Lámina aire F–T (mm) | Lámina aire F–F (mm) | S0 (mm) | fs (mm) |
|-----------|---------------|-------------------|------------|-----------------|--------------------------|-------------------|----------------------|----------------------|---------|---------|
| CA-160/3kV A | 60 | 1400 | 0,6 | 20 | 5300 / 6000 | 250 | 300 | — | 67 | 98 |
| CA-160/3kV B | 60 | 1400 | 0,6 | 20 | 5300 / 6000 | 250 | 300 | — | 61 | 89 |
| CA-160H/3kV | 60 | 1400 | 0,6 | 20 | 5300 / 6000 | 250 | 400 | — | 60 | 91 |
| CA-200H/3kV | 60 | 1400 | 0,5 | 20 | 5300 / 6000 | 250 | 400 | — | 55 | 68 |
| CA-220/3kV | 60 | 1400 | 0,5 | 20 | 5300 / 6000 | 250 | 400 | — | 41 | 42 |
| CA-160/3kV AM | 60 | 1400 | 0,6 | 20 | 4750 / 5000 | 200 | 300 | — | 67 | 98 |
| CA-200/25kV | 60 | 1400 | 0,4 | 20 | 5300 / 6000 | 250 | 300 | 400 | 46 | 78 |
| CA-220/25kV | 60 | 1400 | 0,4 | 20 | 5300 / 6000 | 200 | 450 | 450 | 43 | 77 |
| CA-160H/25kV | 60 | 1400 | 0,6 | 20 | 5300 / 6000 | 250 | 300 | 400 | 34 | 55 |
| CA-200H/25kV | 60 | 1400 | 0,5 | 20 | 5300 / 6000 | 250 | 300 | 400 | 35 | 48 |
| C-350 | 64 | 1400 | 0 | 20 | 5300 / 5300 | 200 | 400 | 450 | 110 | 134 |
| C-350-TR-250 | 64 | 1400 | 0 | 20 | 5300 / 5300 | 200 | 450 | 450 | 95,5 | 128 |
| C-350-TR-200 | 60 | 1400 | 0,4 | 20 | 5300 / 5300 | 200 | 450 | 450 | 43 | 87 |
| SICAT H1.0 | 65 | **1600** | 0 | **30** | 5300 / 5300 | 200 | 450 | 450 | 94,9 | 125 |

> Notas de lectura:
> - La **CA-160/3kV AM** (ancho métrico, 1,5 kV) es la única que usa altura nominal 4750 mm
>   y pantógrafo 1750 mm.
> - **CA-220/3kV**: el nombre hace referencia al sistema de diseño, aunque su Vmax es 200 km/h.
> - Las C-350 / SICAT H1.0 (AV) tienen **flecha 0 ‰** y **altura máxima = nominal (5300 mm)**:
>   el hilo se mantiene plano, con S0 y fs elevados por la dinámica de alta velocidad.
> - A mayor velocidad → menor flecha, menor S0 en catenarias H (compensadas), mayores
>   separaciones de seccionamiento y mayores tenses de hilo.

---

## 7. APLICACIÓN PRÁCTICA AL DISEÑO DE UNA VÍA

Secuencia de uso de la NAE 107 en un proyecto de electrificación:

1. **Fijar el sistema** (4.1.1): tensión 3 kV / 25 kV → define pantógrafos (tabla 2),
   distancias de aislamiento (tabla 11/12) y rangos de tensión.
2. **Fijar Vmáx** (4.1.2) → decide si hace falta auscultación dinámica (UNE-EN 50367).
3. **Elegir tipología** (Anejo 2): a cada velocidad le corresponde una catenaria de Adif.
   Verificar: vano máx., flecha, S0/fs, altura nominal, descentramiento.
4. **Verificar gálibos** (4.2.2.8, 4.2.4): distancia poste–carril vs gálibo de
   implantación; distancias de aislamiento respecto a obstáculos y en seccionamientos.
5. **Verificar condiciones ambientales** (4.1.4): temperatura → cantón de compensación
   (4.2.2.6); viento → vanos y estructuras; hielo → carga sobre conductores y altura mínima.
6. **Comprobar pendientes y alturas** (4.2.2.1–4.2.2.3): altura nominal ±10 mm, pendiente
   según velocidad (tabla 7), altura de sistema 1400 mm.
7. **Proyectar seccionamientos y agujas** (4.2.2.9–4.2.2.10): solapes, separaciones,
   elevaciones, punto de aguja.

> **Ejemplo tipo:** línea de 160 km/h en 3 kV → CA-160/3kV TIPO A o B (BC-107 CuETP
> o BC-120 CuAg0,1). Hilo a 5300 mm (máx. 6000), altura de sistema 1400 mm, vano máx.
> 60 m, descentramiento ±20 cm, separación fase–tierra 300 mm, S0=67/61 mm, fs=98/89 mm.

---

## 8. PREGUNTAS DE AUTOEVALUACIÓN

1. ¿Cuáles son las tensiones permanentes de diseño en salida de subestación en CC 3 kV, CC 1,5 kV y CA 25 kV?
2. ¿Cuándo NO hace falta auscultación dinámica para fijar la velocidad máxima por diseño?
3. ¿Qué pantógrafos admisibles tiene una línea 3 kV transformable a 25 kV?
4. ¿Cuál es la temperatura máxima permanente del hilo de contacto CuAg 0,1? ¿Y a 30 min?
5. ¿Qué carga de hielo se aplica en sustentador a 800 m de altitud? ¿Y en hilo de contacto?
6. Altura nominal del hilo en una línea de 25 kV a 200 km/h, y altura mínima de diseño en una de 300 km/h.
7. ¿Cuál es la altura máxima de diseño del hilo en una línea de 3 kV? ¿Por qué difiere de una de 25 kV > 220 km/h?
8. Pendiente y variación de pendiente admisibles a 160 km/h.
9. Altura nominal del sistema de catenaria y su tolerancia.
10. Descentramiento en recta de catenaria elástica de ancho estándar (valores +/−).
11. ¿Entre qué límites está la longitud máxima de un cantón de compensación? ¿Y un semicantón?
12. ¿Qué es la flecha inicial del hilo de contacto y para qué se usa?
13. Distancia poste–carril y poste–eje vía para GEB16 con ménsulas tubulares (recta).
14. ¿Qué tolerancia total se admite al aplomar el poste en recta? ¿Y en curva?
15. ¿Cuál es la distancia de aislamiento estática fase–tierra en 25 kV? ¿Y la dinámica?
16. En una curva, ¿qué distancia de aislamiento se aplica en el lado interior y cuál en el exterior?
17. Distancia de aislamiento estática fase–fase para un desfase de 120° en 25 kV. ¿Y para 180°?
18. ¿Qué desfase máximo debe garantizarse entre tensiones adyacentes en una zona neutra?
19. Tensión mecánica (kgf y daN) del hilo de contacto de la CA-160/3kV TIPO A.
20. Vano máximo y flecha de la C-350. ¿Qué diferencia a la SICAT H1.0 en altura de sistema y descentramiento?
21. ¿Qué tres datos componen la identificación de un hilo de contacto según UNE-EN 50149?
22. ¿Qué diámetro exterior tiene aproximadamente un sustentador Cu-150?
23. Fórmula del tense real en un equipo de poleas y contrapesos. ¿Qué razones de regulación existen?
24. ¿Entre qué puntos se ubican habitualmente las agujas cruzadas? ¿Y las tangenciales?
25. ¿Qué parámetros dinámicos (S0 y fs) tiene la CA-200/25kV y cuál es su separación fase–fase?

---

## 9. REFERENCIAS

- **NAE 107** (2ª ed. + M1, ene 2024): apartados 4.1–4.2, tablas 1–12, Anejo 2 (fichas)
- UNE-EN 50163: tensiones de alimentación de redes de tracción
- UNE-EN 50119:2021: línea aérea de contacto — diseño, aislamiento, viento, péndolas
- UNE-EN 50367:2022: compatibilidad pantógrafo–LAC (auscultación dinámica)
- UNE-EN 50149:2012: hilos de contacto acanalados (identificación de ranuras)
- Instrucción Ferroviaria de Gálibos (FOM/1630/2015), apdos. 3.5, 3.5.2, 3.5.2.1
- IFE (TMA/135/2023), apdo. 4.1.2.2.1.4 (altura mínima de diseño)
- NAE 300/301/302 (diseño funcional CA-160 / CA-220 / CA-160H-CA-200H): ver Lección 2
- ET 03.364.103.6: conjuntos de poleas para electrificación

---

*Lección 2: Diseño funcional de catenarias — NAE 300 (CA-160/3kV), NAE 301
(CA-220/3kV) y NAE 302 (CA-160H / CA-200H).*
