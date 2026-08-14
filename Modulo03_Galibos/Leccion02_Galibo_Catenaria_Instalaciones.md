# MÓDULO 3 · LECCIÓN 2
# GÁLIBO DE LA LÍNEA DE CONTACTO Y DE LAS INSTALACIONES

## Documento base

> Orden FOM/1630/2015, de 14 de julio, «Instrucción ferroviaria de gálibos» (BOE-A-2015-8765).
> **Secciones:** 1.3 (gálibos considerados), 3.1 (gálibos de implantación de obstáculos),
> 3.2 (reglas asociadas), 3.3 (gálibo límite), 3.4 (gálibo nominal), 3.5 (gálibo del pantógrafo),
> 3.7 (gálibo en elementos específicos), 3.10–3.12 (aplicación a anchos de vía), anejos 3 y 7.
> **Norma de referencia:** EN 15273-3:2013 (implantación de obstáculos), EN 15273-2:2013
> (contornos de referencia), UNE-EN 50119:2010 (distancias de aislamiento).

---

## 1. RESULTADO DE APRENDIZAJE

Al terminar esta lección serás capaz de:

1. Explicar qué es el **gálibo de implantación de obstáculos** y distinguir sus tres tipos
   (límite, nominal y uniforme) según la Orden FOM/1630/2015
2. Relacionar la **altura de la catenaria** (`hf`) con el gálibo del pantógrafo visto en la
   Lección 1, y con las alturas de verificación `h'0` y `h'u`
3. Conocer las **elevaciones del hilo de contacto** (`fs`, `fws+fwa`) que define la orden
   para cada tipo de catenaria
4. Situar correctamente **andenes, paseos, muelles, aceras de evacuación y elementos de obra**
   respecto al gálibo límite, nominal y uniforme
5. Aplicar los **valores numéricos** de la instrucción: distancias de borde de andén a eje de
   vía, entreejes nominales y márgenes complementarios `M3b` y `M3h`
6. Saber dónde se consulta en la norma cada dato (apartado y cuadro exactos)

---

## 2. RESUMEN EJECUTIVO

La Orden FOM/1630/2015 **no define un "gálibo de catenaria" independiente**: lo que define es
el **gálibo de implantación de obstáculos** (el espacio en torno a la vía que no debe ser
invadido por obstáculos ni por vehículos de vías adyacentes) y, dentro de él, todo lo que
afecta a la línea aérea de contacto (LAC) y a las instalaciones próximas a la vía.

La relación entre ambos es la siguiente:

| Elemento | Cómo lo trata la orden | Apartado |
|----------|------------------------|----------|
| **Línea aérea de contacto** | Indirectamente: el gálibo del pantógrafo (Lección 1) y la altura del hilo `hf` condicionan la altura de montaje | 3.5 |
| **Postes, pórticos e instalaciones** | Son "obstáculos": deben respetar el gálibo de implantación de obstáculos (límite, nominal o uniforme) | 3.1–3.4 |
| **Andenes, pasillos, paseos, muelles** | "Elementos específicos" con reglas propias | 3.7 |
| **Obras autorizadas** | Elementos permanentes/provisionales con exigencias distintas | 3.7.7 |
| **Distancia entre vías** | Entreeje límite y nominal | 3.6, 3.10.5–3.12.5 |

**Idea clave:** en la filosofía de la instrucción, la catenaria se cuelga de estructuras
(postes, pórticos, ménsulas) que son a su vez obstáculos de implantación. Por tanto, el diseño
de la electrificación debe **dejar libre el gálibo del pantógrafo** (mecánico y eléctrico) y,
al mismo tiempo, **no invadir el gálibo de implantación de obstáculos** con las propias
estructuras de sustentación.

---

## 3. EL GÁLIBO DE LA LÍNEA AÉREA DE CONTACTO

### 3.1. La altura del hilo de contacto (`hf`)

