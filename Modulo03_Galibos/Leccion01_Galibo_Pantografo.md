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

## 5. APLICACIÓN PRÁCTICA AL DISEÑO DE UNA VÍA

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

## 6. PREGUNTAS DE AUTOEVALUACIÓN

1. ¿Por qué un poste metálico debe respetar el gálibo eléctrico y una estructura aislada no?
2. ¿Cuál es la distancia de aislamiento eléctrico **estática** en una línea de 25 kV c.a.?
3. ¿Qué semiancho de mesilla se usa para 3,0 kV c.c.?
4. ¿Por qué no se permite la mesilla de 1.600 mm en líneas de 3 kV?
5. ¿Qué se considera al calcular la **altura** del gálibo mecánico además de la altura del hilo?
6. ¿En qué lado de la curva se usa la distancia de aislamiento estática y por qué?
7. ¿Qué representa `cw` en el gálibo eléctrico y cuándo vale 0?

---

## 7. REFERENCIAS

- Orden FOM/1630/2015, Instrucción Ferroviaria de Gálibos — apartados 3.5, 3.5.1, 3.5.2, 2.5, anejo 7
- UNE-EN 50119:2010 — Aplicaciones ferroviarias. Instalaciones fijas. Líneas aéreas de contacto
- ETI de Energía (TSI ENE) — gálibo del pantógrafo (se verá en el Módulo 4)
- NAE 107 — parámetros de la LAC (interrelación con la altura del hilo)

---

*Próxima lección: Gálibo de implantación de obstáculos (apartados 3.1–3.4) y
distancia entre ejes de vías (apartado 3.6).*
