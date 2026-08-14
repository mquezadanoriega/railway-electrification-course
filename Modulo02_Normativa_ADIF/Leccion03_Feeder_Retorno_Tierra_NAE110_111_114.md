# MÓDULO 2 · LECCIÓN 3
# CABLE ALIMENTADOR (FEEDER), RETORNO DE CORRIENTE Y CABLES AISLADOS (NAE 110 · 111 · 114)

## Documento base

> **Normas que soportan esta lección:**
>
> - **NAE 110** — «Pliego de condiciones técnicas para el montaje del cable alimentador o feeder (desnudo y aéreo) de la Línea Aérea de Contacto (catenaria 3 kV CC)». 1ª edición, abril 1998. Origen: Renfe, N.R.E.-L.A.C. nº 10 (40 págs.).
> - **NAE 111** — «Montaje del cable de tierra/retorno de la Línea Aérea de Contacto». 2ª edición, enero 2024. Grupo de trabajo GT-300, aprobada por el Comité de Normativa (24-ene-2024). Deroga la NAE 111 1ª ed. de abril 1998 (34 págs.).
> - **NAE 114** — «Montaje de cables aislados para feeders en corriente continua». 2ª edición, abril 2008 (59 págs.).
>
> Normas de montaje y ejecución: definen **cómo se instala** cada conductor; no son especificaciones de material (las ET 03.364.xxx definen **qué** se instala).

---

## 1. RESULTADO DE APRENDIZAJE

Al terminar esta lección serás capaz de:

1. Distinguir las **tres funciones del feeder** (alimentación/acometida, refuerzo o acompañamiento, y retorno) y su composición típica de cobre desnudo.
2. Aplicar los criterios de **montaje del feeder desnudo y aéreo** según NAE 110: ubicación en el poste, distancias, amarres, conexiones y anclajes.
3. Identificar los **cables de tierra/retorno** de la NAE 111 (L 110, LA 110, LA 180, LA 280), su función de puesta a tierra de postes y de conductor de retorno en c.a., y las reglas de separación y tendido.
4. Describir los **cables aislados para feeders de CC** (NAE 114): tensiones asignadas, aislamiento XLPE/EPR, pantallas, terminales termorretráctiles, empalmes y puesta a tierra de pantallas.
5. Relacionar la NAE 110, 111 y 114 con el resto de la familia normativa (NAE 101, 108, 112, NAS 310, ET de conductores) y saber dónde buscar cada dato.

---

## 2. RESUMEN EJECUTIVO

La catenaria necesita tres conductores auxiliares que **no tocan el pantógrafo** pero que hacen posible el funcionamiento del sistema:

- El **feeder** aporta sección conductora extra (alimenta o refuerza la LAC, o baja la resistencia del retorno).
- El **cable de tierra/retorno** protege a las personas e instalaciones ante faltas de aislamiento y, en c.a., conduce parte de la corriente de retorno.
- Los **cables aislados** sustituyen a los desnudos donde no hay gálibo o existe contaminación corrosiva (túneles, cruces, pasos superiores).

Las tres normas comparten filosofía: **tendido con poleas en todos los apoyos, tiro suave y progresivo, sobretense de 24 h, regulación del tense según tabla de tendido y temperatura ambiente, y comprobación por dinamómetro o flecha (error ±3 %)**. El dato eléctrico que condiciona todo es la **resistencia** de cada conductor: mientras más baja, más corriente transporta con menos caída de tensión.

| Concepto | NAE | Conductor típico | Sección (mm²) | Resistencia c.c. (Ω/km) |
|----------|-----|------------------|---------------|--------------------------|
| Feeder de alimentación | 110 | Cobre 2×225 / 2×300 | 225 / 300 | 0,080 / 0,061 |
| Feeder de refuerzo | 110 | Cobre 2×153 | 153,7 | 0,117 |
| Tierra/retorno | 111 | LA 110 / L 110 (y LA 180, LA 280) | 116,2 / 117,0 | 0,3067 / 0,2456 |
| Cable aislado de feeder | 114 | Cobre aislado XLPE/EPR 6/10 kV | 120…500 | 0,153…0,0366 |

> **Regla general de posicionamiento en el poste:** el feeder se coloca **lo más alto posible**, el cable de tierra **a media altura entre sustentador e hilo de contacto**; entre ambos se respetan distancias mínimas (27 cm de separación física en el punto más próximo y 90 cm entre ejes).

---

## 3. EL FEEDER: FUNCIÓN Y CIRCUITO DE ALIMENTACIÓN

El feeder es un **conductor de refuerzo en paralelo con la catenaria**, montado sobre los mismos postes de electrificación. En el sistema de 3 kV CC la corriente de tracción es muy elevada y la sección de sustentador + hilo de contacto no basta para mantener la tensión dentro de límites aceptables; el feeder **añade sección conductora** sin aumentar la superficie de contacto.