La instrucción trata la catenaria desde el punto de vista del **pantógrafo en posición de
captación**. El parámetro de partida del cálculo es la **altura del hilo de contacto** (`hf`),
definida como la altura medida sobre el plano de rodadura (apartado 3.5.1.3).

Como el pantógrafo está en **contacto permanente** con el hilo, su altura varía continuamente
con la del hilo. La orden no fija un valor único de `hf`, sino que exige verificar el gálibo en
dos alturas límite:

| Ancho de vía | Altura máxima de verificación `h'0` | Altura mínima de verificación `h'u` | Apartado |
|--------------|-------------------------------------|-------------------------------------|----------|
| Ibérico (1.668 mm) | **6,5 m** | **5 m** | 3.10.4.2 |
| Estándar europeo (1.435 mm) | **6,5 m** | **5 m** | 3.11.4.2 |
| Métrico (1.000 mm) | **5,5 m** | **4,3 m** | 3.12.4.2 |

Entre ambas alturas, la variación del contorno de referencia del pantógrafo se considera
**lineal**, interpolando para alturas intermedias.

> El único valor de altura de montaje que aparece expresamente en la orden es el de **5,30 m**,
> en el anejo 3 (gálibos históricos): la figura A.3.3 representa el contorno de referencia del
> gálibo cinemático GE14 **para una altura del hilo de contacto de 5,30 m**.

### 3.2. Elevaciones del hilo y del arco del pantógrafo

La altura real que ocupa el pantógrafo sobre el hilo no es `hf`, sino:

```
h_pantógrafo = hf + fs + fws + fwa
```

| Símbolo | Significado | Valor por defecto (catenaria rígida) |
|---------|-------------|--------------------------------------|
| `hf` | Altura del hilo de contacto sobre el plano de rodadura | — (dato de diseño) |
| `fs` | Elevación del hilo por la fuerza ascendente F del pantógrafo | **15 mm** |
| `fws` | Elevación del arco por la flexibilidad del pantógrafo | — |
| `fwa` | Elevación del arco por el desgaste de la pletina/frotador | — |
| `fws+fwa` | Suma de ambas | **70 mm** |

### 3.3. Valores de `fs` y `fws+fwa` según el tipo de catenaria (cuadro 3.6)

La orden da los valores de `fs` (elevación del hilo) en función de la **fuerza de contacto**
`F` (media `Fm`, `Fm+3σmax`, máxima `Fmax`, estática `Fest`) y de la velocidad, para cinco tipos
de catenaria:

| Tipo de catenaria | Vmax (km/h) | Elasticidad centro/apoyo (mm/N) | fs centro vano (mm) — Fm y Vmax | fs apoyo (mm) — Fm y Vmax | fs (mm) — V=0 | fws+fwa (mm) |
|-------------------|-------------|--------------------------------|--------------------------------|---------------------------|---------------|--------------|
| CA-160 | 160 | 0,65 / 0,32 | 120 | 88 | 44 | 70 |
| CAU-220 | 220 | 0,38 / 0,19 | 120 | 60 | 30 | 70 |
| CA-220 | 220 | 0,37 / 0,25 | 120 | 59 | 40 | 70 |
| SICAT H 1.0 | 330 | 0,44 / 0,40 | 90 | 78 | 71 | 70 |
| EAC-350 | 350 | 0,45 / 0,38 | 90 | 86 | 72 | 70 |

> El anejo 7 particulariza para la EAC-350: `fs = 162 mm` con V=Vmáx, `fs = 41 mm` con V=0,
> y `fws+fwa = 70 mm` (para las hipótesis del ejemplo, R=250 m, D=0,160 m, I=0,150 m).

**Conclusión de diseño:** la elevación del hilo depende de la **elasticidad de la catenaria** y
de la fuerza del pantógrafo; por eso la orden la da como dato en el cuadro 3.6 y no como
constante. Las catenarias rápidas (SICAT H 1.0, EAC-350) admiten fuerzas mayores
(`Fmax = 300 N`) con menores elevaciones.

### 3.4. La "zona de caza" del pantógrafo y su relación con la Lección 1

