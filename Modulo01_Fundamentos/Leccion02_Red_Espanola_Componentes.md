# MÓDULO 1 · LECCIÓN 2
# LA RED ESPAÑOLA Y SUS COMPONENTES

## La catenaria española: dos sistemas, una misma filosofía

---

## 1. RESULTADO DE APRENDIZAJE

Al terminar esta lección serás capaz de:

1. Describir los **dos sistemas de electrificación** españoles (3 kV CC y
   25 kV CA) y dónde se aplica cada uno
2. Nombrar e identificar los **componentes** del subsistema de energía: SET,
   línea de contacto (catenaria), feeder, retorno, seccionamientos
3. Explicar el **esquema general de alimentación** de una línea desde la red
   eléctrica hasta el pantógrafo
4. Distinguir las configuraciones **1x25 kV y 2x25 kV** en CA
5. Conocer los **límites eléctricos** de proyecto (tensión, corriente, fuga)

---

## 2. RESUMEN EJECUTIVO

España tiene **dos mundos eléctricos**:

- **Red convencional (RFIG): 3 kV CC.** Catenaria compuesta tipo «Y» o simple,
  con hilo de contacto de cobre de 107 mm², alimentada por subestaciones cada
  12–20 km con rectificadores de 3,3 kV. Es el sistema de cercanías, regionales
  y mercancías convencional.
- **Red de alta velocidad (LAV): 25 kV CA.** Catenaria CA-160, CA-220, CA-160H o
  CA-200H según velocidad (160–350 km/h), subestaciones cada 60–100 km, tensión
  27,5 kV en origen (transformadores con regulación). Es el sistema del AVE.

En el curso (Módulos 2 a 5) desarrollarás ambos en detalle; esta lección te da el
**mapa general** para que sitúes cada pieza.

---

## 3. ESQUEMA GENERAL DE ALIMENTACIÓN

```
RED ELÉCTRICA ESPAÑOLA (REE) 220 kV / 400 kV (50 Hz)
        │
        ▼
SUBESTACIÓN DE TRACCIÓN (SET)
   ├── CC: transformador 3,3 kV + rectificador de onda completa
   │       → barra de CC → DPL → catenaria
   └── CA: transformador 25 kV (o 2x25 kV) + regulación de tensión
           → barra de CA → DPL → catenaria
        │
        ▼
CANTÓN DE ALIMENTACIÓN (catenaria + retorno)
        │
        ▼
PANTÓGRAFO DEL TREN → transformador/motores → RETORNO (carril)
        │
        ▼
(CC)  tierra/retorno: hilos de retorno paralelos al carril
(CA)  carril + transformadores de separación → SET (neutro a tierra)
```

---

## 4. LA SET (SUBESTACIÓN DE TRACCIÓN)

### 4.1 En CC (3 kV)

- Entrada de **media/alta tensión** (hasta 220 kV) desde REE.
- **Transformador reductor** → tensión de rectificación ≈ 3,3 kV (para compensar
  caídas internas del rectificador).
- **Rectificador de silicio** de onda completa (6 o 12 pulsos) → CC.
- **Barra de CC a 3,3 kV**, filtros de armónicos, protección.
- **Dispositivo de protección de línea (DPL)**: disyuntor + seccionador de salida.
- Normalmente **dos grupos** (rectificador + transformador) por SET: uno en
  reserva o ambos en servicio según carga.
- Reversibilidad: en frenado, la energía puede volver por la barra (o disiparse
  en resistencias).

### 4.2 En CA (25 kV)

- Entrada de alta tensión de la red de transporte.
- **Autotransformadores o transformadores de tracción** con regulación
  (tap ± varios %) para mantener 25/27,5 kV en catenaria.
- Configuraciones **1x25 kV** (transformador simple, retorno por carril con
  transformadores de separación) y **2x25 kV** (autotransformador: catenaria a
  +25 kV y feeder a -25 kV, retorno a tierra).
- DPL de salida (disyuntor + seccionador) y seccionadores de telecomando.

---

## 5. LA LÍNEA DE CONTACTO (CATENARIA)

### 5.1 Componentes mecánicos

| Componente | Función |
|-----------|---------|
| **Poste / estructura** | soporta el conjunto (metálicos, presilleta, ménsula, brazos) |
| **Ménsula / brazos** | sostienen el hilo sustentador y el hilo de contacto |
| **Hilo sustentador (mensajero)** | cable de acero o acero-cobre que soporta el peso |
| **Pendolones** | hilos verticales que cuelgan el hilo de contacto del sustentador |
| **Hilo de contacto** | conductor ranurado (p. ej. 107 mm² Cu) por el que contacta el pantógrafo |
| **Anclajes / tensores** | fijan y tensan el cableado (contrapesos en las terminaciones) |
| **Grifas** | uniones entre hilos (grapas de cuña y de compresión) |
| **Aisladores** | separan eléctricamente las partes en tensión (vidrio/porcelana/polímero) |