### 3.1. Tipología según su funcionalidad (NAE 110, apdo. 3)

| Tipo | Función | Composición típica |
|------|---------|--------------------|
| **Feeder de alimentación** (o de acometida) | Procede de la **subestación rectificadora** y aporta energía a la LAC. Se conecta a la catenaria en el **vano de elevación del seccionamiento**. | Cobre **2×225** o **2×300** mm² |
| **Feeder de refuerzo** (o de acompañamiento) | Aumenta la **sección conductora** de la LAC. Se conecta a intervalos equidistantes **al sustentador y al hilo de contacto** mediante cable flexible. | Cobre **2×153** mm² |
| **Feeder de retorno** | Disminuye la **resistencia eléctrica del circuito de retorno** a la subestación rectificadora. | Igual que alimentación: **2×225** o **2×300** mm² |

### 3.2. Diagrama del circuito de alimentación

```
  SUBESTACIÓN RECTIFICADORA 3 kV CC
        |  (+)
        |  ┌───────────────────────────────────────────────┐
        |  │  FEEDER DE ALIMENTACIÓN (2×225 / 2×300)       │
        |  │  ─────────────────────────────────────────►   │
        |  │        conexiones cada ~300 m (cable 95 mm²   │
        |  │        extraflexible, entre 1ª y 2ª péndola)  │
        v  │        │            │            │            │
        |  └────────┼────────────┼────────────┼────────────┘
        |           ▼            ▼            ▼
        |   SUSTENTADOR ──────────────────────────────────────────►
        |        │ (péndolas) │             │
        |        ▼            ▼             ▼
        |   HILO DE CONTACTO  ●●●●● (pantógrafo) ●●●●●
        |           │
        |           │ corriente retorna por carriles
        v           │
  ┌──────────────┐  │
  │ RETORNO      │◄─┘   feeder de retorno (2×225/2×300) baja la
  │ (carriles +  │      resistencia del circuito de vuelta
  │ feeder y/o   │
  │ cable tierra)│
  └──────────────┘
```

### 3.3. Características de los cables de cobre desnudo (NAE 110, apdo. 3)

| Característica | Cu 153 | Cu 225 | Cu 300 |
|----------------|--------|--------|--------|
| Diámetro (mm) | 16,1 | 19,46 | 22,47 |
| Sección (mm²) | 153,73 | 225 | 300 |
| Peso lineal (kg/m) | 1,405 | 2,07 | 2,7 |
| Módulo elástico (kg/mm²) | 10.300 | 10.300 | 10.300 |
| Coef. dilatación (ºC⁻¹) | 17×10⁻⁶ | 17×10⁻⁶ | 17×10⁻⁶ |
| Carga de rotura (kg) | 6.060 | 8.910 | 11.850 |
| Resistencia (Ω/km) | 0,117 | 0,08 | 0,061 |

> **Excepciones (NAE 110):** en túneles, pasos superiores o estaciones pueden emplearse **cables forrados**; también puede justificarse el uso de **cables de aluminio** con sección equivalente en cobre.

---

## 4. MONTAJE DEL FEEDER DESNUDO Y AÉREO (NAE 110)

### 4.1. Ubicación en el poste y distancias

- Se instala en **cabeza de poste** o sobre **mensulilla**, a la **mayor altura posible** y siempre por encima de otros cables sustentados por el mismo apoyo.
- Disposición según número de feeders:
  - **1 feeder:** cabeza de poste o mensulilla.
  - **2 feeders:** mensulilla (uno por arriba y otro por debajo).
  - **3 feeders:** uno en cabeza de poste y dos en mensulilla.
  - Las mensulillas se instalan **entre las dos primeras cartelas del poste**.
  - Casos especiales (más feeders): ménsulas o crucetas con equipos de suspensión adecuados, justificando técnicamente.
- **Distancia a otros cables del mismo poste:** nunca menor de **25 cm** en el punto más próximo, para la condición ambiental más desfavorable.
- Cada cable queda **sujeto al aislador** en cada suspensión mediante su elemento de amarre; los aisladores serán de **una o dos gargantas** según el número de cables.

### 4.2. Cables múltiples y amarres

- Si el feeder está formado por **más de un cable**, se amarran entre sí con **retenciones de alambre de cobre recocido de 2,3 mm** de diámetro, **mínimo 3 vueltas**, separadas **máximo 2 m**, formando un solo cuerpo.

### 4.3. Conexiones y anclajes