La Lección 1 introdujo el **gálibo mecánico** y el **gálibo eléctrico** del pantógrafo. La
lección 2 necesita ese resultado porque:

- **La anchura del gálibo mecánico** (Lección 1) define la distancia horizontal mínima a la que
  puede situarse cualquier estructura de sustentación de la catenaria respecto al eje del
  pantógrafo:
  - Lado interior de la curva: `b_obstáculo,i = b'w + ep + S'i + qs'i + j'`
  - Lado exterior de la curva: `b_obstáculo,a = b'w + ep + S'a + qs'a + j'`
- **La anchura del gálibo eléctrico** añade la distancia de aislamiento `belec` (cuadro 3.7):
  - Estática (lado interior): 100 mm (1,5 kV), 150 mm (3,0 kV), **270 mm (25 kV)**
  - Dinámica (lado exterior): 50 mm (1,5 y 3,0 kV), **150 mm (25 kV)**
- En **líneas existentes** se admite `cw = 0,2` (pantógrafos con trocadores aislados); en
  **líneas nuevas o acondicionadas** `cw = 0` (trocadores no aislados), que restringe más el
  espacio disponible para la infraestructura.

Los desplazamientos laterales máximos del pantógrafo que la orden fija para el cálculo son:

| Ancho | `epo` (a h'0) | `epu` (a h'u) | L (empate) | s'0 | h'c0 | D'0 = I'0 |
|-------|---------------|---------------|------------|-----|------|-----------|
| Ibérico | 0,170 m | 0,110 m | 1,733 m | 0,225 | 0,5 m | 1/15 ≈ 0,066 m |
| Estándar | 0,170 m | 0,110 m | 1,500 m | 0,225 | 0,5 m | 1/15 ≈ 0,066 m |
| Métrico | 0,150 m | 0,082 m | 1,055 m | 0,225 | 0,5 m | 0,07 m |

> **Relación con la Lección 1:** allí se calculó el gálibo del pantógrafo; aquí ese gálibo se
> convierte en **restricción de implantación** para postes, pórticos y soportes de la LAC.

---

## 4. GÁLIBO DE INFRAESTRUCTURA: ELEMENTOS PRÓXIMOS A LA VÍA

### 4.1. Partes altas y partes bajas

La orden divide el gálibo de implantación de obstáculos en dos partes, separadas por la cota
**h = 0,4 m** sobre el plano de rodadura:

- **Partes altas (h > 0,4 m):** aquí se aplican los márgenes complementarios `M3b` (laterales)
  y `M3h` (verticales) en los gálibos nominales.
- **Partes bajas (h ≤ 0,4 m):** sin márgenes complementarios; utilizan los gálibos de partes
  bajas **GI1/GI2/GI3** (ancho 1.435 mm) y **GEI1/GEI2/GEI3** (ancho 1.668 mm).

### 4.2. Qué gálibo se exige a cada tipo de línea (cuadros 1.2 y 1.3)

En partes altas, el gálibo uniforme de implantación de obstáculos exigido es:

| Tipo de línea | Ancho 1.435 mm | Ancho 1.668 mm |
|---------------|----------------|----------------|
| **Nuevas** | GC | GEC16 |
| **Acondicionadas** | GC (o GB si se justifica técnica y económicamente) | GEC16 (o GEB16) |
| **Ancho mixto (tres carriles)** | Envolvente de ambos anchos | Envolvente de ambos anchos |

En partes bajas:

| Tipo de línea | Ancho 1.435 mm | Ancho 1.668 mm |
|---------------|----------------|----------------|
| Apta para autopista ferroviaria | GI3 | GEI3 |
| No apta para autopista ferroviaria | GI2 | GEI2 |

> **Detalle:** las vías de las **estaciones de clasificación** se diseñarán para GI2/GEI2,
> salvo donde existan **frenos de vía**, donde se adoptará GI1/GEI1.
> En líneas de **ancho métrico**: gálibo uniforme **GEE10** (nuevas y acondicionadas), pudiéndose
> autorizar GED10 o mantener el gálibo existente.

