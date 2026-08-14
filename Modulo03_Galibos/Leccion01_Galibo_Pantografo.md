# MÓDULO 3 · LECCIÓN 1
# EL GÁLIBO DEL PANTÓGRAFO

## Instrucción Ferroviaria de Gálibos — Orden FOM/1630/2015

> **Documento base:** BOE-A-2015-8765, Orden FOM/1630/2015, de 14 de julio,
> «Instrucción ferroviaria de gálibos».
> **Secciones:** 3.5 (gálibo del pantógrafo), 2.5 (cálculo en material rodante),
> anejo 7 (ejemplos de cálculo).

---

## 1. RESULTADO DE APRENDIZAJE

Al terminar esta lección serás capaz de:

1. Explicar por qué el gálibo del pantógrafo se divide en **mecánico** y **eléctrico**
2. Determinar si un obstáculo debe respetar uno, otro o ambos gálibos
3. Calcular la **anchura** y la **altura** del gálibo mecánico del pantógrafo
4. Aplicar la **distancia de aislamiento eléctrico** según la tensión de la catenaria
5. Saber dónde se consulta en la norma (apartado exacto) cada dato de diseño

---

## 2. RESUMEN EJECUTIVO

El gálibo del pantógrafo es el espacio libre que debe garantizar la infraestructura
alrededor del pantógrafo en **posición de captación** (levantado y en contacto con el
hilo de contacto). No es un único gálibo: son **dos**, con lógica distinta:

| Gálibo | Qué protege | Qué lo define |
|--------|-------------|---------------|
| **Mecánico** | Interferencias físicas (choque) | La envolvente del pantógrafo + sus desplazamientos |
| **Eléctrico** | Interferencias eléctricas (arco/descarga) | Distancia de aislamiento según tensión + condiciones del obstáculo |

**Regla de oro para el diseñador:** el gálibo a exigir a cada obstáculo depende de
cómo esté ese obstáculo conectado eléctricamente:

| Tipo de obstáculo | Gálibo que debe respetar |
|-------------------|--------------------------|
| A la **misma tensión** que la LAC | Solo el **mecánico** |
| **Aislado** de tierra | Solo el **mecánico** |
| **No aislado** (a tierra o a potencial distinto) | **Mecánico + eléctrico** |

> Esto explica por qué los postes metálicos (a tierra) exigen más distancia a la
> catenaria que las estructuras aisladas, y por qué el diseño de los brazos de
> atirantado se juega en esta distancia.

---

## 3. DATOS CLAVE (MEMORIZAR)

### 3.1. Semiancho de la mesilla del pantógrafo — Cuadro 3.5

| Ancho mesilla (mm) | Tensión de catenaria | Semiancho bw (mm) |
|--------------------|----------------------|-------------------|
| 1.700 | 1,5 kV c.c. | **850** |
| 1.950 | 3,0 kV c.c. | **975** |
| 1.950 | 25 kV c.a. | **975** |
| 1.600 | 25 kV c.a. | **800** |

> **Nota de la norma:** el ancho de 1.600 mm no se admite en líneas de 3,0 kV por
> incompatibilidad con el diseño de la catenaria.

**Interpretación:** la mesilla de 1.950 mm es la estándar en España para 3 kV y 25 kV.
El ancho del gálibo mecánico será, como mínimo, el doble del semiancho + márgenes.

### 3.2. Distancias de aislamiento eléctrico — Cuadro 3.7 (UNE-EN 50119:2010)

| Tensión de catenaria | Estática (mm) | Dinámica (mm) |
|----------------------|---------------|---------------|
| 1,5 kV c.c. | **100** | **50** |
| 3,0 kV c.c. | **150** | **50** |
| 25 kV c.a. | **270** | **150** |

**Cómo se usa:**
- **Estática** → lado **interior** de la curva (el obstáculo más próximo a la mesilla)
- **Dinámica** → lado **exterior** de la curva

### 3.3. Elevaciones del hilo de contacto — Cuadro 3.6 (fs y fws+fwa)

Valores para el cálculo de la **altura** del gálibo mecánico:

| Tipo catenaria | Vmax (km/h) | Elasticidad centro/apoyo (mm/N) | fws+fwa (mm) |
|----------------|-------------|-------------------------------|--------------|
| CA-160 | 160 | 0,65 / 0,32 | 70 |
| CAU-220 | 220 | 0,38 / 0,19 | 70 |
| CA-220 | 220 | 0,37 / 0,25 | 70 |
| SICAT H 1.0 | 330 | 0,44 / 0,40 | 70 |
| EAC-350 | 350 | 0,45 / 0,38 | 70 |

> **Catenaria rígida** (a falta de datos específicos): fs = **15 mm**; fws+fwa = **70 mm**.

---