| Elemento | Prescripción (NAE 110, apdo. 4) |
|----------|----------------------------------|
| Conexión feeder–catenaria | En el **vano de elevación del seccionamiento** correspondiente. |
| Conexión de alimentación feeder–sustentador | Cada **~300 m**, con **dos cables independientes de cobre de 95 mm² extraflexible** a tensión reducida, colocadas **entre la primera y segunda péndola** del mismo hilo de contacto; conexión con **grifas** adecuadas al tipo de cable. |
| Amarre de seguridad (feeder de acompañamiento) | Aproximadamente cada **2.000 m** de tendido, ubicado en el **anclaje del punto fijo de vía general**. |
| Anclajes de extremo | En los puntos finales de alimentación, con **colas de anclaje**, conjuntos de tirante y **macizos de anclaje** adecuados al tense establecido. |
| Empalmes | Distancia entre dos empalmes **nunca menor de 800 m**; se prohíben empalmes por rotura del cable en bobina, montaje inadecuado o restos de bobina. Se realizan en el **centro del vano** o lo más próximo, según la **ET RENFE 03.364.015.2** y la **N.R.E.-L.A.C. nº 1** (grifas). |

### 4.4. Tendido y tensado

- El tendido se realiza con **arrastre mecánico** (o a mano si la obra o el terreno lo impiden).
- **Medios obligatorios:** poleas en todos los apoyos (UNE 21100), cabrestantes con freno, portabobinas con frenado, dinamómetros (precisión ±2 % de la escala; ±0,1 % en electrónicos digitales) y termómetros (±1 ºC).

| Cable | Polea UNE 21100 | d (mm) | d₁ (mm) | l (mm) | R (mm) |
|-------|-----------------|--------|---------|--------|--------|
| Cu 153 | Pt 450 | 450 | 500 | 350 | 25 |
| Cu 225 | Pt 450 | 450 | 500 | 350 | 25 |
| Cu 300 | Pt 660 | 660 | 730 | 500 | 36 |

*(d = diámetro en el fondo de la garganta; d₁ = diámetro exterior; l = longitud de la horquilla; R = radio de la base de la garganta.)*

- La garganta tendrá **superficie lisa**, profundidad **> 2× el diámetro del cable**, radio de base **R ≥ 10 % superior al radio del cable** y **d > 20× el diámetro del cable**.
- Condiciones de tendido: se desprecian ~**1 m** al principio y fin de cada bobina; el **ángulo de despegue** del cable con la horizontal **no excederá de 45°**; el tiro será **suave y progresivo**; las maniobras, sin sacudidas; se usan **quitavueltas** entre conductor y cable piloto.
- **Tracción máxima de tendido:** la tensión máxima de la hipótesis de viento (zona B) o de hielo (zona C) de las tablas del Anexo 1. La tensión mínima será la que permita hacer circular el cable por las poleas sin rozar obstáculos.

### 4.5. Secuencia después del tendido

1. **Arriostrado** por sus extremos con **sobretense** hasta la tensión máxima de las tablas, durante **mínimo 24 h**.
2. **Destensado** del tramo.
3. Colocación del cable en su **conjunto de suspensión** (desmontaje de las poleas).
4. **Regulación del tense** según la tabla de tendido y la temperatura ambiente, comprobando con **dinamómetro** o por **medición de flecha** (error admitido **±3 %**, norma UNE 21-101-73).
5. **Retención** de los cables al aislador y desmontaje de las poleas.

### 4.6. Amarres de seguridad finales

- Ubicados en el **poste del punto fijo de vía general**, aprovechando sus macizos y conjuntos de anclaje, **alternativamente cada ~200 m**.
- En el conjunto de suspensión del feeder del poste del punto fijo se monta un **yugo de hilo de contacto recocido** amarrado al cable con grifas.
- Se instalan **anclajes tipo Cu-26V**, amarrados por un extremo a cada lado del conjunto de suspensión y por el otro al poste de anclaje. **No se permite el uso de aprietahilos.**

### 4.7. Tabla de tendido y zonas climáticas (NAE 110, apdo. 7)

El cálculo se efectúa según el **Reglamento Técnico de Líneas Aéreas de Alta Tensión** del Ministerio de Industria:

| Cable | Zona | Hipótesis | Peso condicional (kg/m) | t inicial | Tensión máx. (kg) | Coef. seguridad |
|-------|------|-----------|-------------------------|-----------|-------------------|-----------------|
| Cu 153 | B | Viento | 2,127 | −15 ºC | 1.330 | 4,56 |
| Cu 153 | C | Hielo | 2,849 | −20 ºC | 1.330 | 4,56 |
| Cu 225 | B | Viento | 2,864 | −15 ºC | 1.782 | 5 |
| Cu 225 | C | Hielo | 3,658 | −20 ºC | 1.782 | 5 |
| Cu 300 | B | Viento | 3,553 | −15 ºC | 2.236 | 5,3 |
| Cu 300 | C | Hielo | 4,407 | −20 ºC | 2.236 | 5,3 |

- **Zona B:** altitudes entre 500 y 1.000 m. **Zona C:** altitudes superiores a 1.000 m. **Zona A** (< 500 m): se aplican los datos de la zona B (flechas y tensiones coincidentes).

