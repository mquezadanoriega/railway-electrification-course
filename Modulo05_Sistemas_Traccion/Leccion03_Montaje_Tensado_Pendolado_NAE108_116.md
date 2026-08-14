# MÓDULO 5 · LECCIÓN 3
# MONTAJE Y TENSADO DEL SUSTENTADOR E HILO · PENDOLADO

## NAE 108 · NAE 116 — De la teoría de diseño al montaje real

> **Documentos base:**
> - **NAE 108**, «Ejecución del montaje del sustentador e hilo de contacto»,
>   2ª edición, diciembre 2025. Aplica a 1,5 kV c.c., 3 kV c.c. y 25 kV c.a.
> - **NAE 116**, «Cálculo y montaje del pendolado para líneas aéreas de contacto
>   de c.c.», 1ª edición + M1, enero 2019 (aplica a CA-160 y CA-220).

---

## 1. RESULTADO DE APRENDIZAJE

Al terminar esta lección serás capaz de:

1. Explicar el **proceso de tendido** del sustentador y los hilos de contacto
   (cantones, poleas, bloqueos, colas de anclaje)
2. Aplicar el **sobretense** (20 %, 24–48 h) y saber por qué se hace
3. Calcular con las fórmulas de compensación por temperatura el **desplazamiento
   de ménsula (D)** y el **desplazamiento de contrapesos (Dv)** de una obra
4. Leer las **tablas de tense** (nominal, sobretense y límites de tendido) por
   tipo de catenaria
5. Distinguir **pendolado arbitrario, equidistante y por parejas**, y saber cuál
   aplica en cada vía
6. Usar las **tablas de distribución de péndolas** y los **criterios de cálculo**
   (elasticidad, fuerzas del pantógrafo, descentramiento)
7. Conocer los **coeficientes de seguridad** y los materiales de los conductores

---

## 2. RESUMEN EJECUTIVO

Las lecciones 1 y 2 (NAE 107 y NAE 300/301/302) definieron **qué** hay que instalar
y **cuánto vale cada parámetro**. Esta lección explica **cómo** se lleva al terreno:
la NAE 108 fija el **proceso de tensado** (que convierte los `kgf` de diseño en un
montaje real con una temperatura y una fecha concretas) y la NAE 116 fija el
**cálculo y montaje del pendolado**, que es lo que materializa la geometría
(altura de hilo, flecha) en cada vano.

Idea clave de la NAE 108: **el tense de diseño solo se materializa a la temperatura
media anual**. Si se tiende en otro momento, la dilatación del cobre obliga a
desplazar las ménsulas (D) y los contrapesos (Dv) respecto de su posición neutra.
Por eso las dos fórmulas de compensación por temperatura son el corazón de la norma.

Idea clave de la NAE 116: el pendolado se **calcula** (longitud de cada péndola a
partir de las flechas de sustentador e hilo) y se **distribuye** según tablas de
referencia por parejas; el objetivo es una elasticidad uniforme (~3 mm/kg) para
que el pantógrafo no pierda contacto a alta velocidad.

---

## 3. NAE 108 — MONTAJE DEL SUSTENTADOR E HILO DE CONTACTO

### 3.1. Objeto y condiciones previas

- Aplica a **obra nueva, rehabilitación, renovación y control de calidad** en las
  catenarias de **1,5 kV c.c., 3 kV c.c. y 25 kV c.a.** de Adif/Adif AV.
- El tendido se hace **por cantones completos, sin empalmes** de sustentador ni de
  hilo; las bobinas se identifican y se metran previamente.
- Condiciones previas: postes con el desplome correcto según radio, **ménsulas
  montadas y bloqueadas durante el tendido**, descentramientos en curva ya
  calculados en proyecto.

### 3.2. Proceso de tendido

1. **Cola de anclaje del cantón** instalada y bloqueada (si es compensada);
   conexión del cable con grapa o preformado.
2. **Tendido:** las bobinas desbobinan hacia las **poleas de freno**, que regulan
   el tense. Si el sistema lo permite se tiende **directamente a tense nominal**;
   en caso contrario se sobretensa después. El sustentador nunca arrastra por el
   suelo; **ángulo de despegue de la bobina ≤ 45°**.
3. **Colocación provisional:** sustentador sobre **poleas de sujeción**; en ménsulas
   de celosía se amarra con **preformados**, y en tubulares con **casquillo
   bimetálico**. El hilo cuelga de **ganchos de cobre** sobre el sustentador,
   **al menos 1 cada 15 m**.
