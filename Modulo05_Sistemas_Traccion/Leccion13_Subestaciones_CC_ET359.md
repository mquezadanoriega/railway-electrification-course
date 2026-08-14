# MÓDULO 5 · LECCIÓN 13
# LA SUBESTACIÓN DE TRACCIÓN EN CORRIENTE CONTINUA (3 kV Y 1,5 kV)

## Serie ET 03.359 — Especificaciones técnicas de subestaciones de tracción

> **Documentos base:** serie **ET 03.359.1xx / 5xx** de Adif, especificaciones de
> subestaciones de tracción (grupo de trabajo GT-301 «Subestaciones»). Las aplicables
> a los sistemas de corriente continua (3,3 kV y 1,5 kV) son:
>
> - **ET 03.359.101.7 +M1** — Transformadores de potencia sumergidos en aceite, 3.300 y
>   6.600 kVA, para SS/EE de tracción de 3,3 kV CC.
> - **ET 03.359.121.5 ED2+M1+M2** — Transformadores secos, 3.300 y 6.600 kVA, para SS/EE de
>   tracción de 3,3 kV CC.
> - **ET 03.359.104.1 3ª edición +M1** (ene 2020) — Rectificadores de potencia para SS/EE
>   de tracción de 3,3 kV CC (3.000 / 6.000 kW).
> - **ET 03.359.115.7 ED2+M1+M2** — Bobina de alisamiento del grupo transformador-rectificador.
> - **ET 03.359.106.6 1ª edición +M1** (ene 2020) — Rectificadores de potencia para SS/EE
>   de tracción de 1,5 kV CC (1.250 kW).
> - **ET 03.359.510.9 +M1** — Transformadores secos de 1.315 y 2.500 kVA para 1,5 kV CC.
> - **ET 03.359.511.7 +M1** — Transformadores de potencia sumergidos en aceite de 1.315 y
>   2.500 kVA para 1,5 kV CC.
> - **ET 03.359.100.9 4ª edición +M1** — Disyuntores extrarápidos de SS/EE (40 y 80 kA).
> - **ET 03.359.123.1 +M1+M2 (erratum)** — Cabinas de corriente continua (feeder y seccionadores).
> - **ET 03.359.108.2** — Analizador de línea aérea de contacto de las SS/EE de tracción.
> - **ET 03.359.110.8** — Gestor de protecciones 3,3 kV en SS/EE de tracción.
> - **ET 03.359.109.0** — Sistema de control automatizado mediante PLCs (10 partes).
> - **ET 03.359.116.5 ED3** — Transformadores de alimentación a servicios auxiliares (SSAA).

---

## 1. RESULTADO DE APRENDIZAJE

Al terminar esta lección serás capaz de:

1. Describir la **configuración tipo de una subestación de tracción en CC**: grupos
   transformador-rectificador, feeders, barras ómnibus y acoplamiento con SS/EE colaterales
2. Dimensionar el **grupo transformador-rectificador de 3,3 kV** con los datos reales de
   las ET (potencia, tensiones, corrientes básicas, clase de servicio)
3. Explicar la **función de la bobina de alisamiento** y sus valores característicos
4. Distinguir el **sistema de 1,5 kV** (configuración de 6 pulsos) del de 3,3 kV
   (configuración de 12 pulsos), con sus transformadores y rectificadores
5. Seleccionar el **disyuntor extrarápido** adecuado (40 u 80 kA) según la subestación
6. Conocer los **equipos de protección, medida y control**: analizador de LAC, gestor de
   protecciones 3,3 kV y sistema de control mediante PLCs
7. Saber dónde buscar cada dato dentro de la serie ET 03.359 (apartado exacto)

---

## 2. RESUMEN EJECUTIVO

La subestación de tracción en corriente continua (SET-CC) transforma la energía que recibe
de la red de transporte/distribución en **corriente continua de 3,3 kV o de 1,5 kV** para
alimentar la línea aérea de contacto (LAC). Es el corazón del sistema de tracción de la red
convencional española (3 kV CC), y también se emplea en líneas de ancho métrico (1,5 kV).

Cada SET-CC está formada, en esencia, por:

| Elemento | Función | ET de referencia |
|----------|---------|------------------|
| **Transformador de potencia** | Baja la tensión de la red a la tensión de alimentación del rectificador (1.300 V o 1.221 V) | 101.7 / 121.5 (3,3 kV) · 510.9 / 511.7 (1,5 kV) |
| **Rectificador de diodos** | Convierte la CA en CC (puentes de Graetz) | 104.1 (3,3 kV) · 106.6 (1,5 kV) |
| **Bobina de alisamiento** | Eleva la impedancia a armónicos y limita el di/dt en faltas | 115.7 |
| **Cabinas de CC** | Alojan disyuntores extrarápidos y seccionadores de feeder / grupo / barras | 123.1 |
| **Disyuntor extrarápido (DRE)** | Protege la LAC y los feeders contra cortocircuitos | 100.9 |
| **Analizador de LAC** | Verifica el estado de la catenaria antes de autorizar el reenganche | 108.2 |
| **Gestor de protecciones 3,3 kV** | Lógica de desconexiones de la propia S/E y de las colaterales | 110.8 |
| **Control mediante PLCs** | Mando, supervisión y telemando (CDMEIF) de la S/E | 109.0 |
| **Transformadores de SSAA** | Alimentan los servicios auxiliares de la propia S/E | 116.5 |

> **Regla de diseño:** los valores nominales (potencias, tensiones, corrientes) vienen
> **fijados por las ET**; el proyecto solo elige entre las potencias normalizadas
> (p. ej. rectificador de 3.000 ó 6.000 kW) y justifica la elección con el tráfico y la
> distancia entre SS/EE.

---

## 3. CONFIGURACIÓN GENERAL DE LA SET DE CC

El modelo tipo de subestación que emplean las ET 03.359.109.0 y 03.359.110.8 es:

```
  RED DE ALTA TENSIÓN (20 / 25 / 30 / 45 / 66 kV)
                          │
        ┌─────────────────┼─────────────────┐
        │                                     │
   Transformador SSAA              Seccionador de entrada AT
   (116.5, 100-400 kVA)                    │
        │                              GRUPO TRANSFORMADOR-RECTIFICADOR
   Servicios auxiliares                   Transformador (101/121 ó 510/511)
   (400/230 V)                                  │
                                        Rectificador de diodos (104/106)
                                              │
                                        Bobina de alisamiento (115)
                                              │
                              ┌───────────────┴───────────────┐
                         Cabina de grupo 1               Cabina de grupo 2
                              │                              │
                    BARRAS ÓMNIBUS (UBO) — acoplamiento entre grupos
                              │
              ┌───────────────┼───────────────────────────────┐
        Cabina feeder 1   Cabina feeder 2  …  Cabina feeder 6  (cada una: DRE + seccionadores)
              │                │                    │
        Seccionador         Seccionador         Seccionador
        de punta            de punta            de punta
              └────────────────┴────────────────────┘
                                    │
                              LÍNEA AÉREA DE CONTACTO
```

**Datos del modelo de S/E (ET 03.359.110.8, apdo. 1.3):**

- **Dos grupos rectificadores** (grupos transformador-rectificador)
- **Seis salidas de feeder** hacia la catenaria
- **Dos barras by-pass** y **acoplamiento por ambos lados** con las SS/EE colaterales
- Conexión para **subestación móvil** (S/E móvil) en el seccionador de entrada de AT

**Magnitudes de medida en los feeders (ET 03.359.108.2):**

| Sigla | Significado |
|-------|-------------|
| **UBO** | Tensión de barra ómnibus |
| **UF** | Tensión del feeder / de la Línea Aérea de Contacto |
| **Umin / Umáx** | Umbrales de tensión que gobiernan el cierre del DRE |

> La SET-CC **no trabaja sola**: las SS/EE colaterales se comunican entre sí (y con el
> CDMEIF, telemando de electrificación) para coordinar desconexiones y arrastres.

---

## 4. DATOS CLAVE — EL GRUPO TRANSFORMADOR-RECTIFICADOR DE 3,3 kV

### 4.1. Transformadores de potencia (ET 03.359.101.7 aceite · ET 03.359.121.5 seco)

Características comunes a ambas especificaciones:

| Parámetro | Valor |
|-----------|-------|
| Grupo de conexión | **Yy0d11** (dos secundarios: uno en estrella y otro en triángulo) |
| Potencia aparente básica | **3.300 ó 6.600 kVA** |
| Potencia de cada secundario | **1.650 kVA** (transformador de 3.300) · **3.300 kVA** (el de 6.600) |
| Tensión asignada de los secundarios | **1.300 V** (cada uno) |
| Regulación | Por tomas en el arrollamiento primario (todas de plena potencia) |
| Aislamiento | Pantalla entre bobinados AT y BT; nivel de aislamiento acorde a la tensión de alimentación |
| Clase de servicio | **IXA** (ciclo de carga del grupo rectificador) |

**ET 03.359.101.7 (baño de aceite):**

| Parámetro | 3.300 kVA | 6.600 kVA |
|-----------|-----------|-----------|
| Tensión de cortocircuito (75 ºC) | 9 % (cada secundario) · 10 % (ambos) | 9 % · 10 % |
| Pérdidas en vacío | 26.000 W | 45.000 W |
| Calentamiento del aceite (parte superior) | 45 K | 45 K |
| Rendimiento | > 99,3 % | > 99,2 % |
| Modo de refrigeración | ONAN | ONAN |
| Peso / dimensiones aprox. | 15.000 kg · 4.000×2.600×3.500 mm | 25.000 kg · 5.000×3.500×4.000 mm |
| Accesorios | Desecador de aire con sílice, indicador de nivel, termómetro y termostatos de aceite | igual |

**ET 03.359.121.5 (tipo seco):** mismas potencias (3.300 / 6.600 kVA), misma tensión de
secundarios (1.300 V) y mismo grupo **Yy0d11**. Peso aproximado 25.000 kg (3.300 kVA) y
35.000 kg (6.600 kVA).

### 4.2. Rectificador de potencia (ET 03.359.104.1)

| Parámetro | Valor |
|-----------|-------|
| Clasificación (UNE-EN 50328) | Convertidor CA→CC, rectificador de diodos, **tipo a.1** |
| Montaje | **Dos puentes trifásicos de Graetz**, montaje nº 12 de la tabla 4 de UNE-EN 50328 (12 pulsos) |
| Potencia | **3.000 kW ó 6.000 kW** |
| Tensión asignada de entrada | **1.300 V** a 50 Hz |
| Tensión asignada en CC | **3.300 V** (máx. 3.549 V · media 3.510 V · mín. 3.432 V) |
| Corriente básica continua | **909 A** (3.000 kW) · **1.818 A** (6.000 kW) |
| Clase de servicio | **IX** (tabla 5 de UNE-EN 50328) |
| Factor de utilización | 0,97 |
| Factor de ondulación (rizado) | 0,0172 |
| Pérdidas máximas admisibles | 6.000 W (3.000 kW) · 12.500 W (6.000 kW) |
| Distancia de aislamiento a masa | ≥ 120 mm |
| Niveles de aislamiento | 18,5 kV eficaz (50 Hz) · 40 kV cresta (impulso rayo 1,2/50 µs) |
| Condiciones de servicio | Interior, refrigeración AN, −5 ºC…+40 ºC, altitud ≤ 1.000 m, polución PD3A |
| Dimensiones máx. | 2.200×2.000×2.600 mm (3.000 kW) · 2.200×2.500×2.600 mm (6.000 kW) |

**Ciclo de carga de la clase IX (ET 03.359.104.1, apdo. 4.3.7):**

| Régimen | Capacidad acumulativa |
|---------|------------------------|
| (a) | **1,0 × corriente básica continua**, de manera permanente |
| (b) | **1,5 × corriente básica**, durante 2 horas (partiendo de (a)) |
| (c) | **3,0 × corriente básica**, durante 5 minutos (partiendo de (b)) |

**Componentes del rectificador (apdos. 4.6–4.7):**

- **Diodos** tipo *press-pack*: VRRM ≥ 4.400 V, VRSM ≥ 4.600 V, IF entre 1.800 y 2.420 A,
  VFM ≤ 2,90 V a 1.800 A, Rth(j-c) ≤ 41 ºC/kW. Número: 24–48 (3.000 kW) y 36–96 (6.000 kW),
  con configuración **np-1 por rama** (positiva y negativa).
- **Cartuchos fusibles ultrarrápidos** (uno por diodo): tipo **aR**, 2.000 V, poder de corte
  ≥ 50 kA, tensión de arco máx. 3.800 V.