> **Seguridad (NAE 110):** antes de la puesta en servicio se advertirá con tiempo suficiente; se cumplirá la Consigna General C/G/SHT nº 3 (7-1-85), la Ley BOE 8-11-95 de prevención de riesgos laborales y la Consigna C-16.

---

## 5. CIRCUITO DE TIERRA Y RETORNO (NAE 111)

### 5.1. Objeto y campo de aplicación

La NAE 111 (2ª ed., ene-2024) fija las condiciones del **montaje del cable de tierra y/o cable de retorno** en las LAC de Adif y Adif AV, tanto en **c.c.** (3 kV y 1,5 kV) como en **c.a.** (25 kV). Solo aplica a cables de **aluminio y aluminio-acero** indicados en la norma.

**Definición (UNE-EN 50119, transcrita en NAE 111):** *cable de tierra/retorno* es el cable o hilo metálico que conecta los **soportes a la tierra o al rail** para asegurar la protección de las personas e instalaciones en caso de falta de aislamiento y que, además, puede servir de **cable de retorno**.

> La norma distingue también el **feeder de alimentación** (aéreo, en la misma estructura de la LAC, conectado a intervalos frecuentes para incrementar su sección) y el **feeder de refuerzo** (aéreo, al lado de la LAC, que alimenta diferentes secciones).

### 5.2. Conductores normalizados (NAE 111, Tabla 1)

Como regla general se emplea **LA 110** (aluminio-acero, 94-AL1/22-ST1A) o **L 110** (aluminio, 117-AL1). Los **LA 180** (147-AL1/34-ST1A) y **LA 280** (242-AL1/39-ST1A) se seleccionan en función del **estudio de dimensionamiento eléctrico**.

| Característica | LA 110 | L 110 | LA 180 | LA 280 |
|----------------|--------|-------|--------|--------|
| Denominación UNE-EN 50182 | 94-AL1/22-ST1A | 117-AL1 | 147-AL1/34-ST1A | 242-AL1/39-ST1A |
| Diámetro (mm) | 14,0 | 14,0 | 17,5 | 21,8 |
| Sección (mm²) | 116,2 | 117,0 | 181,6 | 281,1 |
| Masa (kg/m) | 0,4325 | 0,3215 | 0,6758 | 0,9762 |
| Módulo elástico (daN/mm²) | 8.044,2 | 5.591,7 | 8.044,2 | 7.553,7 |
| Coef. dilatación (ºC⁻¹) | 17,8×10⁻⁶ | 23,0×10⁻⁶ | 17,8×10⁻⁶ | 18,9×10⁻⁶ |
| Resistencia a la tracción (daN) | 4.317 | 1.989 | 6.494 | 8.489 |
| **Resistencia c.c. (Ω/km)** | **0,3067** | **0,2456** | **0,1963** | **0,1195** |

### 5.3. Características del montaje (NAE 111, apdo. 5)

- El cable de tierra se monta **a lo largo de todo el trazado**, sobre los postes de la LAC.
- **Misión principal:** poner a tierra los postes en los que **no se pueda colocar pica de puesta a tierra** y, en sistemas de **c.a.**, conducir **parte de la corriente de retorno**.
- Se coloca **preferiblemente a media altura entre sustentador e hilo de contacto**, respetando el **punto de fijación de la cara exterior** definido en cada poste.
- **Todos los postes** quedan unidos **mecánica y eléctricamente** al cable de tierra mediante la **grapa de suspensión** correspondiente (según tipo de catenaria).

**Distancias y separaciones clave:**

| Magnitud | Valor (NAE 111) |
|----------|-----------------|
| Separación feeder – cable de tierra (punto más próximo, condición más desfavorable) | **≥ 27 cm** (con feeder por encima del cable de tierra) |
| Separación entre ejes de la grapa de tierra y del feeder en el poste | **≥ 90 cm** |
| Altura mínima del cable de tierra en pasos a nivel | **> 5,5 m** (casos excepcionales según UNE-EN 50122-1) |
| Cruce de vías | En **canalización bajo vías** (norma NAS 310), **nunca sobre la LAC ni sobre el feeder** |

**Otras prescripciones:**
- **Anclajes** en los extremos del tendido (colas de anclaje, conjuntos de tirante y macizos) y a la **entrada/salida de túneles**.
- En **c.c.**, donde exista **pozo de tierras**, se realiza una **bajada** para conectar el cable de tierra con la **pica principal**.
- Los **pararrayos de óxidos metálicos** de los postes se conectan al cable de tierra mediante grapa y cable adecuado, y a la pica o pozo correspondiente.
- **Empalmes:** **no se admiten**; solo con autorización de la Dirección de Obra, en el **centro del vano** o lo más próximo, con **manguitos de empalme de compresión de plena tracción**.
- Excepcionalmente, en tramos cortos con vanos cortos donde no se pueda anclar, se admite tender con **tense reducido**.