4. **Anclaje final:** se intercala **cabrestante + dinamómetro**, se eleva el tense
   al nominal, se fija en el **punto fijo**, se desbloquean las poleas y se añaden
   **rodelas de contrapeso** para conseguir el sobretense. La interrupción de la
   secuencia no debe superar las **24 h**.
5. **Ajuste definitivo (tras el sobretense):** se retiran las rodelas en exceso, el
   sustentador pasa a su conjunto de suspensión, y se ajustan **D** (Anejo 2) y
   **Dv** (Anejo 3) según la temperatura en el momento del tendido.

> Control posterior: vigilar las descompensaciones por dilatación durante **al
> menos 30 días** tras el montaje; los reajustes forman parte del propio proceso.

### 3.3. Sobretense — por qué y cuánto

- **Tense nominal de diseño:** el definido por diseño (tablas de cada catenaria).
- **Tense de tendido:** fuerza durante la instalación; idealmente el nominal.
- **Sobretense:** incremento **máximo del 20 % sobre el tense nominal**, aplicado
  tras el tendido para eliminar las tensiones residuales del cable. Se mantiene un
  **mínimo de 24 h (recomendable 48 h)**.
- En **compensaciones tipo muelle**, si el sobretense se aplica en horas calurosas
  o con fuerte gradiente térmico, se revisa periódicamente o se añade un porcentaje
  suplementario para compensar pérdidas.

### 3.4. Tabla de tenses del sustentador (Anejo I, Tabla 1)

Valores en **kgf** (una fila por tipo de catenaria). La tensión de tendido máxima
se obtiene con un **coeficiente Cs = 1,7** (UNE-EN 50119 + IFE, hilo sin desgaste).

| Catenaria | Sustentador | Rotura (kgf) | Tense nominal (kgf) | Sobretense (kgf) | Tendido máx (kgf) | Tendido mín (kgf) |
|-----------|-------------|--------------|----------------------|------------------|-------------------|-------------------|
| CA-160 Tipo A | Cu ETP 150 | 5.708 | 1.425 | 285 | 3.357 | 300 |
| CA-160 Tipo B | Cu ETP 150 | 5.708 | 1.425 | 285 | 3.357 | 300 |
| CA-160H/3kV | Cu ETP 150 | 5.708 | 1.425 | 285 | 3.357 | 300 |
| CA-200H/3kV | Cu ETP 150 | 5.708 | 1.650 | 330 | 3.357 | 300 |
| CA-220/3kV | Cu ETP 185 | 6.843 | 2.475 | 495 | 4.025 | 300 |
| CA-200/25kV | Cu ETP 95 | 3.593 | 1.575 | 315 | 2.113 | 300 |
| CA-220/25kV | Cu ETP 95 | 3.593 | 1.575 | 315 | 2.113 | 300 |
| CA-160H/25kV | Cu ETP 150 | 5.708 | 1.425 | 285 | 3.357 | 300 |
| CA-200H/25kV | Cu ETP 150 | 5.708 | 1.650 | 330 | 3.357 | 300 |
| SICAT H1.0 | BZ II 120 | 6.757 | 2.142 | 428 | 3.974 | 500 |
| C-350 (TR 250 / TR 200) | Cu ETP 95 | 3.593 | 1.575 | 315 | 2.113 | 500 |

### 3.5. Tabla de tenses del hilo de contacto (Anejo I, Tabla 2)

| Catenaria | Hilo | Rotura (kgf) | Tense nominal (kgf) | Sobretense (kgf) | Tendido máx (kgf) | Tendido mín (kgf) |
|-----------|------|--------------|----------------------|------------------|-------------------|-------------------|
| CA-160 Tipo A | BC 107 CuETP | 3.560 | 1.050 | 210 | 2.094 | 300 |
| CA-160 Tipo B | BC 120 CuAg0,1 | 3.992 | 1.200 | 240 | 2.348 | 300 |
| CA-160H/3kV | BC 120 CuAg0,1 | 3.992 | 1.200 | 240 | 2.348 | 300 |
| CA-200H/3kV | BC 120 CuAg0,1 | 3.992 | 1.500 | 300 | 2.348 | 300 |
| CA-220/3kV | BC 150 CuAg0,1 | 4.991 | 1.875 | 375 | 2.935 | 300 |
| CA-200/25kV | BC 120 CuAg0,1 | 3.992 | 1.575 | 315 | 2.348 | 300 |
| CA-220/25kV | BC 150 CuAg0,1 | 4.991 | 1.875 | 375 | 2.935 | 300 |
| CA-160H/25kV | BC 120 CuAg0,1 | 3.992 | 1.200 | 240 | 2.348 | 300 |
| CA-200H/25kV | BC 120 CuAg0,1 | 3.992 | 1.500 | 300 | 2.348 | 300 |
| SICAT H1.0 | AC-120 CuMg0,5 | 5.596 | 2.753 | 530 * | 3.291 | 500 |
| C-350 | BC 150 CuMg0,5 | 6.702 | 3.150 | 630 | 3.942 | 500 |
| C-350 TR 250 | BC 150 CuMg0,5 | 6.702 | 2.100 | 420 | 3.942 | 500 |
| C-350 TR 200 | BC 150 CuMg0,5 | 6.702 | 1.575 | 315 | 3.942 | 500 |