### 4.3. Elementos específicos (apartado 3.7)

La orden dedica reglas propias a cada tipo de instalación próxima a la vía:

**Andenes (3.7.2)**
- Se situarán **fuera del gálibo límite de implantación de obstáculos**.
- Por encima del andén se dejará libre de obstáculos una banda de al menos **20 cm** (apertura
  de puertas, espejos retrovisores).
- No se colocarán andenes en los lados de vías donde esté prevista la circulación de
  transportes excepcionales.
- Altura del borde de andén (`hq`): **55, 68 o 76 cm** en ancho ibérico o estándar europeo;
  **105 cm** en ancho métrico.
- Con aparatos de vía en el andén, se verificará además el gálibo en aparatos de vía (3.7.1.2)
  y, si es necesario, se incrementará la separación.

**Pasillos de evacuación en túneles (3.7.3)**
- El borde de la acera se situará en el **límite del gálibo nominal** para la posición más
  desfavorable del peralte; excepcionalmente (con autorización de la Autoridad Ferroviaria)
  podrá respetar únicamente el **gálibo límite**.
- En túneles de **vía única** sin itinerario alternativo, solo se colocarán aceras por encima de
  la cota de carril y a un solo lado del túnel, salvo autorización en contrario.

**Paseos de servicio (3.7.4)**
- Se evitará la implantación de **instalaciones, fijas o provisionales**, u otros elementos que
  dificulten o impidan el paso de personas.

**Muelles (3.7.5)**
- No se colocarán junto a **vías generales o de circulación** ni junto a **vías con peralte**.
- El borde del muelle estará **fuera del gálibo límite de implantación de obstáculos**.

**Apeos de vía (3.7.6)**
- Al apear la vía (cajones empujados, cruces de tubos) se verificará el **gálibo de partes
  bajas** y las condiciones particulares de explotación.

**Obras autorizadas por el administrador de infraestructura (3.7.7)**
- **Elementos permanentes:** cumplirán con carácter general el **gálibo uniforme**.
- **Elementos provisionales:** cumplirán el **gálibo nominal**; si V ≤ 120 km/h podrán situarse
  verificando el **gálibo nominal sin resguardos**; excepcionalmente y debidamente justificado,
  el **gálibo límite**.

**Frenos de vía (3.8)**
- Pueden elevarse hasta **0,115/0,125 m** sobre el plano de rodadura a partir de x = **3 m** del
  final de un acuerdo convexo de Rv ≥ 250 m (ampliado a x = **5 m** en lomos de asno para
  ciertos vagones de transporte combinado) y en acuerdos cóncavos de Rv ≥ 300 m o sus
  proximidades.

### 4.4. Postes e instalaciones como obstáculos

Los **postes, pórticos, biondas, pantallas antiruido, carteles y demás elementos fijos** no
tienen regla propia en la instrucción: son "obstáculos" genéricos y deben respetar, según su
categoría, el gálibo uniforme, nominal o límite de implantación de obstáculos (apartado 1.3.2).
El espacio que dejan libre es el definido por las ampliaciones del apartado 3.2 (salientes,
cuasiestáticos, aleatorios y márgenes) aplicadas al contorno de referencia del gálibo
correspondiente.

---

## 5. VALORES NUMÉRICOS DE LA INSTRUCCIÓN

### 5.1. Distancia del borde de andén al eje de la vía

**Ancho ibérico (cuadro 3.15).** Hipótesis: sobreancho máximo 30 mm, D = Imax = 0,115 m, vía en
balasto en mal estado, andén vertical recto sin bordillo retranqueado.

| Altura del andén hq (mm) | Borde | R ≥ 5.000 m | 5.000 > R ≥ 1.000 m | 1.000 > R ≥ 250 m |
|--------------------------|-------|-------------|---------------------|-------------------|
| 760 | Exterior | 1.750 | 1.755 | 1.765 |
| 760 | Interior | 1.750 / 1.795 (D) | 1.755 / 1.800 (D) | 1.765 / 1.810 (D) |
| 680 | Exterior | 1.745 | 1.750 | 1.760 |
| 680 | Interior | 1.745 / 1.790 (D) | 1.750 / 1.790 (D) | 1.760 / 1.805 (D) |