- **Protecciones**: circuito R-C por rama (sobretensiones de conmutación), circuito R-C en el
  lado de CC (condensadores 4 / 10 / 20 / 40 µF, 4.000 Vcc de servicio, UNm 4.800 Vcc) y
  **protección por temperatura**: alarma a **90 ºC**, desconexión a **100 ºC**.
- **Señales al control**: alarma/desconexión por temperatura y por fusión de cartuchos, por
  fibra óptica o transformador de aislamiento (ensayo 18,5 kV, 60 s).

### 4.3. Bobina de alisamiento (ET 03.359.115.7)

Se instala **en conexión serie a la salida del rectificador**. Proporciona impedancia elevada
a las corrientes armónicas y reduce el incremento de corriente en las faltas de CC.

| Parámetro | Valor |
|-----------|-------|
| Tipo | Seca, **núcleo de aire**, sin pantalla magnética, interior, refrigeración AN |
| Inductancia incremental asignada (Linc) | **0,6 mH** |
| Corriente continua permanente asignada (Id) | **909 A** (grupo 3.000 kW) · **1.818 A** (grupo 6.000 kW) |
| Tensión asignada de aislamiento (UNm) | **4,8 kV** (tabla 1 de UNE-EN 50123) |
| Clase de servicio | **IXA** (tabla A.1 de UNE-EN 50329, con IBd = IN) |
| Clase térmica del aislamiento | **155 (F)**, calentamiento medio máx. 100 K |
| Niveles de aislamiento | 18,5 kV eficaz (50 Hz, 60 s) · 40 kV cresta (rayo) |
| Corriente asignada de corta duración (INcw) | **10 kA** (grupo 3.000 kW) · **20 kA** (grupo 6.000 kW) |
| Sobrecargas de la clase IXA | 1,0 × IN permanente · 1,5 × IN (2 h) · 3,0 × IN (5 min) |

Sobrecargas concretas para el grupo de 3.000 kW: **1.364 A durante 2 horas** y **2.727 A
durante 5 minutos** (ET 03.359.115.7, apdo. 4.9).

---

## 5. DATOS CLAVE — EL SISTEMA DE 1,5 kV

### 5.1. Rectificador (ET 03.359.106.6)

| Parámetro | Valor |
|-----------|-------|
| Montaje | **Un puente trifásico de Graetz**, montaje nº 8 de la tabla 4 de UNE-EN 50328 (6 pulsos) |
| Potencia | **1.250 kW** |
| Tensión asignada de entrada | **1.220 V** a 50 Hz |
| Tensión asignada en CC | **1.650 V** (máx. 1.720 V · media 1.647 V · mín. 1.488 V) |
| Corriente básica continua | **758 A** |
| Clase de servicio | **IX** (1,0 × IN permanente · 1,5 × IN 2 h · 3,0 × IN 5 min) |
| Factor de utilización | 0,95 |
| Factor de ondulación (rizado) | 0,042 |
| Pérdidas máximas admisibles | 2.000 W |
| Niveles de aislamiento | 9,2 kV eficaz (50 Hz) · 20 kV cresta (rayo 1,2/50 µs) |
| Dimensiones máx. | 1.400×1.200×1.850 mm |
| Diodos | 12–18, tipo *press-pack*, con configuración np-1 |
| Condensadores R-C (lado CC) | 2.000 Vcc de servicio, UNm 3.000 Vcc, 4 / 10 / 20 / 40 µF |

### 5.2. Transformadores (ET 03.359.510.9 secos · ET 03.359.511.7 aceite)

| Parámetro | ET 03.359.510.9 (seco) | ET 03.359.511.7 (aceite) |
|-----------|-------------------------|---------------------------|
| Grupo de conexión | **Yd11** | **Yd11** |
| Potencia básica | 1.315 y 2.500 kVA | 1.315 y 2.500 kVA |
| Tensión asignada del secundario | **1.221 V** (nivel 3 kV) | **1.221 V** (nivel 3 kV) |
| Tomas (primario) | 1.315 kVA: ±2,5 %; +5 %; +7,5 % · 2.500 kVA: ±2,5 %; +5 %; +7,5 % | 1.315: ±2,5 %; +5 %; +7,5 % · 2.500: ±2,5 %; ±5 % |
| Ucc | **10 %** (referida a 120 ºC) | **9,5 %** (1.315) · **9 %** (2.500), a 75 ºC |
| Pérdidas en vacío | — | 13.000 W (1.315) · 17.500 W (2.500) |
| Rendimiento | > 99,2 % / > 99,1 % (aprox.) | > 99,2 % (1.315) · > 99,1 % (2.500) |
| Refrigeración | Aire natural (seco, resina) | **ONAN** |
| Peso aprox. | 10.000 kg / 15.000 kg | 9.000 kg / 11.000 kg |