### 5.4. Proceso de montaje, poleas y cálculo de tendido

- **Poleas:** obligatorias en todos los apoyos, de **aleación de aluminio** (UNE-EN 1706) según UNE 21100. Para los cuatro conductores la polea es **Pt 450** (d = 450, d₁ = 500, l = 350, R = 25 mm). Garganta lisa, profundidad > 2× diámetro, R ≥ 10 % del radio del cable y d > 20× diámetro.
- Proceso idéntico al feeder: sobretense hasta tensión máxima **mínimo 24 h**, destensado, regulación del tense con dinamómetro o flecha (**error 3 %**, UNE 21101), fijación en su suspensión y desmontaje de poleas.
- **Empalme excepcional:** para L 110 / LA 110 según la **NAE 101** vigente; para LA 180 / LA 280 según el proyecto constructivo.
- **Cálculo mecánico (apdo. 8):** los cables de tierra/retorno **no están compensados**, por lo que son sensibles a la temperatura (flecha y tense). Condiciones límite:
  - **Coeficiente de seguridad a la rotura ≥ 2,5** en las condiciones de máxima tracción.
  - **EDS a 15 ºC sin sobrecarga ≤ 15 %** de la carga de rotura.
  - Vano de regulación: **ar = √(Σai³ / Σai)**; flecha de cada vano: **fi = fr·(ai/ar)²**.
  - Flecha en vanos a nivel o desnivel < 10 %: **f = a²·p / (8·T)**; en vanos de gran desnivel (> 10 %): **f = b²·p / (8·Tm)**.
  - Tablas de tendido del Anejo 3 calculadas según la **tabla 4 de la ITC-LAT 07** del RLAT (RD 223/2008) y el punto 104 de la ITC-LAT 01.

### 5.5. Conexión a carril y referencia de material

La definición de la norma (apdo. 3) contempla la conexión del cable de tierra **a la tierra o al rail**; los esquemas de montaje, las grapas de sujeción/conexión y terminales se recogen en el **Anejo 1** de la NAE 111 y en las ET asociadas (ET 03.364.021.0 «Grapas de sujeción, conexión y terminales para la línea de tierra de la LAC en c.c.» y ET 03.360.161.8 «Carril»). El detalle constructivo de cada tipo de catenaria se toma de las **NAE 300/301/302** de diseño funcional.

> **Normativa de seguridad aplicable (NAE 111):** procedimiento **Adif-PE-301-001-006-SC-521** «Cortes de Tensión en Líneas Aéreas de Contacto alimentadas en 25 kV c.a., 3 kV c.c. y 1,5 kV c.c.», además de la reglamentación de Seguridad y Salud.

---

## 6. CABLES AISLADOS PARA FEEDERS EN CC (NAE 114)

### 6.1. Cuándo se usan y tipos de montaje

Los cables aislados (especificados en la **ET 03.364.157.2**) se instalan donde **no existe gálibo para colocarlos desnudos** o el ambiente es agresivo:

- Contaminación atmosférica **corrosiva** (gases de industrias químicas).
- **Túneles de gálibo escaso**, cruces de vías y pasos superiores.
- Otros casos "especiales" con **autorización expresa del Director de Obra**.

Tipos de montaje:
- **Aéreo:** fijado a muros, apoyado o suspendido de los postes de electrificación.
- **Subterráneo:** en zanja o canal, canaleta, galería o tubo.

### 6.2. Características de los cables

| Parámetro | Valor (NAE 114) |
|-----------|-----------------|
| Tensión asignada (feeders) | **6/10 (12) kV** |
| Tensión asignada (cables de negativo) | **0,6/1 (1,2) kV** |
| Aislamiento | **XLPE** (polietileno reticulado) o **EPR** (goma etileno-propileno) |
| Cubierta externa | Según **UNE-HD 620**; poliolefina (Z1), mezcla **DMZ2**; resistente al frío, agua, abrasión, golpes y desgarro |
| Pantalla metálica (cables 6/10 kV que la lleven) | Corona de **alambres de cobre recocido de 0,5 a 1 mm** en hélice (paso ≤ 20× diámetro bajo pantalla; separación entre alambres ≤ 4 mm) + **fleje de cobre de ≥ 1 mm²** (paso ≤ 4× diámetro bajo pantalla) |

**Tabla I — Características dimensionales** (extracto):