### 5.2 Configuraciones en función de la velocidad

| Tipo | Velocidad | Descripción |
|------|-----------|-------------|
| **CA-160 / CA-220** | 160 / 220–250 km/h | compuesta: mensajero + hilo de contacto, poligonal |
| **CA-160H / CA-200H** | 160 / 200 km/h | variantes en hilo (H) con pórticos o mensajeros reforzados |
| **Simple (3 kV)** | ≤ 160 km/h | catenaria compuesta tradicional de la red convencional |
| **Y (compuesta)** | ≤ 200 km/h | tres hilos: mensajero, sustentador auxiliar y contacto |

### 5.3 Tensado

- **Tensado automático (T.A.)**: contrapesos (anclajes de tensión) mantienen
  constante la tensión del hilo con la temperatura → para velocidades > 120 km/h
  y en la mayor parte de la red.
- **Tensado semiautomático / fijo**: tensores de muelle o fijos, en vías
  apartadas o de baja velocidad.

---

## 6. ALIMENTACIÓN Y RETORNO

### 6.1 El feeder

- **Feeder (alimentador):** conductores que unen la SET con los puntos de
  alimentación del cantón y con las instalaciones de ayuda.
- En 2x25 kV el feeder es **negativo** (-25 kV) y cuelga del mismo poste.
- Los feeders se cablean por el poste en tensión y se seccionan con
  seccionadores de línea.

### 6.2 El retorno

- **CC:** los carriles hacen de retorno; se añaden **hilos de retorno (tierra)**
  en paralelo para reducir la caída y el potencial de tierra. La conexión
  carril-tierra se hace en las SET.
- **CA:** el retorno es el carril, pero para no interferir con la señalización
  se instalan **transformadores de separación** que obligan a la corriente de
  retorno a volver por el carril próximo al poste, y las corrientes homopolares
  se drenan con los **dispositivos de puesta a tierra**.

---

## 7. SECCIONAMIENTO Y PROTECCIÓN

- **Seccionamiento longitudinal:** separa tramos de catenaria entre subestaciones
  (elementos de seccionamiento, seccionadores de poste) para explotación en
  tensión o para aislar averías.
- **Seccionamiento transversal:** separa vías en estaciones (embarques,
  apartaderos) y permite trabajos en una vía mientras la otra sigue electrificada.
- **DPL:** disyuntor de línea que corta sobreintensidades; se telecontrola desde
  el telemando.
- **Seccionadores de puesta a tierra:** para trabajos, garantizan ausencia de
  tensión y descarga del tramo.

---

## 8. LÍMITES ELÉCTRICOS DE PROYECTO (RESUMEN)

| Magnitud | 3 kV CC | 25 kV CA |
|----------|---------|----------|
| Tensión de proyecto en catenaria | 3.000 V (2.000–3.600 V) | 25.000 V (17.500–27.500 V) |
| Tensión en SET | 3.300 V | 27.500 V |
| Distancia típica entre SET | 12–20 km | 60–100 km |
| Corriente de régimen (aprox.) | 2.000–4.000 A | 400–1.000 A |
| Línea de fuga mínima (zona normal) | 300 mm | 240 mm (a < 1.000 m) |
| Sección hilo de contacto típica | 107 mm² (Cu) | 107–150 mm² (Cu/Ag) |

---

## 9. AUTOEVALUACIÓN

1. ¿Qué dos sistemas coexisten en España y en qué tipo de red se aplica cada uno?
2. ¿Para qué sirve el transformador de 3,3 kV en la SET de CC?
3. Dibuja (en un esquema mental) el camino de la corriente desde REE al motor.
4. Diferencia entre 1x25 kV y 2x25 kV.
5. ¿Qué es el feeder en CC y qué función tiene el feeder en 2x25 kV?
6. ¿Por qué en CA hacen falta transformadores de separación en el retorno?
7. Nombra 6 componentes de la línea de contacto y su función.
8. ¿Qué diferencia hay entre tensado automático y tensado fijo?
9. ¿Qué es el DPL y qué protege?
10. ¿Qué línea de fuga mínima se exige en 3 kV y por qué?

---

## 10. REFERENCIAS

- NAE 300 Parte 1 (CA-160/3 kV) y NAE 301 Parte 1 (CA-220/3 kV).
- NAE 302 (CA-160H / CA-200H) — alta velocidad.
- ET 03.359.104.1 (rectificadores), ET 03.359.501.x (subestaciones CA).
- UNE-EN 50163, UNE-EN 50119.

---

*Siguiente módulo: Módulo 2 · Normativa ADIF: las NAE de montaje y diseño.*