Corrientes asignadas de los secundarios (ET 03.359.510.9): **621,80 A** (1.315 kVA) y
**1.182,1 A** (2.500 kVA).

> **Diferencia clave 3,3 kV vs 1,5 kV:** el grupo de 3,3 kV usa **dos secundarios
> (estrella + triángulo, Yy0d11) → 12 pulsos**, mientras que el de 1,5 kV usa **un único
> secundario (Yd11) → 6 pulsos**. Esto se traduce en un factor de rizado mucho menor en
> 3,3 kV (0,0172 frente a 0,042).

---

## 6. DISYUNTORES EXTRARRÁPIDOS Y CABINAS DE CC

### 6.1. Disyuntores extrarápidos (ET 03.359.100.9)

Protegen la LAC y los feeders contra cortocircuitos en corriente continua. Cumplen los
requisitos de la **UNE-EN 50123-2** (interruptores automáticos de CC de tracción).

| Parámetro | Valor |
|-----------|-------|
| Tensión nominal (Un) | **1.500 V** |
| Constante de tiempo asignada de la vía (TNc) | **31,5 ms** |
| Corriente asignada de cortocircuito (INss) | **40 kA** (versión A) · **80 kA** (versión B) |
| Poder de corte / cierre asignado | **40 kA** · **80 kA** |
| Tiempo de apertura | **≤ 30 ms** |
| Rigidez dieléctrica (mando–tierra) | 2.000 Vca (50 Hz) |

Para líneas electrificadas en 3,3 kV se definen dos familias de corriente asignada del
disyuntor: **entre 1.250 A y 2.700 A** y **entre 2.000 A y 5.000 A**.

> El disyuntor extrarápido (DRE) es un **interruptor automático de línea** (punto de
> instalación L) de actuación muy rápida, adecuado para el régimen de cortocircuito de la
> tracción en CC, que además soporta el **cierre sobre falta** (la verificación previa de
> la catenaria la realiza el analizador de LAC, apdo. 7.1).

### 6.2. Cabinas de CC (ET 03.359.123.1)

Las cabinas alojan la aparamenta de potencia y control de la parte de CC. Se definen tres
tipos:

| Tipo de cabina | Función |
|----------------|---------|
| **Cabina de feeder** | Disyuntor extrarápido + seccionador de salida de feeder + seccionador de by-pass (diseño **desenchufable**) |
| **Cabina de seccionador de grupo 1** | Seccionador de salida de grupo 1 + seccionador de conexión de subestación móvil |
| **Cabina de seccionador de grupo 2** | Seccionador de salida de grupo 2 + seccionador de unión de **barras ómnibus** |

**Características (apdo. 4):**

| Parámetro | Valor |
|-----------|-------|
| Corriente asignada de servicio de barras y circuitos (INe) | **2.700 A** |
| Corriente soportada de corta duración de barras (INcw) | **50 kA** |
| Nivel de tensión soportada del embarrado negativo | 5 kV (50 Hz, 1 min) |
| Nivel de tensión soportada de la cabina | 2 kV (frecuencia industrial) |
| Dimensiones máx. | 800 × 2.300 × 1.450 mm |
| Envolvente | Chapa de acero laminado en frío o inoxidable, aislamiento al aire |

- Envolvente metálica; los embarrados principales se forman con **dos pletinas**.
- La cabina de feeder dispone de amperímetro y voltímetro de salida, señalización de posición
  del DRE y de los seccionadores, y rótulo «feeder X».
- **Transductores de intensidad** específicos para electrificaciones de 3,3 kV y de 1,5 kV.
- Los enclavamientos son mecánicos y eléctricos; accionamientos eléctricos de seccionadores
  según ET 03.364.151.5.