| Sección del conductor (mm²) | 120 | 150 | 185 | 240 | 300 | 400 | 500 |
|-----------------------------|-----|-----|-----|-----|-----|-----|-----|
| Diámetro máx. del conductor (mm) | 13,5 | 15,0 | 16,8 | 19,2 | 21,6 | 24,6 | 27,6 |
| Aislamiento 0,6/1 XLPE (mm) | 1,2 | 1,4 | 1,6 | 1,7 | 1,8 | 2,0 | 2,2 |
| Aislamiento 0,6/1 EPR (mm) | 1,6 | 1,8 | 2,0 | 2,2 | 2,4 | 2,6 | 2,8 |
| Aislamiento 6/10 XLPE y EPR (mm) | 3,4 | 3,4 | 3,4 | 3,4 | 3,4 | 3,4 | 3,4 |
| Pantalla metálica, sección mín. (mm²) | 25 | 25 | 25 | 25 | 25 | 25 | 25 |
| Cubierta, espesor nominal (mm) | 2,5 | 2,5 | 2,5 | 3,0 | 3,0 | 3,0 | 3,0 |

*(Semiconductoras sobre conductor y aislamiento, cuando proceda: 0,5 mm.)*

**Tabla II — Características eléctricas (cables al aire, 40 ºC):**

| Sección (mm²) | 120 | 150 | 185 | 240 | 300 | 400 | 500 |
|---------------|-----|-----|-----|-----|-----|-----|-----|
| Resistencia máx. del conductor a 20 ºC (Ω/km) | 0,153 | 0,124 | 0,0991 | 0,0754 | 0,0601 | 0,0470 | 0,0366 |
| Intensidad permanente 6/10 kV XLPE (A) | 365 | 415 | 475 | 555 | 645 | 745 | 845 |
| Intensidad permanente 6/10 kV EPR (A) | 345 | 390 | 450 | 525 | 610 | 705 | 805 |
| Intensidad permanente 0,6/1 kV XLPE (A) | 335 | 385 | 450 | 535 | 615 | 720 | 825 |
| Intensidad permanente 0,6/1 kV EPR (A) | 325 | 375 | 440 | 515 | 595 | 700 | 800 |

### 6.3. Cortocircuito y correcciones

- **Densidad de corriente de cortocircuito admisible** (XLPE y EPR, temperatura final 250 ºC): 0,1 s → **449 A/mm²**; 0,5 s → 201; 1,0 s → 142; 2,0 s → 100; 3,0 s → **82 A/mm²**.
- **Tabla VII:** intensidades máximas en kA por sección y tiempo (p. ej., 1 s: 120 mm² → 17,14 kA; 300 mm² → 42,86 kA; 500 mm² → 71,44 kA).
- **Factores de corrección** para enterrados: por temperatura distinta, por resistividad térmica del terreno distinta de 150 ºC cm/W, por influencia térmica de cables/ternas paralelos (p. ej., 2 ternas separadas 7 cm → 0,85) y por profundidad de zanja.

### 6.4. Radios de curvatura

| Situación | Cable | Radio mínimo |
|-----------|-------|--------------|
| En servicio (campo no radial) | Sin armadura, D < 25 mm | 4D |
| En servicio (campo no radial) | Sin armadura, 25–50 mm | 5D |
| En servicio (campo no radial) | Sin armadura, D > 50 mm | 6D |
| En servicio (campo no radial) | Armados | 10D |
| En servicio (campo radial, unipolares) | — | 10(D+d) |
| Durante el tendido | No armados | 4D / 5D / 6D según D |
| Durante el tendido | Armados | 10D |

### 6.5. Manipulación de bobinas

- Bobinas de **madera**, con ala de diámetro entre **63 y 270 cm**; etiqueta indeleble con código de barras, características, peso y longitud.
- Izado con barra o eje por los agujeros centrales de los platos (grúa) o por la parte inferior de ambos platos (carretilla elevadora).
- **Prohibido:** retener la bobina con cuerdas que la abracen, dejarla caer al suelo (aunque se use amortiguador), rodarla largas distancias y apilarla en exceso.
- **Almacenamiento:** evitar intemperie prolongada y agua bajo la bobina; proteger los **extremos del cable** contra la humedad (capuchones de goma).

### 6.6. Montaje subterráneo

| Elemento | Prescripción (NAE 114) |
|----------|-------------------------|
| Zanja | Profundidad mínima **1,10 m**; cable de energía primero y los de seguridad/comunicaciones después, separados por **40 cm** de tierra. Catas de reconocimiento y señalización de obra antes de abrir. |
| Canaleta | Para instalaciones no accesibles al público, con tapas enrasadas. |
| Tubo | Arquetas de registro en cambios de dirección, cruces de vías y empalmes. Cumple la **NAS 310**. |
| Galerías accesibles | Cables en laterales; energía en **bandejas inferiores**; si hay tuberías de fluidos, cables en la pared opuesta. |
| Galerías no accesibles | Se consideran como tubos o canaletas. |

**Tendido en zanja/canaleta:** lecho de **10 cm de arena o tierra cribada**; rodillos cada **3 a 6 m** (esfuerzos de arrastre ≈ **15 % del peso** del cable); tracción máxima **5 kg/mm²**; velocidad **≤ 5 m/min**; dinamómetros obligatorios; no dejar el cable en zanja abierta sin cubrir con **0,10 m de arena fina** y protección.