(En el lado exterior con peralte se usa el valor sin peralte, por previsión de cambio a
peralte cero.)

**Ancho estándar europeo (cuadro 3.22).** Hipótesis: sobreancho máximo 30 mm, D = Imax =
0,100 m, vía en balasto en mal estado, andén vertical recto.

| Altura del andén hq (mm) | Borde | R ≥ 5.000 m | 5.000 > R ≥ 1.000 m | 1.000 > R ≥ 250 m |
|--------------------------|-------|-------------|---------------------|-------------------|
| 760 | Exterior | 1.675 | 1.680 | 1.690 |
| 760 | Interior | 1.675 / 1.720 (D) | 1.680 / 1.725 (D) | 1.690 / 1.735 (D) |
| 680 | Exterior | 1.670 | 1.675 | 1.685 |
| 680 | Interior | 1.670 / 1.715 (D) | 1.675 / 1.715 (D) | 1.685 / 1.730 (D) |

**Tolerancias en andenes (cuadros 3.16 y 3.23):**

| Actuación en vía | Tolerancia hq | Tolerancia Tq |
|------------------|---------------|---------------|
| Construcción, acondicionamiento o renovación | (0; −10) mm | 10 mm |
| Mantenimiento de vía | (0; −30) mm | 30 mm |

> En ancho métrico la distancia de borde de andén a eje de vía figura como **"punto abierto
> (pendiente de estudio)"** (apartado 3.12.6).

### 5.2. Distancia nominal entre ejes de vías (entreeje)

**Valores normales (cuadro 3.13):**

| Velocidad (km/h) | Entreeje nominal (mm) |
|------------------|-----------------------|
| Vmax ≤ 140 | 3.808 |
| 140 < Vmax ≤ 200 | 4.000 |
| 200 < Vmax < 250 | 4.300 |
| 250 ≤ Vmax ≤ 350 | 4.700 |

**Valores excepcionales (cuadro 3.14), con estudio específico:**

| Velocidad (km/h) | Entreeje nominal (mm) |
|------------------|-----------------------|
| Vmax ≤ 160 | 3.808 |
| 160 < Vmax ≤ 200 | 3.808 (ancho 1.435) / 3.920 (ancho 1.668 o mixto) |
| 200 < Vmax < 250 | 4.000 |
| 250 ≤ Vmax ≤ 300 | 4.300 |
| 300 < Vmax ≤ 350 | 4.500 |

> Con V ≤ 120 km/h se admite entreeje inferior a 3.808 mm si se demuestra que se cumple al
> menos el **entreeje límite** (apartado 3.10.5.1).

### 5.3. Márgenes complementarios de los gálibos nominales (apartado 3.11.1.4)

| Margen | Valor | Zona |
|--------|-------|------|
| `M3b` (lateral) | **0,200 m** | Puntos con h > 0,4 m |
| `M3b` | 0,200 m y 0 | En h = 0,4 m (discontinuidad del gálibo nominal) |
| `M3b` | 0 | Puntos con h < 0,4 m |
| `M3h` (vertical) | **0,150 m** | Puntos con h > 0,4 m |
| `M3h` | 0,150 m y 0 | En h = 0,4 m (discontinuidad) |
| `M3h` | 0 | Puntos con h < 0,4 m |

Estos márgenes cubren: incrementos de velocidad, transportes excepcionales, futuras
modificaciones de trazado o de gálibo, efectos aerodinámicos y vientos transversales y obras en
la vía (apartado 3.2.2.4). Solo se aplican en **partes altas**.

### 5.4. Semianchos de la mesilla del pantógrafo (cuadro 3.5)