---

## 7. PROTECCIÓN, MEDIDA Y CONTROL

### 7.1. Analizador de línea aérea de contacto (ET 03.359.108.2)

Cuando un disyuntor extrarápido dispara por un defecto en la catenaria, el analizador de LAC
es quien decide si se puede **autorizar el reenganche** del disyuntor. Para ello:

1. **Comprueba el estado de sus propios equipos de medida** (tensión de barra UBO y tensión
   de feeder UF, fusibles y circuitos de medida) antes de emitir ningún permiso.
2. Realiza el **análisis de aislamiento** de la catenaria (medida de resistencia de la línea)
   y el **análisis de diferencia de tensión** entre los extremos del disyuntor.
3. Si el defecto ha desaparecido, **autoriza el cierre** del DRE; si persiste, lo **bloquea**.
4. Registra cada prueba de cortocircuito, cada diferencia de tensión y cada bloqueo
   (registro histórico con códigos de evento, p. ej. 1300 = cierre intempestivo).

Datos de referencia (apdo. de ensayos): **Umin de catenaria > 600 V con 150.000 mΩ a
3.300 V**; rigidez de maniobra y entrada/salida del analizador 15 kV (1 min) y 35 kV
(impulso 1,2/50 µs); aislamiento > 10⁴ MΩ a 5 kV cc.

> El analizador convierte el **reenganche automático** en una operación segura: el DRE no se
> recieira sobre una catenaria que sigue en falta.

### 7.2. Gestor de protecciones 3,3 kV (ET 03.359.110.8)

Equipo que, mediante una lógica determinada, **supervisa permanentemente los órganos de la
subestación** y efectúa las desconexiones correspondientes en la propia S/E y en las SS/EE
**colaterales**. Aplicaciones: subestaciones de tracción de CC y centros de puesta en
paralelo de catenarias de CC.

- Parámetro clave: **tiempo de diagnosis–actuación ≤ 4 ms**.
- Módulos: **lógica centralizada**, **entradas–salidas**, **visualización de E/S (unifilar
  de la S/E)** y **supervisión de salidas relés**.
- Entradas–salidas mínimas para una S/E con **2 grupos rectificadores, 6 salidas de feeders
  y 2 barras by-pass**, más un 5 % para ampliaciones.

Funciones típicas (apdo. 2.2):

| Función | Objeto |
|---------|--------|
| Puesta a masa de grupo/s | Descarga y seguridad tras desconexión |
| Puesta a masa de feeders y de pórtico | Idem sobre la catenaria |
| Detección de **bombeo de un disyuntor extrarápido** | Evita cierres repetidos sobre falta |
| Indefinición de posición en seccionadores | Salida de grupo, unión de BB/OO, salida de feeder, by-pass, punta de feeders (A), unión de vía impar (B) y par (C) en la LAC |
| Orden de desconexión de S/E colateral | Recepción de arrastre entre SS/EE |
| Fallo de comunicaciones entre SS/EE | Tratamiento de pérdida de enlace |
| Registro histórico de eventos y de marcha–paro | Trazabilidad de maniobras |

### 7.3. Sistema de control automatizado mediante PLCs (ET 03.359.109.0)

Especificación en **10 partes** que define el sistema de control de las SS/EE de tracción:

| Parte | Contenido |
|-------|-----------|
| 01 | Generalidades (objeto, arquitectura de red, PLCs y puestos de control) |
| 02 | Línea de acometida en AT |
| 03 | Servicios auxiliares y medida |
| 04 | Línea de señales de tráfico |
| 05 | Grupo transformador-rectificador |
| 06 | Salida de feeder |
| 07 | Pórtico de seccionadores |
| 08 | Puesto de control centralizado |
| 09 | Adaptador de red |
| 10 | Gestor de protecciones |

Ideas clave:

- Los elementos de la S/E se agrupan en **bloques eléctricos**, cada uno controlado por un
  **PLC**; la red es **descentralizada**, con un **bus de comunicaciones común**.
- Cada PLC lee y analiza la información de los órganos que controla y la distribuye al resto
  de PLCs y a los archivos generales.
- El sistema sustituye a los **relés intermedios del telemando** y permite el control
  completo de la S/E, con **mando local y telemando**.