**Tendido en tubo:** diámetro interior **2D** (unipolares/tripolares) o **4D** (ternas). Tubo general: **PVC negro rígido de 100 mm** de diámetro exterior, 3 mm de espesor y 6 m de longitud (otros, con autorización del Director de Obra). Grupos de tres en triángulo, separación entre ejes **≥ 60 cm**, a **≥ 5 cm** de las paredes, plano superior a **80 cm** de profundidad; solera de **hormigón H-125 de 5 cm**, cobertura de hormigón de **10 cm**, **30 cm de arena** y **cintas plásticas indicativas**; relleno en capas de 20 cm.

### 6.7. Montaje aéreo

- Uso en **grandes estaciones**, zonas con edificios próximos a la vía o túneles.
- Sobre postes, ménsulas, pórticos rígidos o muros; en lo aplicable se sigue el **REBT** y el **RAT**.
- Tracción máxima **5 kg/mm²**; velocidad **≤ 5 m/min**.
- **Cable fiador de acero tipo Ac-72** cuando las solicitaciones lo requieran, con tensión de servicio de unos **1.425 kg a 20 ºC**; unión al fiador con **grapas tipo telefónico** (que no dañen la cubierta) cada **~0,5 m**.
- **Conjuntos de feeders aéreos más comunes:** 1×300, 2×300, 2×240 y 2×150 mm².

| Conjunto | Diámetro unitario (mm) | Peso unitario (kg/m) | Peso total (kg/m) |
|----------|------------------------|----------------------|-------------------|
| 1×300 | 40 | 4,3 | 4,3 |
| 2×300 | 40 | 4,3 | 8,6 |
| 2×240 | 40 | 3,8 | 7,6 |
| 2×150 | 36 | 2,6 | 5,2 |

- En muros o túneles: tendido con **perchas y grapas** sujetas a la pared, instaladas cada **1 a 1,50 m**.

### 6.8. Terminales y empalmes

- Se adoptan **accesorios termorretráctiles** (material plástico reticulado por radiación electrónica): se adaptan a varios diámetros de cable, son estables frente a agentes externos, de fácil instalación con aporte de calor y con carácter **sellador antihumedad**.
- **Terminales:** montaje según instrucciones de cada fabricante (norma **UNE-HD 692-2**). El engastado puede ser por **tornillería fusible, compresión o punzonado**.
- **Empalmes:**
  - Los **feeders de alimentación se montan siempre sin empalmes** en toda su longitud (se pide la bobina midiendo el tramo).
  - En montaje subterráneo se admite el **conector con tornillos de par de apriete predefinido** (pernos que se **autocizallan** al alcanzar el par, garantizando la conexión).
  - El aislamiento del empalme lo forman **dos tubos elastoméricos termorretráctiles de doble pared** (capa semiconductora exterior que actúa de pantalla).
  - Un empalme es siempre un **caso excepcional** y requiere **autorización expresa del Director Facultativo**.

### 6.9. Puesta a tierra de pantallas

- Las **pantallas** se conectan a tierra para evitar **tensiones inducidas** en las cubiertas metálicas.
- Cada bobina se pone a tierra en **un extremo**, coincidiendo con la **tierra de la pantalla del lado de la subestación**, unida al **cable de tierra**; **la pantalla de los empalmes no se une en los mismos**.
- Longitud máxima de bobina ≈ **1.000 m**; los empalmes deberían coincidir con la **bajada del cable de tierra**.
- Se desnuda armadura y pantalla y se conecta al **pozo de tierra** mediante terminal de apriete y la línea de tierra. Antes de trabajar en cables apantallados (después de cortar tensión) es preceptivo **descargar a tierra la pantalla**.
- **Sección mínima de la línea de tierra** (cobre): calculada por la expresión **S ≥ Id·√t / α**, con **α = 13** para cobre (t ≤ 5 s) y Δθ de 160 ºC (aislado) o 180 ºC (desnudo); **en ningún caso inferior a 50 mm²**. Se elige la sección normalizada igual o superior.
- En montaje aéreo, la **bajada al pozo** va **entubada con tubo PVC armado de 1 pulgada**, grapado por la parte interior del poste. La conexión al pozo se hace con grapas apropiadas, tornillería de acero inoxidable o elementos de compresión, con contactos limpios y sin humedad.

---

## 7. COORDINACIÓN CON OTRAS NORMAS