*En SICAT H1.0 el sobretense queda limitado a 530 kgf por el tense de tendido máximo.

**Conductores:** sustentador Cu ETP según UNE 207015 y ET 03.364.158.0
(Cu 95/150/185 mm²); hilos según UNE-EN 50149 y ET 03.364.291.9
(BC 107 CuETP, BC 120 CuAg0,1, BC 150 CuAg0,1, BC 150 CuMg0,5, AC 120 CuMg0,5).

### 3.6. Coeficiente de dilatación

Para el cobre (único valor de la norma): **α = 1,7 × 10⁻⁵ °C⁻¹**.

### 3.7. Anejo 2 — Desplazamiento horizontal de ménsula (D)

**Fórmula: D = L₀ · α · ΔT · 1000** (resultado en **mm**)

- **L₀**: distancia de la ménsula al **punto fijo** (m)
- **ΔT = Tt − Tm**: temperatura de tendido − temperatura media de la zona (°C)
- **D negativo →** desplazamiento hacia el punto fijo; **D positivo →** hacia el
  lado contrario.

> **Ejemplo:** Tm = 15 °C, Tt = 25 °C (ΔT = +10 °C), L₀ = 600 m →
> D = 600 × 1,7·10⁻⁵ × 10 × 1000 = **102 mm** (positivo).

### 3.8. Anejo 3 — Desplazamiento vertical de los contrapesos (Dv)

**Fórmula: Dv = L₀ · α · ΔT · 100 · Rt** (resultado en **cm**)

- **L₀**: distancia del **semicantón** (m)
- **Rt**: factor de relación de compensación = **3 ó 5** (razones de polea 1:3, 1:5)
- **Referencia:** el punto medio del tubo guía (Dv = 0 = posición del bloque de
  contrapesos a la temperatura media anual). **Dv positivo →** ascendente;
  **Dv negativo →** descendente.

> **Ejemplo:** L₀ = 410 m, Rt = 1:5, Tt = 20 °C, Tm = 30 °C →
> Dv = 410 × 1,7·10⁻⁵ × (−10) × 100 × 5 = **−34,85 cm** (el centro de los
> contrapesos desciende 34,85 cm respecto al centro del tubo guía).

### 3.9. Utillaje y requisitos numéricos

| Elemento | Requisito |
|----------|-----------|
| Ganchos de tendido | Cobre, extremos redondeados en U; ≥ 1 cada 15 m; prohibido acero corrugado |
| Poleas de tendido | Garganta ≥ 2 × Ø cable; paredes con pendiente ≥ 15°; base de garganta ≥ Ø + 10 %; cojinetes de bolas/rodillos; superficie lisa |
| Ángulo de despegue | ≤ 45° |
| Dinamómetro | Precisión 2 % de la escala (0,5 % digital) |
| Termómetro | Digital, ±1 °C |
| Interrupción de montaje | Reanudar en < 24 h |
| Control post-montaje | ≥ 30 días (descompensaciones por dilatación) |

---

## 4. NAE 116 — CÁLCULO Y MONTAJE DEL PENDOLADO

### 4.1. Tipos de pendolado (apdo. 5)

| Tipo | Característica |
|------|----------------|
| **Arbitrario** | Distancia apoyo–1ª péndola y entre péndolas **variable** |
| **Equidistante** | Distancia **uniforme** entre péndolas (salvo la anterior/posterior al apoyo) |
| **Por parejas** | Distancia uniforme **dentro de cada pareja y entre parejas** (salvo las parejas junto al apoyo) |

Según el **tipo de vía** (Tabla 1 de la norma):

