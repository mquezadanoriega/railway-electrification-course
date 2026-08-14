# MÓDULO 6 · LECCIÓN 2
# CASO COMPLETO: DISEÑO DE LA CATENARIA DESDE UN TRAZADO

## Integra el flujo de diseño funcional (Módulo 5, lección 2) con los gálibos
## (Módulo 3), la IFE (Módulo 4) y las cimentaciones (Módulo 2, lección 2)

> **Enfoque:** se parte de un **trazado real** (alineaciones, radios, peralte, aparato de
> vía, túnel) y se recorre la **secuencia de diseño funcional** de las NAE 300/301/302.
> El objetivo es **identificar correctamente cuándo se elige de catálogo y cuándo se
> dispara un cálculo específico** — el alumno debe saber reconocer estos casos, aunque no
> ejecute el cálculo estructural.

---

## 1. RESULTADO DE APRENDIZAJE

Al terminar esta lección serás capaz de:

1. Leer un trazado y extraer los datos de diseño de la LAC (sistema, familia, alturas,
   vanos por radio, descentramientos, cantón de compensación)
2. Calcular el **gálibo del pantógrafo** (mecánico y eléctrico) en los puntos singulares
   de un trazado (recta, curva, túnel) y decidir si la infraestructura lo respeta
3. Comprobar la **desviación lateral del hilo** frente al viento y conocer cuándo entra
   en juego el apéndice E de la IFE
4. Seleccionar **poste y macizo de catálogo** por función, verificando el momento límite
   de servicio (MLS)
5. **Detectar los puntos del trazado que requieren cálculo específico** (poste, macizo,
   pendolado) y justificarlo con la norma aplicable

---

## 2. DATOS DE PARTIDA

Se proyecta la electrificación de un tramo de **vía única de ancho ibérico**, 12 km,
**v = 160 km/h**, alimentado en **3 kV c.c.** como prolongación de la red existente, con
**compromiso de transformación futura a 25 kV c.a.** (por ello se aplican desde el
proyecto las hipótesis de la IFE para electrificaciones nuevas de 3 kV: distancias de
aislamiento de 25 kV y familia **híbrida**). El trazado es:

| PK | Alineación | Datos |
|----|-----------|-------|
| 0+000 – 5+000 | Recta | Cantón de compensación en este tramo |
| 5+000 – 6+500 | Curva | **R = 3.000 m**, I = 120 mm |
| 6+500 – 8+000 | Recta | **Desvío a vía secundaria en PK 7+200** (aguja P-50) |
| 8+000 – 9+400 | Curva | **R = 800 m**, I = 120 mm |
| 9+400 – 9+650 | Túnel | Longitud 250 m, altura interior reducida |
| 9+650 – 12+000 | Recta | — |

**Hipótesis de proyecto:**

| Parámetro | Valor | Origen |
|-----------|-------|--------|
| Sistema / familia | **3 kV c.c. → 25 kV** · **CA-160H/3kV** (transformable) | IFE 4.1.2.2.1 · NAE 302 |
| Altura nominal del hilo | **5.300 mm** | NAE 302, tabla 5 |
| Altura máxima / mínima de diseño | 6.000 mm / según gálibo (IFE 4.1.2.2.1.4) | NAE 302 · IFE |
| Altura de sistema | 1.400 mm | NAE 302 |
| Viento estructural / funcional | 120 km/h / **29 m/s** (zona costera, anejo I) | NAE 302 |
| Pantógrafo de proyecto | 1.950 mm (estándar 3 kV y 25 kV) | FOM/1630/2015, cuadro 3.5 |
| Terreno | Tipo (C₀ = 6 daN/m³, γt = 1400 daN/m³, tanα = 0,005, σlat = 1 daN/cm²) **salvo tramo 8+000–9+400 con arcilla blanda** | NAE 106, anejo III |

---

## 3. PASO 1 — SISTEMA, FAMILIA Y ALTURAS DEL HILO

**Decisión:** al ser 3 kV c.c. con transformación futura a 25 kV, se adopta la
**CA-160H/3kV** (NAE 302). Las catenarias híbridas se diseñan ya con:
- Distancias de aislamiento de **25 kV** (fase–tierra 270/150 mm; fase–fase 120° 400/230 mm).
- Conductores que **no cambian** al transformar (2×120 mm² CuAg0,1).
- Alturas mínimas de la variante **25 kV** desde el proyecto (NAE 302, 5.2).