- Equipos de la red: PLC de cada bloque, **PLC gestor de protecciones 3,3 kV**, **PLC
  archivo-memoria**, **PC puesto de control local centralizado** y **puesto de control
  CDMEIF** (telemando de electrificación, por cable).
- Los PLCs incorporan CPU programable (diagramas de funciones secuenciales), tarjetas de E/S
  separadas galvánicamente, fuentes de alimentación y modos de funcionamiento (marcha/paro)
  con supervisión de estados.

### 7.4. Transformadores de servicios auxiliares (ET 03.359.116.5)

Alimentan los servicios auxiliares de la propia subestación (alumbrado, mando, carga de
baterías, climatización…):

| Parámetro | Valor |
|-----------|-------|
| Potencias asignadas | **100, 160, 250 y 400 kVA** |
| Tensión asignada del primario | **20, 25, 30, 45 y 66 kV** |
| Tensión asignada del secundario | **240 V** |
| Grupo de conexión | **Yzn11** |
| Tipos | Baño de aceite y tipo seco |
| Clase térmica (tipo seco) | 155 (F) |

---

## 8. APLICACIÓN PRÁCTICA AL DISEÑO DE UNA SET

Secuencia de diseño de una subestación de tracción en CC 3,3 kV:

1. **Definir la demanda**: tráfico, material rodante y longitud del cantón → potencia del
   grupo. El proyecto elige entre **3.000 ó 6.000 kW** (ET 03.359.104.1) y, en consecuencia,
   el transformador de **3.300 ó 6.600 kVA** (ET 03.359.101.7 / 121.5).
2. **Seleccionar el rectificador**: dos puentes de Graetz (montaje nº 12), 1.300 V entrada,
   3.300 V salida, 909 A (3.000 kW) o 1.818 A (6.000 kW), clase IX.
3. **Verificar la bobina de alisamiento**: 0,6 mH, 909/1.818 A, 4,8 kV de aislamiento,
   clase IXA (ET 03.359.115.7).
4. **Elegir el disyuntor extrarápido**: 40 kA (SS/EE con menor corriente de cortocircuito) u
   80 kA, apertura ≤ 30 ms, TNc 31,5 ms (ET 03.359.100.9).
5. **Configurar las cabinas de CC**: feeder (desenchufables), seccionadores de grupo 1 y 2,
   unión de barras ómnibus; INe 2.700 A, INcw 50 kA (ET 03.359.123.1).
6. **Definir la protección y el control**: analizador de LAC por feeder (ET 03.359.108.2),
   gestor de protecciones 3,3 kV (ET 03.359.110.8) y control por PLCs con telemando CDMEIF
   (ET 03.359.109.0).
7. **Dimensionar los servicios auxiliares**: transformadores 100–400 kVA, 20–66 kV / 240 V,
   Yzn11 (ET 03.359.116.5).

> **Ejemplo tipo:** una SET de 6.000 kW → transformador Yy0d11 de 6.600 kVA (2 × 3.300 kVA a
> 1.300 V), rectificador de 12 pulsos 1.818 A, bobina de 0,6 mH/1.818 A, cabinas con
> disyuntores de 80 kA. Para una línea de 1,5 kV: rectificador de 1.250 kW (758 A), 6 pulsos,
> transformador Yd11 de 1.315 ó 2.500 kVA a 1.221 V.

---

## 9. PREGUNTAS DE AUTOEVALUACIÓN