| Tipo de vía | CA-160 | CA-220 |
|-------------|--------|--------|
| Vía **general** | Por parejas, péndolas **equipotenciales** (interior del par = 0,5 m) | ídem |
| Vía **secundaria** (sustentador de cobre) | Por parejas equipotenciales (0,5 m) | ídem |
| Vía **secundaria** (con sustentador de acero / tipo C) | Equidistante-arbitraria, péndolas de varilla (Co7/Co8) | Por parejas equidistante, equipotenciales |

### 4.2. Criterios de cálculo (apdos. 4 y 6)

- **Elasticidad media del sistema: 3 mm/kg** (CA-160 y CA-220).
- **Fuerza del pantógrafo:** estática **8–12 kg**; en dinámica crece con el cuadrado
  de la velocidad; para el cálculo dinámico se usa una fuerza de empuje de **15 kg**.
- **Descentramiento:** referencia = avance de la kilometración. **Negativo =
  izquierda**; **positivo = derecha**. En CA-160/CA-220 el sustentador se descentra
  igual que los hilos (mismo plano vertical).
- **Peso soportado por cada péndola:** su propio peso + la mitad del peso de los
  hilos a cada lado.
- **Longitud de la péndola:** se mide entre los **ejes medios del sustentador y del
  hilo de contacto**; deriva de las **flechas del sustentador y del hilo** (datos de
  salida del cálculo).
- **Pendiente de vía:** se ignora si es **≤ 1 ‰**.
- **Desgaste del hilo:** < 10 % de la sección nominal → se trata como nuevo; > 10 % →
  peso real y tense reducido proporcionalmente. Si el coeficiente de seguridad cae a
  **K ≤ 2** en la sección útil, **no se cambia el pendolado**: se reduce el tense y
  se vuelve a subir K.
- **Vano de elevación en seccionamiento:** zona común de frotamiento normal
  **50–100 %**, admisible **15–50 %**, no admitida **< 15 %** salvo autorización
  expresa de la Dirección facultativa.

### 4.3. Coeficientes de seguridad (Tabla 8)

| Sustentador | Hilos de contacto * | Cables de colas | Piezas de anclaje | Grapas de anclaje |
|-------------|---------------------|-----------------|-------------------|-------------------|
| **3** | **2,5** | **3** | **3** | = carga de rotura del cable |

*Teniendo en cuenta el máximo desgaste permitido. Las tensiones se determinan por
estudios de interacción pantógrafo–catenaria según tipología y velocidad.

### 4.4. Tenses y contrapesos (Tablas 2 y 3)

**Tense mecánico = peso total del contrapeso × razón de regulación.**

| | Cu 150 — CA-160 A | Cu 150 — CA-160 B | Cu 185 — CA-220 |
|---|---|---|---|
| Tense (kgf) | 1.425 | 1.425 | 2.475 |
| Contrapeso razón 1:3 | 475 kg | 475 kg | 825 kg |
| Contrapeso razón 1:5 | 285 kg | 285 kg | 495 kg |

| Hilo | 2HC 107 (A) | 2HC 120 (B) | 1HC 107 (C) | 2HC 150 (CA-220) |
|---|---|---|---|---|
| Tense 1:3 (kgf) | 2×1.050 | 2×1.200 | 1.050 | — |
| Contrapeso 1:3 | 700 | 800 | 350 | — |
| Tense 1:5 (kgf) | 2×1.050 | 2×1.200 | 1.050 | 2×1.875 |
| Contrapeso 1:5 | 420 | 480 | 210 | 750 |

### 4.5. Materiales (Tablas 4 a 7)

**Sustentador:**

| | Cu 150 | Cu 185 |
|---|---|---|
| Sección nominal (mm²) | 147,1 | 184,5 |
| Nº de hilos / estructura | 37 · 1+6+12+18 | 37 · 1+6+12+18 |
| Diámetro aparente (mm) | 15,75 | 17,64 |
| Peso lineal (kg/m) | 1,344 | 1,687 |
| Carga de rotura | 58,25 kN (5.938 kg) | 67,1 kN (6.844 kg) |
| Módulo elástico (kg/mm²) | 10.500 | 10.500 |
| α (°C⁻¹) | 17×10⁻⁶ | 17×10⁻⁶ |
| Resistencia 20 °C (Ω/km) | 0,124 | 0,099 |

**Hilos de contacto (CuETP y CuAg0,1; módulo 12.800 kg/mm²):**