## 4. CÓMO SE CALCULA

### 4.1. Anchura del gálibo mecánico

Distancia horizontal mínima del obstáculo al eje del pantógrafo:

- **Lado interior:** `b_w + e_p + S'_i + qs'_i + j'`
- **Lado exterior:** `b_w + e_p + S'_a + qs'_a + j'`

| Símbolo | Significado |
|---------|-------------|
| `bw` | Semiancho de la mesilla (cuadro 3.5) |
| `ep` | Desplazamiento lateral del pantógrafo (a h'0 usa epo; a h'u usa epu) |
| `S'i, S'a` | Salientes del pantógrafo en curva (interior/exterior) |
| `qs'i, qs'a` | Desplazamientos cuasiestáticos por balanceo del vehículo |
| `j'` | Margen de desplazamientos aleatorios laterales (vía, peralte, disimetrías, oscilaciones) — valor cuadrático medio × K' |

Los desplazamientos aleatorios se combinan como **media cuadrática** (no suma simple),
por la escasa probabilidad de que ocurran todos a la vez.

### 4.2. Altura del gálibo mecánico

```
h_pantógrafo = h_f + f_s + f_ws + f_wa
```

| Símbolo | Significado |
|---------|-------------|
| `hf` | Altura del hilo de contacto (dato de diseño de la catenaria) |
| `fs` | Elevación del hilo por la fuerza ascendente F del pantógrafo |
| `fws` | Elevación del arco por la flexibilidad del pantógrafo |
| `fwa` | Elevación del arco por el desgaste de la pletina/frotador |

> El gálibo se verifica en dos alturas: **h'0 (máxima)** y **h'u (mínima)** de
> verificación, interpolando linealmente entre ambas.

### 4.3. Gálibo eléctrico

Se obtiene a partir del **mecánico**:

- **Anchura:** `b_elect = b_mec + b_elec − cw` (donde `cw` = proyección horizontal del
  trocador aislado; si no hay trocador, cw = 0)
- **Altura:** `h_elect = h_mec + b_elec`

Solo se consideran las **partes no aisladas** del pantógrafo (no cuenta el trocador aislado).

---

## 5. CÁLCULO RESUELTO (25 kV, CA-160H)

> Ejemplo completo, resuelto con los datos de la norma. El desarrollo íntegro y sus
> criterios de decisión se repiten y amplían en el Módulo 6, Caso 1 (3 kV); este
> ejemplo aporta la variante de **25 kV c.a.** con catenaria híbrida.

### 5.1. Datos

| Parámetro | Valor | Origen |
|-----------|-------|--------|
| Sistema / catenaria | **25 kV c.a.** · CA-160H/25kV | NAE 302 (Módulo 5, lección 2) |
| Mesilla del pantógrafo | 1.950 mm → **bw = 975 mm** | Cuadro 3.5 (25 kV) |
| Altura de verificación | h'0 = 6,5 m → **ep = 170 mm**; h'u = 5 m → **ep = 110 mm** | FOM/1630/2015, 3.10.4.2 |
| Vehículo | Longitud 26 m; centros de bogies L = 19 m; batalla n = 3 m | Hipótesis del caso |
| Curva de estudio | R = 1.200 m; insuficiencia de peralte I = 120 mm | Hipótesis del caso |
| Coeficiente de balanceo | s'0 = 0,225 | FOM/1630/2015, 3.10.4.2 |
| Altura del hilo | hf = 5.300 mm | NAE 302, tabla 5 |
| Elevación por la fuerza F | **fs = 55 mm** (a Vmáx) | NAE 302 (Módulo 5, lección 2) |
| Flexibilidad + desgaste | fws + fwa = 70 mm | Cuadro 3.6 |
| Distancia de aislamiento 25 kV | Estática **270 mm** / dinámica **150 mm** | Cuadro 3.7 · UNE-EN 50119 |
| Trocador aislado | cw = 0 | FOM/1630/2015, 3.5.2 |
| Margen de aleatorios | j' = 50 mm (media cuadrática × K', K' = 1) | FOM/1630/2015, anejo 7 |

### 5.2. Paso 1 — Salientes por inscripción en curva (R = 1.200 m)

```
S'i = (19² − 3²) / (8 · 1200) = 352 / 9.600 = 0,0367 m ≈ 37 mm
S'a = (26² − 19²) / (8 · 1200) = 315 / 9.600 = 0,0328 m ≈ 33 mm
```

### 5.3. Paso 2 — Semiancho del gálibo mecánico (a h'0 = 6,5 m, ep = 170 mm)

El cuasiestático `qs'` se obtiene por el procedimiento de EN 15273-3 a partir de
s'0 = 0,225 e I = 120 mm: **qs' ≈ 90 mm** (a I = 100 mm resulta 75 mm, como en el
Módulo 6, lección 1, caso 1).