1. ¿Qué dos potencias normalizadas admite la ET 03.359.104.1 para el rectificador de 3,3 kV?
2. ¿Qué corriente básica continua corresponde a cada potencia del rectificador de 3,3 kV?
3. ¿Cuál es el montaje rectificador del sistema de 3,3 kV (UNE-EN 50328)? ¿Y el del de 1,5 kV?
4. Clase de servicio de los rectificadores y capacidades acumulativas del ciclo de carga.
5. Grupo de conexión y potencia de los transformadores de 3,3 kV. ¿Qué tensión tienen sus secundarios?
6. ¿Qué inductancia incremental tiene la bobina de alisamiento? ¿En qué conexión se instala?
7. ¿Qué clase de servicio (UNE-EN 50329) y qué corriente continua permanente asignada tiene la bobina?
8. Tensión asignada, máxima, media y mínima en CC del rectificador de 3,3 kV.
9. Potencia y corriente básica del rectificador de 1,5 kV. ¿Qué tensión tiene su entrada?
10. Grupo de conexión y potencias de los transformadores de 1,5 kV (secos y en aceite).
11. Tensión asignada de cortocircuito (Ucc) de los transformadores de 1,5 kV (510 y 511).
12. Constante de tiempo asignada de la vía y tiempo máximo de apertura del disyuntor extrarápido.
13. ¿Qué corrientes asignadas de cortocircuito definen los disyuntores extrarápidos?
14. Corriente asignada de servicio (INe) y de corta duración (INcw) de las barras de las cabinas.
15. ¿Qué tres tipos de cabinas de CC define la ET 03.359.123.1?
16. ¿Qué tensión y resistencia mínima se exigen a la catenaria en el análisis de aislamiento del analizador?
17. ¿Qué medidas realiza el analizador de LAC antes de autorizar el cierre del DRE?
18. Tiempo de diagnosis–actuación exigido al gestor de protecciones 3,3 kV.
19. Enumera al menos cinco funciones del gestor de protecciones (ET 03.359.110.8).
20. ¿En cuántas partes se estructura la ET 03.359.109.0 y qué controla cada una?
21. ¿Qué puestos y PLCs forman la red de control automatizado de la S/E?
22. Potencias y tensiones de los transformadores de servicios auxiliares (ET 03.359.116.5).
23. ¿Por qué el factor de rizado es menor en el sistema de 3,3 kV que en el de 1,5 kV?
24. ¿Qué señales envía el rectificador a los circuitos de control y cómo se garantiza el aislamiento?
25. ¿Qué niveles de aislamiento exige la ET 03.359.104.1 para el rectificador?

---

## 10. REFERENCIAS

- **ET 03.359.101.7 +M1** — Transformadores sumergidos en aceite 3.300/6.600 kVA, 3,3 kV CC
  (apdos. 4.1–4.3: grupo Yy0d11, potencias, Ucc, ONAN)
- **ET 03.359.121.5 ED2+M1+M2** — Transformadores secos 3.300/6.600 kVA, 3,3 kV CC
- **ET 03.359.104.1 3ª ed. +M1** — Rectificadores 3,3 kV CC (apdos. 4.3–4.9: montaje nº 12,
  3.000/6.000 kW, clase IX, tabla resumen 4.9)
- **ET 03.359.106.6 1ª ed. +M1** — Rectificadores 1,5 kV CC (montaje nº 8, 1.250 kW, clase IX)
- **ET 03.359.115.7 ED2+M1+M2** — Bobina de alisamiento (apdos. 4.2–4.9: Linc 0,6 mH, IXA)
- **ET 03.359.510.9 +M1** — Transformadores secos 1.315/2.500 kVA, 1,5 kV CC (Yd11, 1.221 V)
- **ET 03.359.511.7 +M1** — Transformadores aceite 1.315/2.500 kVA, 1,5 kV CC (Yd11, 1.221 V)
- **ET 03.359.100.9 4ª ed. +M1** — Disyuntores extrarápidos (40/80 kA, TNc 31,5 ms, ≤ 30 ms)
- **ET 03.359.123.1 +M1+M2** — Cabinas de CC (INe 2.700 A, INcw 50 kA)
- **ET 03.359.108.2** — Analizador de LAC de SS/EE de tracción
- **ET 03.359.110.8** — Gestor de protecciones 3,3 kV (≤ 4 ms, funciones apdo. 2.2)
- **ET 03.359.109.0** — Sistema de control automatizado mediante PLCs (partes 01–10)
- **ET 03.359.116.5 ED3** — Transformadores de SSAA (100–400 kVA, 240 V, Yzn11)
- UNE-EN 50328: convertidores de potencia de alimentación para tracción (montajes y clases)
- UNE-EN 50329: transformadores de tracción (clase de servicio de la bobina, tabla A.1)
- UNE-EN 50123: interruptores automáticos de CC de tracción (tabla 1 de aislamiento)

---

*Lección 12 / siguientes: seccionamiento y postes de seccionamiento, circuito de retorno y
protecciones de la LAC. Ver también Lección 1 (parámetros de la LAC, NAE 107) para los
requisitos de la catenaria que alimenta esta subestación.*