| | HC 107 | HC 120 | HC 150 |
|---|---|---|---|
| Sección nominal (mm²) | 107 | 120 | 150 |
| Ø nominal (mm) | 12,24 | 12,85 | 14,50 |
| Peso (kg/m) | 0,951 | 1,067 | 1,334 |
| Rotura CuETP (kg) | 3.700 | 3.914 | 4.597 |
| Rotura CuAg0,1 (kg) | 3.700 | 4.153 | 5.132 |
| Resistencia 20 °C (Ω/km) | 0,171 | 0,153 | 0,122 |

**Péndolas:**

| Tipo | Ø (mm) | Peso (kg/m) |
|------|--------|-------------|
| Varilla Cu | 5 | 0,174 |
| Cable flexible 25 mm² | 5,8 | 0,234 |

### 4.6. Distribución de péndolas por parejas (apdo. 9)

Son **tablas de referencia**; para cada caso particular se hace un cálculo específico.

**CA-160 Tipos A y B — vías generales** (interior del par = 0,50 m; Tabla 9):

| Vano (m) | Péndolas | Parejas | 1ª péndola (m) | Entre parejas (m) |
|----------|----------|---------|----------------|-------------------|
| 60,00 | 18 | 9 | 4,75 | 5,75 |
| 54,00 | 16 | 8 | 4,70 | 5,80 |
| 50,00 | 16 | 8 | 4,80 | 5,20 |
| 48,00 | 14 | 7 | 4,70 | 5,85 |
| 42,00 | 14 | 7 | 4,70 | 4,85 |
| 41,50 | 12 | 6 | 4,75 | 5,80 |
| 38,00 | 12 | 6 | 4,75 | 5,10 |
| 35,50 | 10 | 5 | 4,70 | 5,90 |
| 30,00 | 10 | 5 | 4,75 | 4,50 |
| 29,00 | 8 | 4 | 4,80 | 5,80 |
| 25,00 | 8 | 4 | 4,75 | 4,50 |
| 23,00 | 6 | 3 | 4,85 | 5,90 |
| 20,00 | 6 | 3 | 4,75 | 4,50 |

**CA-220 — vías generales** (interior del par = 0,50 m; Tabla 11). La misma tabla
figura en el **Anejo II de la NAE 301** (ver Lección 2): 60 m → 16 péndolas / 8
parejas (1ª a 5,25 m, entre parejas 6,50); 40 m → 12/6; 32,5 m → 8/4; 20 m → 6/3.

**CA-160 Tipo C — vías secundarias, 1 hilo, pendolado equidistante (Tabla 10):**
cada 6 m (vanos 30–60) o cada 5 m (20–29), alternando 1ª péndola a 3,00/5,50 m.

> **Aplicación conjunta:** los tenses de la Lección 2 (NAE 300/301) coinciden con
> los de esta norma (NAE 116), lo que permite fijar **primero el tense** (Lección 2)
> y **después distribuir las péndolas** con estas tablas.

### 4.7. Péndolas en agujas y seccionamientos (apdo. 6.13–6.14)

- **Vano de elevación de seccionamiento:** hay tipos con y sin eje; se distinguen
  tres zonas — **pendolado**, **elevación** y **transición** (de la elevación al
  semieje donde inicia la cola de anclaje).
- **Vano de elevación de aguja tangencial:** zona de pendolado (hasta el P25 del
  desvío), zona de elevación (desde el P50 hasta la altura de montaje) y, si
  procede, zona de transición. Datos de entrada: distancia del P25 al punto de
  aguja y distancia entre ejes de vía general y desviada.
- **Vano de elevación de aguja cruzada:** zona de pendolado + zona de elevación
  (desde el punto común de frotamiento hasta la altura de montaje en el perfil de
  elevación). **En este montaje no se considera flecha en los hilos.**
- La elevación (y) a una distancia (x) se calcula con la tensión mecánica (T) y el
  peso (P) del hilo: `y = f(x, T, P)`.

### 4.8. Montaje (apdo. 8)

1. **Verificaciones previas:** longitud del vano y altura de catenaria en los apoyos.
2. **Marcado:** medir sobre el hilo con **flexómetro calibrado** desde un apoyo;
   marcar con **rotulador de tinta indeleble** (nunca limas ni sierras).
3. **Montaje:** de un apoyo al otro, una a una; primero la grifa sobre el
   sustentador (sin apriete excesivo) y después la grifa del hilo; ajustar la grifa
   del sustentador para que la péndola quede **vertical**.