| Ancho de la mesilla (mm) | Tensión de catenaria | Semiancho bw (mm) |
|--------------------------|----------------------|-------------------|
| 1.700 | 1,5 kV c.c. | 850 |
| 1.950 | 3,0 kV c.c. | 975 |
| 1.950 | 25 kV c.a. | 975 |
| 1.600 | 25 kV c.a. | 800 |

---

## 6. GÁLIBOS LÍMITE Y DE REFERENCIA SEGÚN EN 15273

### 6.1. Contornos de referencia considerados (cuadro 1.1)

| Tipos de gálibo | Ancho 1.668 mm | Ancho 1.435 mm | Ancho 1.000 mm |
|-----------------|----------------|----------------|----------------|
| Nuevos | GEA16, GEB16, GEC16 | GA, GB, GC | GED10, GEE10 |
| Históricos | GHE16, GEC14 | GC14 | — |

- **Siglas:** G (gálibo), H (histórico), E (español), A/B/C (envolvente del gálibo GA/GB/GC),
  y dos cifras = ancho de vía redondeado a decímetros. G1, GA, GB y GC son gálibos
  **interoperables europeos** (solo ancho estándar europeo); el contorno del **G1** se define
  en la norma **EN 15273-3:2013**.
- **Nota de la orden:** no se considera el gálibo GEA16, asimilado al GEB16 (difieren solo en
  110 mm en el intervalo 4.350–3.700 mm, diferencia cubierta por los márgenes de 200 mm del
  gálibo nominal).
- **Métrico:** E = eléctrico, D = diésel (GEE10 eléctrico, GED10 diésel).

### 6.2. Los tres gálibos de implantación (apartados 3.1, 3.3 y 3.4)

| Gálibo | Definición | Tratamiento de los desplazamientos aleatorios |
|--------|------------|------------------------------------------------|
| **Límite** | Espacio que no debe invadir ningún obstáculo en circunstancia alguna, con reserva para variaciones de la vía entre mantenimientos | K veces su **media cuadrática** (escasa probabilidad de concurrencia simultánea) |
| **Nominal** | Similar al límite, con márgenes para transportes excepcionales, incrementos de velocidad, etc. | Se **suman directamente** (mayor probabilidad de concurrencia) |
| **Uniforme** | Un único gálibo para toda la línea, envolvente de los nominales para parámetros suficientemente desfavorables | Según la hipótesis de la línea (figuras 3.26, 3.27, 3.31, 3.32, 3.35, 3.36) |

En el ejemplo del anejo 7 la orden aplica **K = 1,2** (salvo desplazamientos aleatorios
laterales para h < 0,5 m, donde K = 1) para el gálibo límite, y **K' = 1** para el gálibo del
pantógrafo.

### 6.3. Desplazamientos que amplían el contorno (apartado 3.2)

El semiancho del contorno de referencia se amplía con:

1. **Salientes** `Si`, `Sa` (inscripción en curva)
2. **Desplazamientos cuasiestáticos** `qs` (exceso o insuficiencia de peralte entre D0 y D, o
   entre I0 e I, para un coeficiente de flexibilidad `s0`); solo para h > hco
3. **Desplazamientos aleatorios (M1+M2)**: desplazamiento de la vía `Tvía`, desviaciones del
   peralte `TD`, disimetrías del vehículo `σ0`, oscilaciones `σosc`
4. **Márgenes complementarios `M3b`/`M3h`** (solo gálibo nominal, solo partes altas)

En vertical (partes altas): inscripción en acuerdos verticales `hRV`, desplazamientos
cuasiestáticos de puntos PT `hPT`, desplazamientos aleatorios y márgenes `M3h`. En partes bajas
(h ≤ 0,4 m) solo se aplican las reducciones correspondientes.

### 6.4. Vehículos de referencia (cuadros 3.17 y 3.30)

Para zonas de aparatos de vía o curvas de transición se usan vehículos de referencia con
semiancho de contorno `bCR`:

| Gálibo | hmin (mm) | bCR (mm) | bveh (mm) |
|--------|-----------|----------|-----------|
| GHE16 / GEC16 | 400 | 1.720 | 1.535 / 1.495 |
| GEB16 | 400 (3.320 máx.) | 1.720 | 1.535 / 1.495 / 1.600 |
| GEE10 / GED10 | 400 | 1.530 | 1.345 / 1.305 |

Estos vehículos condicionan los **salientes** en curvas de transición y aparatos de vía, y por
tanto el espacio que debe quedar libre para la implantación de postes y pórticos en esas zonas.

---

## 7. INTERACCIÓN CON EL DISEÑO DE LA CATENARIA (NAE 107/300/301) Y CON LA TSI ENE

### 7.1. Las catenarias citadas por la orden

La instrucción no diseña la catenaria, pero **usa sus parámetros como datos de entrada** en el
cálculo del gálibo. Los tipos que cita son los habituales de la red española:

- **CA-160, CA-220, CAU-220** — catenarias de ADIF para vías convencionales
- **SICAT H 1.0, EAC-350** — catenarias de alta velocidad
- **Catenaria rígida** — la orden recomienda valorar su instalación en electrificación de
  líneas existentes si facilita la implantación futura de los gálibos del cuadro 1.2
  (apartado 1.3.2); a falta de datos específicos, `fs = 15 mm` y `fws+fwa = 70 mm`

Los detalles de diseño de estas catenarias (tensionado, vanos, flechas, anclajes) no son objeto
de la Orden FOM/1630/2015: se desarrollan en la normativa técnica de ADIF (**NAE 107** para la
línea aérea de contacto y **NAE 300/301** de gálibos e implantación) y en la **ETI de Energía
(TSI ENE)** para interoperabilidad. La orden solo aporta la **envolvente de gálibo** que la
instalación debe respetar.

### 7.2. Cómo se condicionan mutuamente

| Aspecto de diseño | Qué exige la orden |
|-------------------|--------------------|
| **Altura de montaje del hilo** | Verificar el gálibo del pantógrafo entre `h'0` (6,5 m) y `h'u` (5 m) en anchos ibérico/estándar |
| **Desplazamientos laterales del hilo** | El contorno del pantógrafo en posición de captación define la "zona" que debe quedar libre: `bw + ep + S' + qs' + j'` |
| **Distancia de aislamiento** | Postes y brazos a tierra deben respetar `belec` (270/150 mm en 25 kV c.a.) |
| **Anchura de la mesilla** | Un pantógrafo de 1.950 mm (2·bw = 1.950 mm, `bw = 975 mm`) es el estándar para 3 kV y 25 kV; el de 1.600 mm no se admite en 3 kV |
| **Peralte y velocidad** | Los desplazamientos cuasiestáticos crecen con la insuficiencia de peralte; por eso los gálibos uniformes se definen para D e I máximos |

### 7.3. Hipótesis de los gálibos uniformes

El gálibo uniforme de implantación de obstáculos **asume una catenaria concreta** y un ancho de
mesilla, lo que muestra la ligazón entre gálibo e instalación:

| Parámetro | Ancho ibérico (3.10.7) | Ancho estándar (3.11.7) | Ancho métrico (3.12.7) |
|-----------|------------------------|-------------------------|------------------------|
| Radio mínimo en planta R | 250 m | 250 m | 100 m |
| Radio mínimo de acuerdo vertical Rv | 2.000 m | 2.000 m | 2.000 m |
| Sobreancho máximo | 30 mm | 30 mm | 30 mm |
| Peralte máximo D | 0,160 m | 0,160 m | 0,110 m |
| Insuficiencia de peralte máxima Imax | 0,175 m | 0,150 m | 0,070 m |
| TN en partes bajas | 5 mm | 5 mm | 5 mm |
| Estado de la vía | Balasto, mal estado | Balasto, mal estado | Balasto |
| **Catenaria** | **CA-160** | **EAC-350** | **CA-160** |
| Pantógrafo | 2·bw = 1.950 mm, cw = 0 | 2·bw = 1.950 mm, cw = 0 | 2·bw = 1.700 mm, cw = 0 |