```
Recta:          b_mec = 975 + 170 + 0 + 0 + 50 = 1.195 mm
Curva interior: b_mec = 975 + 170 + 37 + 90 + 50 = 1.322 mm
Curva exterior: b_mec = 975 + 170 + 33 + 90 + 50 = 1.318 mm
```

### 5.4. Paso 3 — Gálibo eléctrico (25 kV, cw = 0)

En curva: estática (270 mm) al **interior**, dinámica (150 mm) al **exterior**.
En recta se aplica la estática (hipótesis dominante a V = 0).

```
Recta:          b_elect = 1.195 + 270 − 0 = 1.465 mm
Curva interior: b_elect = 1.322 + 270 − 0 = 1.592 mm
Curva exterior: b_elect = 1.318 + 150 − 0 = 1.468 mm
```

### 5.5. Paso 4 — Alturas del gálibo

```
h_mec   = hf + fs + fws + fwa = 5.300 + 55 + 70 = 5.425 mm
h_elect = h_mec + belec       = 5.425 + 270     = 5.695 mm ≤ 6.500 mm ✓
```

### 5.6. Paso 5 — Verificación a la altura mínima h'u = 5 m

Con ep = 110 mm y el hilo a 5.000 mm de altura de verificación:

```
b_mec (recta, h'u) = 975 + 110 + 50 = 1.135 mm  → menos restrictivo que a h'0
h_mec (h'u)        = 5.000 + 55 + 70 = 5.125 mm → h_elect = 5.395 mm ≤ 6.500 mm ✓
```

La verificación a **h'0 = 6,5 m es la dominante** (mayor ep y mayor hf).

### 5.7. Resumen

| Magnitud | Recta | Curva interior | Curva exterior |
|----------|-------|----------------|----------------|
| Semiancho mecánico `b_mec` | 1.195 mm | 1.322 mm | 1.318 mm |
| **Semigálibo eléctrico `b_elect`** | **1.465 mm** | **1.592 mm** | **1.468 mm** |
| Altura del gálibo `h_elect` | 5.695 mm | 5.695 mm | 5.695 mm |

> La catenaria **híbrida** se verifica con distancias de **25 kV** (270/150 mm) aun
> explotándose en 3 kV: así el gálibo queda preparado para la transformación futura,
> como exige la IFE para las electrificaciones nuevas de 3 kV (Módulo 4, lección 1).

---

## 6. APLICACIÓN PRÁCTICA AL DISEÑO DE UNA VÍA

En el diseño de la electrificación, este gálibo condiciona:

1. **La altura de montaje del hilo de contacto** sobre el plano de rodadura
   (interfiere con el gálibo de la infraestructura)
2. **La posición de los postes y estructuras** en la plataforma (deben estar fuera
   del gálibo mecánico o eléctrico según su conexión)
3. **Los elementos próximos:** pórticos, biondas, pantallas antiruido, carteles —
   todo lo que se sitúe sobre el gálibo del pantógrafo debe comprobarse
4. **Los túneles** — el gálibo del pantógrafo en posición de captación define la
   sección mínima del túnel bajo la catenaria
5. **La interoperabilidad** — la ETI de Energía exige respetar el gálibo del
   pantógrafo definido para la línea; un pantógrafo más ancho que el gálibo de la
   línea no puede circular

---

## 7. PREGUNTAS DE AUTOEVALUACIÓN

1. ¿Por qué un poste metálico debe respetar el gálibo eléctrico y una estructura aislada no?
2. ¿Cuál es la distancia de aislamiento eléctrico **estática** en una línea de 25 kV c.a.?
3. ¿Qué semiancho de mesilla se usa para 3,0 kV c.c.?
4. ¿Por qué no se permite la mesilla de 1.600 mm en líneas de 3 kV?
5. ¿Qué se considera al calcular la **altura** del gálibo mecánico además de la altura del hilo?
6. ¿En qué lado de la curva se usa la distancia de aislamiento estática y por qué?
7. ¿Qué representa `cw` en el gálibo eléctrico y cuándo vale 0?

---

## 8. REFERENCIAS

- Orden FOM/1630/2015, Instrucción Ferroviaria de Gálibos — apartados 3.5, 3.5.1, 3.5.2, 2.5, anejo 7
- UNE-EN 50119:2010 — Aplicaciones ferroviarias. Instalaciones fijas. Líneas aéreas de contacto
- ETI de Energía (TSI ENE) — gálibo del pantógrafo (se verá en el Módulo 4)
- NAE 107 — parámetros de la LAC (interrelación con la altura del hilo)

---

*Próxima lección: Gálibo de implantación de obstáculos (apartados 3.1–3.4) y
distancia entre ejes de vías (apartado 3.6).*