4. **Verificación final:** altura del hilo y flecha inicial.
- Muestreo: mínimo **dos péndolas por vano** antes del montaje (longitudes según
  cálculo y tolerancias).
- Las grifas se montan con **par de apriete** (Libro de LAC) y **llaves
  dinamométricas obligatorias**.

---

## 5. TABLA MAESTRA — TENSADO vs PENDOLADO

| Aspecto | NAE 108 (tensado) | NAE 116 (pendolado) |
|---------|--------------------|----------------------|
| Objetivo | Materializar el tense de diseño | Materializar la geometría (hilo a su altura) |
| Parámetro central | Tense nominal + sobretense | Flechas de sustentador e hilo |
| Cálculo clave | D y Dv por temperatura | Longitud de cada péndola |
| Referencia de temperatura | Tm (media anual de la zona) | — |
| Herramientas | Poleas, cabrestante, dinamómetro, rodelas | Flexómetro, rotulador, llaves dinamométricas |
| Coef. de seguridad | Cs = 1,7 en tendido | Sustentador 3 · hilo 2,5 · colas 3 · piezas 3 |
| Compensación | Rodelas de contrapeso (razón 1:3/1:5) | — |

---

## 6. PREGUNTAS DE AUTOEVALUACIÓN

1. ¿Por qué se sobretensa el cable tras el tendido y cuánto tiempo se mantiene?
2. ¿Qué porcentaje máximo de sobretense se aplica sobre el tense nominal?
3. Tense nominal y sobretense del sustentador de la CA-220/3kV (185 mm²) y de los
   hilos 2×BC-150.
4. Tensión de tendido máxima y mínima de un sustentador de CA-160 (¿de dónde sale
   el valor máximo?).
5. ¿Qué es Cs = 1,7 y sobre qué se aplica?
6. Fórmula y unidades de D (Anejo 2). Si se tiende 10 °C por encima de la media a
   600 m del punto fijo, ¿hacia dónde se desplaza la ménsula?
7. Fórmula y unidades de Dv (Anejo 3). ¿Qué representan Rt = 3 y Rt = 5?
8. ¿Cuál es el valor del coeficiente de dilatación del cobre?
9. Diferencias entre pendolado arbitrario, equidistante y por parejas.
10. ¿Qué pendolado se emplea en vías generales de CA-160 y CA-220? ¿Y en vías
    secundarias con sustentador de acero?
11. Elasticidad media del sistema y fuerzas del pantógrafo (estática y dinámica).
12. Regla de signos del descentramiento y a partir de qué se mide.
13. Coeficientes de seguridad del sustentador, hilo de contacto y colas.
14. Contrapeso (razón 1:5) de los hilos 2×120 de la CA-160 Tipo B. ¿Y razón 1:3?
15. Vano de 54 m en CA-160 vía general: número de péndolas, parejas y distancia
    entre parejas.
16. Vano de 40 m en CA-220 vía general: número de péndolas y parejas.
17. ¿Qué se hace si el hilo tiene más de un 10 % de desgaste? ¿Y si el coeficiente
    de seguridad baja de 2?
18. Zonas de un vano de elevación de seccionamiento y zona común de frotamiento
    admisible.
19. Material y peso de las péndolas (varilla y cable flexible).
20. ¿Con qué herramienta se mide y marca la posición de las péndolas?

---

## 7. REFERENCIAS

- **NAE 108** (2ª ed., dic 2025): objeto/campo, proceso de tendido (apdo. 5),
  tense y sobretense (apdo. 7), Anejo I (tablas de tense), Anejo 2 (D), Anejo 3
  (Dv), Anejo 4 (mapa de temperaturas)
- **NAE 116** (1ª ed. + M1, ene 2019): tipos de pendolado (5), criterios de cálculo
  (4 y 6), coefs. de seguridad (7.6), materiales (7.1–7.3), tenses (6.15),
  distribución por parejas (9), montaje (8)
- Complementarias: NAE 300/301 (tenses de diseño — Lección 2), NAE 115 (agujas —
  Lección 4), ET 03.364.158.0 (sustentador), ET 03.364.291.9 (hilo ranurado),
  UNE-EN 50119, UNE-EN 50149
- IFE (TMA/135/2023): 4.1.2.2.1.2 desviación lateral del hilo; UNE-EN 50125-2
  (temperaturas)

---

*Próxima lección: agujas aéreas (NAE 115) — geometría del P-50/P-90, replanteo y
montaje.*