> Si en un punto de la línea no se cumplen estas hipótesis, la determinación del gálibo nominal
> requiere un **estudio específico**.

### 7.4. Compatibilidad con la ETI de Energía (TSI ENE)

- El gálibo del material rodante interoperable (G1, GA, GB, GC) debe ser compatible con el
  gálibo de implantación de obstáculos de la línea (apartado 1.3.3, cuadro 1.4).
- La **distancia de aislamiento eléctrico** procede de la norma **UNE-EN 50119:2010** (líneas
  aéreas de contacto), que es la base técnica de la TSI ENE.
- Las distancias de borde de andén y los entreejes nominales de la orden son consistentes con
  los valores que exige la TSI ENE para material interoperable.
- En líneas de altas prestaciones con tráfico mixto, la orden remite además a las medidas
  operacionales de la **ETI de infraestructura de alta velocidad** (vientos laterales y
  condiciones de estibaje) para garantizar la seguridad de la circulación.

---

## 8. AUTOEVALUACIÓN

1. ¿Qué es el gálibo de implantación de obstáculos según la EN 15273-3:2013, tal como lo
   transcribe la orden?
2. Diferencia entre gálibo **límite**, **nominal** y **uniforme** de implantación de
   obstáculos. ¿Cómo se tratan los desplazamientos aleatorios en cada uno?
3. ¿Cuáles son las alturas de verificación del gálibo del pantógrafo (`h'0` y `h'u`) en una
   línea de ancho ibérico y en una de ancho métrico?
4. ¿Qué valores de `fs` y `fws+fwa` adopta la orden para la catenaria rígida?
5. ¿Qué altura de andén se exige en líneas de ancho ibérico o estándar europeo? ¿Y en ancho
   métrico?
6. ¿A qué distancia mínima del eje de la vía se sitúa el borde de un andén de 680 mm en vía
   recta de ancho estándar europeo (D = 0)?
7. ¿Qué banda libre de obstáculos debe dejarse por encima del andén?
8. ¿Cuál es el entreeje nominal para una línea con Vmax = 250 km/h? ¿Y para Vmax = 160 km/h en
   ancho ibérico (valores excepcionales)?
9. ¿Cuáles son los valores de los márgenes complementarios `M3b` y `M3h` del gálibo nominal y
   en qué zona se aplican?
10. ¿Qué gálibo deben cumplir los elementos **permanentes** y los **provisionales** en una zona
    de obras autorizadas por el administrador de infraestructura?

---

## 9. REFERENCIAS

- Orden FOM/1630/2015, de 14 de julio, Instrucción Ferroviaria de Gálibos (BOE-A-2015-8765):
  apartados 1.3, 1.3.1–1.3.3, 3.1–3.4, 3.5, 3.7.1–3.7.7, 3.8, 3.10.2–3.10.8, 3.11.2–3.11.8,
  3.12.2–3.12.8; cuadros 1.1–1.5, 3.5–3.8, 3.13–3.17, 3.22–3.24, 3.30; anejos 3 y 7
- EN 15273-3:2013 — Gálibos. Parte 3: Gálibo de implantación de obstáculos
- EN 15273-2:2013 — Gálibos. Parte 2: Gálibos del material rodante (contornos GA, GB, GC, GI)
- UNE-EN 50119:2010 — Aplicaciones ferroviarias. Instalaciones fijas. Líneas aéreas de contacto
- ETI de Energía (TSI ENE) y ETI de Infraestructura de Alta Velocidad — interoperabilidad
- Lección 1 del Módulo 3 — El gálibo del pantógrafo (mecánico y eléctrico)
- NAE 107 y NAE 300/301 (ADIF) — diseño de la línea aérea de contacto e implantación de
  instalaciones (referencia de proyecto, no contenido en la orden)

---

*Siguiente lección (prevista): distancias entre ejes de vías y gálibos en elementos
específicos, con aplicación práctica del anejo 7 de la orden.*