| Norma / Documento | Relación con esta lección |
|-------------------|---------------------------|
| **NAE 101** | Grifas de conexión y empalme para la catenaria; referenciada por NAE 110 (empalmes) y NAE 111 (empalmes excepcionales de L 110/LA 110). |
| **NAE 108 / NRE-LAC 1, 2, 3** | Normas de tendido/tensado y montaje de grifas, accesorios preformados y anclajes de seguridad (referenciadas por NAE 110). |
| **NAE 112** | Seccionamiento de la LAC: el feeder de alimentación se conecta a la catenaria en el **vano de elevación del seccionamiento** (NAE 110, apdo. 4). |
| **NAE 300 / 301 / 302** | Diseño funcional de catenarias CA-160/3 kV, CA-220/3 kV y CA-160H/CA-200H; fijan el punto de fijación del cable de tierra y las grapas según tipo (NAE 111, apdo. 5). |
| **NAS 310** | Sistemas de tendido subterráneo de cables; aplica a canalizaciones bajo vías (NAE 111) y a tubos/arquetas (NAE 114). |
| **ET 03.364.xxx** | Especificaciones de material: cables de cobre desnudo (03.354.011), cables de aluminio desnudo (03.364.161.4), grifas (03.364.015.2), accesorios preformados (03.364.004.6), anclajes de seguridad (03.364.017.8), grapas de línea de tierra (03.364.021.0), carril (03.360.161.8) y cables aislados para feeders (03.364.157.2). |
| **RD 223/2008 (RLAT + ITC-LAT 01, 07)** | Base de cálculo de las tablas de tendido del feeder (NAE 110) y del cable de tierra (NAE 111). |
| **IFE (Orden TMA/135/2023)** | Instrucción ferroviaria del subsistema de energía; condiciones límite del cálculo mecánico (NAE 111). |
| **UNE-EN 50119 / 50122-1** | Definiciones de cable de tierra y seguridad eléctrica/puesta a tierra (NAE 111). |
| **Adif-PE-301-001-006-SC-521** | Cortes de tensión en LAC (3 kV y 1,5 kV c.c.; 25 kV c.a.) — seguridad en trabajos. |

---

## 8. AUTOEVALUACIÓN

1. ¿Cuáles son las tres tipologías de feeder según la NAE 110 y con qué cables se componen típicamente cada una?
2. ¿Qué distancia mínima debe respetarse entre el feeder y otros cables apoyados en el mismo poste (NAE 110)?
3. ¿Cada cuántos metros se instalan las conexiones de alimentación entre el feeder y el sustentador, y con qué cable se ejecutan?
4. ¿Cuál es la distancia mínima entre dos empalmes del feeder desnudo? ¿Dónde deben realizarse los empalmes?
5. ¿Cuánto tiempo mínimo se somete el feeder al sobretense tras el tendido, y con qué error máximo se mide la flecha?
6. ¿Qué dos conductores son los normalizados por defecto para el cable de tierra/retorno en la NAE 111 y cuál es su resistencia en c.c.?
7. ¿Cuáles son las separaciones mínimas entre el cable de tierra y el feeder (27 cm y 90 cm) y qué significado tiene cada una?
8. ¿Qué condiciones debe cumplir el empalme excepcional del cable de tierra/retorno según la NAE 111?
9. ¿Cuáles son las tensiones asignadas de los cables aislados de feeder y de negativo, y qué aislamientos se emplean (NAE 114)?
10. ¿Cuál es la sección mínima de la línea de tierra para las pantallas y qué valor tiene α para el cobre con t ≤ 5 s?

---

## 9. REFERENCIAS

- **NAE 110** (1ª ed., abr 1998). «Pliego de condiciones técnicas para el montaje del cable alimentador o feeder (desnudo y aéreo) de la Línea Aérea de Contacto (catenaria 3 kV CC)». Origen: Renfe N.R.E.-L.A.C. nº 10.
- **NAE 111** (2ª ed., ene 2024). «Montaje del cable de tierra/retorno de la Línea Aérea de Contacto». Adif, Comité de Normativa.
- **NAE 114** (2ª ed., abr 2008). «Montaje de cables aislados para feeders en corriente continua». Adif.
- Normas citadas en los textos: UNE 21100, UNE 21101, UNE 21-101-73, UNE-EN 50119, UNE-EN 50122-1, UNE-EN 50182, UNE-EN 1706, UNE 21018, UNE 21123, UNE 21192, UNE-HD 620, UNE-HD 692-2, IEC 60502-2.
- Reglamentación: RD 223/2008 (RLAT e ITC-LAT 01 y 07); Orden TMA/135/2023 (IFE); Ley BOE 8-11-95 de prevención de riesgos laborales; procedimiento Adif-PE-301-001-006-SC-521.
- Normas de diseño funcional: NAE 300, NAE 301, NAE 302.
- Especificaciones técnicas: ET 03.364.157.2, ET 03.364.161.4, ET 03.364.021.0, ET 03.360.161.8, ET 03.364.015.2, ET 03.364.017.8, ET 03.364.004.6.
- Norma de sistemas subterráneos: NAS 310.