**Alturas:** nominal **5.300 mm**; en el túnel se reduce a **5.100 mm** (ver Pasos 2 y 6).
La altura mínima de diseño debe cumplir la IFE (≥ 5.080 mm para v ≥ 250 km/h; en v < 250
se calcula según 4.1.2.2.1.4).

---

## 4. PASO 2 — GÁLIBO DEL PANTÓGRAFO EN LOS PUNTOS SINGULARES

Se aplica la metodología del Módulo 3, lección 1 (§5, cálculo resuelto) con los datos
del vehículo: longitud 26 m, centros de bogies 19 m, batalla 3 m, s'0 = 0,225,
j' = 50 mm. Al ser la línea **diseñada para 25 kV**, se usan las distancias de
aislamiento **estática 270 mm / dinámica 150 mm**.

**Curva R = 3.000 m** (a h'0 = 6,5 m, ep = 170 mm):

```
S'i = (19² − 3²) / (8 · 3000) = 352 / 24.000 ≈ 15 mm
S'a = (26² − 19²) / (8 · 3000) = 315 / 24.000 ≈ 13 mm
qs' (I = 120 mm) ≈ 90 mm

b_mec interior = 975 + 170 + 15 + 90 + 50 = 1.300 mm
b_mec exterior = 975 + 170 + 13 + 90 + 50 = 1.298 mm
b_elect interior = 1.300 + 270 = 1.570 mm
b_elect exterior = 1.298 + 150 = 1.448 mm
```

**Curva R = 800 m** (caso dominante):

```
S'i = 352 / 6.400 ≈ 55 mm ;  S'a = 315 / 6.400 ≈ 49 mm
b_mec interior = 975 + 170 + 55 + 90 + 50 = 1.340 mm
b_elect interior = 1.340 + 270 = 1.610 mm
```

**Túnel (hilo a 5.100 mm):**

```
h_mec   = 5.100 + 55 + 70 = 5.225 mm   (fs = 55 mm, fws+fwa = 70 mm)
h_elect = 5.225 + 270    = 5.495 mm ≤ 6.500 mm ✓  (y ≥ 5.080 mm de mínima de diseño ✓)
```

**Verificación de implantación:** los postes en ancho ibérico con gálibo GEB16 se sitúan
a **3,00 m** del eje en recta y **3,20 m** en curva (NAE 107, tabla 10) ≫ 1.610 mm → el
gálibo eléctrico **cabe** con holgura. La **caja del tren** (semiancho 1.500 mm) queda
también dentro.

**Decisión:** el gálibo del pantógrafo es **CORRECTO** en todos los puntos singulares
del trazado (criterios del Módulo 6, lección 1, caso 1).

---

## 5. PASO 3 — DESVIACIÓN LATERAL DEL HILO POR VIENTO

Con **viento funcional 29 m/s** (retorno 10 años), las tablas de la NAE 302 ya garantizan
la desviación lateral admisible (IFE: **550 mm** con pantógrafo de 1.950 mm) en vanos y
descentramientos **dentro de tabla**:

| Parámetro | Recta | R = 3.000 m | R = 800 m |
|-----------|-------|-------------|-----------|
| Vano máximo (NAE 302, tablas 15–18, pant. 1600 mm, viento 29 m/s) | **60 m** | 60 m | **45 m** |
| Descentramiento | **+20 / −20 cm** | **+15 / +15 cm** | **+20 / +20 cm** |

> Las tablas de vanos y descentramientos de las NAE 300/301/302 están **calculadas** con
> la metodología del apéndice E de la IFE (fuerza del viento por UNE-EN 50119 §6.2.4 y
> UNE-EN 50367 §4.2). Mientras el punto se mantenga dentro de sus hipótesis (radio,
> altitud, pantógrafo, viento), **no se recalcula la desviación**: se aplica la tabla.

**Punto que dispara verificación específica:** el **desvío a vía secundaria (aguja P-50)
en PK 7+200** introduce vanos y descentramientos **no tabulados** en el aparato de vía;
allí debe comprobarse la desviación lateral según el **apéndice E de la IFE** y el
replanteo de la aguja según **NAE 115** (ver Paso 6).

---

## 6. PASO 4 — CANTÓN DE COMPENSACIÓN Y SECCIONAMIENTOS

- **Cantón de compensación:** 1.200 m en recta (NAE 302, 5.2) = **20 vanos de 60 m** en el
  tramo 0+000–5+000. Puntos fijos cada cantón con colas de anclaje.
- **Seccionamiento de cantón:** se prevé en recta (p. ej. en PK 4+800) para aislar el
  tramo en caso de actuación; la configuración se toma del **anejo de seccionamientos**
  de la NAE 302 (4 vanos en general, 3 solo con vano ≥ 55 m).
- **Aguja P-50:** sección de aguja según NAE 115 (lección 4 del Módulo 5), con su
  alimentación y aisladores de sección.

---

## 7. PASO 5 — SELECCIÓN DE POSTES Y MACIZOS DE CATÁLOGO

Para cada apoyo se determina la **función** y se elige el **poste de catálogo** con su
**MLS** (momento límite de servicio) y su **macizo** del anejo III (NAE 300/301/302),
verificando que la solicitación del punto no supera el MLS:

| Función del apoyo | Poste | MLS (daN·m) | Macizo desmonte | Macizo terraplén | Armadura |
|-------------------|-------|-------------|-----------------|------------------|----------|
| Suspensión simple | XR2 | 6.829 | d5 / Cd1 | t8 / t9 / Ct1 | ARM-2 · Ø25 |
| Suspensión + feeder de refuerzo | XR3 | 8.074 | d6 / Cd2 | t9 / t10 / Ct2 | ARM-2 · Ø25 |
| Seccionamiento de cantón (seccionador) | XR4E | 8.528 | d7 / Cd2 | t9 / t10 / Ct2 | ARM-2 · Ø25 |
| Anclaje de compensación (colas de cantón) | Z3 | 10.263 | d8 / Cd2 | t10 / t11 / Ct3 | ARM-2 · Ø25 |
| Anclaje de aguja / semieje | Z2 | 8.858 | d7 / Cd2 | t9 / t10 / Ct2 | ARM-2 · Ø25 |
| Aguja de vía general en ancho ibérico | (aguja aérea P-50) | — | — | — | NAE 115 |

> Valores tomados del anejo III de la CA-220 (lección 2 del Módulo 5, tabla de
> cimentaciones). El procedimiento es idéntico con el anejo correspondiente de la NAE 302;
> en el proyecto real se usan las tablas de la familia proyectada.

**Regla aplicada:** mientras la solicitación (viento 29 m/s, tense de la CA-160H, 2 hilos
de contacto, feeder si procede, aguja) **no supere el MLS**, el poste y su macizo son
**de catálogo**: no se calcula, se planta la solución tabulada.

---

## 8. PASO 6 — DETECCIÓN DE CASOS QUE REQUIEREN CÁLCULO ESPECÍFICO

En este trazado concreto se detectan **cuatro casos** que **salen de catálogo** y exigen
memoria de cálculo específico en el proyecto:

| # | Punto del trazado | Motivo | Cálculo requerido (identificar, no ejecutar) |
|---|-------------------|--------|----------------------------------------------|
| 1 | **PK 9+400–9+650 (túnel)** | Hilo reducido a 5.100 mm y vanos no tabulados en túnel | Recálculo del **pendolado** según NAE 116; verificación de **gálibo** (hecho en Paso 2) y de **carga de hielo** con Ktun (IFE 4.1.2.2.1.4) |
| 2 | **PK 7+200 (aguja P-50 sobre recta)** | Vanos y descentramientos del aparato de vía **no tabulados** | Cálculo de **desviación lateral** (IFE apéndice E) y replanteo de **aguja** (NAE 115); pendolado específico |
| 3 | **PK 8+000–9+400 (arcilla blanda)** | Terreno **distinto** de la hipótesis del anejo III (C₀ ≠ 6 daN/m³) | **Recálculo del macizo** según NAE 106 (o cimentación especial); los macizos de catálogo no son válidos |
| 4 | **R = 800 m con vano forzado > 45 m** (si un obstáculo impide colocar el apoyo) | Vano o radio **fuera de tabla** | Justificación con **cálculo de desviación lateral** y verificación de captación; si el poste resultante supera el MLS de la familia → **poste especial** |

> **Caso adicional de comprobación rápida (no presente en el trazado):** si el tramo con
> feeder doble o pórtico exigiera un momento > 33.053 daN·m (Z6bis, la mayor de la
> familia), no existiría poste de catálogo y se proyectaría un **poste especial** con
> cálculo de esfuerzos propio (ET 03.364.101.0).

**Regla de oro:** el proyecto tipo de Adif **ya calculó** postes, macizos, vanos y
pendolado. El diseñador elige de catálogo mientras no cambien las hipótesis (radio,
vano, viento, altitud, terreno, pantógrafo). **Cada desviación de hipótesis que se
detecte en el trazado se convierte en un cálculo específico que el proyecto debe
justificar por escrito.**

---

## 9. TABLA RESUMEN DE DECISIONES

| Decisión | Solución | Normativa aplicada |
|----------|----------|--------------------|
| Sistema / familia | **3 kV c.c. transformable** → **CA-160H/3kV** | IFE 4.1.2.2.1 · NAE 302 |
| Altura del hilo | 5.300 mm nominal; **5.100 mm** en túnel | NAE 302 · IFE 4.1.2.2.1.4 |
| Gálibo del pantógrafo | **CORRECTO** (b_elect máx. 1.610 mm en R = 800; h_elect 5.495 mm en túnel) | FOM/1630/2015 · Mod. 3 L1 · Mod. 6 L1 |
| Vano / descentramiento | 60 m y +20/−20 (recta) · 60 m y +15/+15 (R = 3000) · 45 m y +20/+20 (R = 800) | NAE 302, tablas 13–18 |
| Desviación lateral | Dentro de tabla en alineaciones; **verificación específica en aguja y vanos forzados** | IFE 4.1.2.2.1.2 y apéndice E |
| Cantón de compensación | 1.200 m = 20 vanos de 60 m | NAE 302 |
| Postes / macizos | XR2/XR3/XR4E/Z2/Z3 con su macizo de catálogo | NAE 302 · NAE 106 (anejo III) |
| **Cálculos específicos** | 4 casos detectados (túnel, aguja, arcilla, vano forzado) | NAE 116 · NAE 106 · NAE 115 · IFE apéndice E · ET 03.364.101.0 |

---

## 10. PREGUNTAS DE AUTOEVALUACIÓN

1. ¿Por qué se elige una familia **híbrida** para una electrificación nueva de 3 kV c.c.?
2. ¿Qué distancias de aislamiento se aplican al calcular el gálibo del pantógrafo de esta
   línea, y por qué no las de 3 kV?
3. En la curva de R = 800 m, ¿cuál es el vano máximo y el descentramiento de catálogo?
4. ¿Qué punto del trazado dispara la verificación de la **desviación lateral** por el
   apéndice E de la IFE, y por qué?
5. ¿Qué poste y qué macizo seleccionarías para un **seccionamiento de cantón**? ¿Y para
   una **colas de anclaje de compensación**?
6. ¿Por qué el tramo de **arcilla blanda** invalida el macizo de catálogo? ¿Qué norma
   obliga a recalcularlo?
7. Enumera los **casos de cálculo específico** detectados en este trazado y la norma que
   los exige.
8. ¿Qué ocurriría si un pórtico exigiera un momento mayor que el de la mayor familia de
   postes (Z6bis, 33.053 daN·m)?

---

## 11. REFERENCIAS

- **NAE 302** (2ª ed., dic 2024): CA-160H/CA-200H — composición, alturas, vanos y
  descentramientos (tablas 13–18), cantón, seccionamientos, postes X-AV
- **NAE 300 / NAE 301** (2ª ed., jun 2024): anejos III (cimentaciones) y IV (seccionamientos)
- **NAE 106** (2ª ed., jun 2017): ejecución de macizos; hipótesis del anejo III y casos de
  salida de catálogo (lección 2 del Módulo 2)
- **NAE 115**: agujas aéreas P-50/P-90 (lección 4 del Módulo 5)
- **NAE 116**: pendolado — tablas de referencia; caso particular → cálculo específico
- **IFE (Orden TMA/135/2023)** 4.1.2.2.1.1–4.1.2.2.1.4 y **apéndice E**: desviación
  lateral, altura mínima, gradiente, hielo
- **Orden FOM/1630/2015**: gálibo del pantógrafo (3.5) y gálibos de implantación (3.10–3.11)
- **UNE-EN 50119:2021** (§6.2.4 viento) y **UNE-EN 50367** (§4.2 desviación)
- **ET 03.364.101.0**: estructuras metálicas de soporte (familias, MLS, validación)
- Módulos 2, 3, 4 y 5 de este curso (lecciones de referencia indicadas en cada paso)

---

*Fin del Módulo 6 · Lección 2. Complementa la lección 1 (casos resueltos) con el
recorrido completo del diseño de la catenaria desde un trazado real y la detección de los
cálculos específicos.*
