# MÓDULO 1 · LECCIÓN 1
# FUNDAMENTOS DE LA ELECTRICIDAD DE TRACCIÓN

## De la ley de Ohm al cálculo del cantón de alimentación

---

## 1. RESULTADO DE APRENDIZAJE

Al terminar esta lección serás capaz de:

1. Explicar por qué se electrifica una línea y qué ventajas aporta frente a la
   tracción diésel
2. Conocer las **tensiones normalizadas de contacto** según UNE-EN 50163 y su
   distribución geográfica mundial
3. Comparar **corriente continua (CC) y corriente alterna (CA)** en tracción:
   ventajas, inconvenientes y campos de aplicación
4. Calcular la **caída de tensión** de un cantón de alimentación
5. Entender los conceptos de **cantón de alimentación**, seccionamiento y
   dispositivo de protección de línea

---

## 2. RESUMEN EJECUTIVO

La electricidad se ha impuesto en el ferrocarril porque permite **potencias
específicas muy altas** con bajo consumo y **cero emisiones en origen** si la
energía es renovable. Existen cuatro familias de tensión normalizada por la
norma EN 50163:

- **CC**: 750 V y 1,5 kV (metros, tranvías, cercanías) y **3 kV** (convencional).
- **CA**: **15 kV / 16,7 Hz** (centroeuropa) y **25 kV / 50 Hz** (alta velocidad,
  y casi todo lo moderno).

España usa **3 kV CC en la red convencional** (la más extendida en superficie) y
**25 kV CA en la red de alta velocidad** (AVE, LAV). El 3 kV es una reliquia bien
conservada que sigue siendo eficiente para líneas de media exigencia; el 25 kV es
el estándar interoperable de la TSI ENE.

---

## 3. EL SISTEMA DE TRACCIÓN ELÉCTRICO

### 3.1 ¿Por qué electrificar?

| Ventaja | Detalle |
|---------|---------|
| **Potencia específica** | un tren eléctrico puede tirar de más tonelaje y acelerar antes |
| **Eficiencia** | rendimiento global muy superior al diésel |
| **Emisiones** | nulas en túnel y ciudad; descarbonización si origen renovable |
| **Fiabilidad** | menos mantenimiento mecánico que un motor térmico |
| **Freno regenerativo** | recupera energía (en CC puede devolverse a red o a acumuladores) |

### 3.2 Magnitudes básicas que debes manejar

```
P = V · I          potencia (W)
V = I · R          ley de Ohm (V)
P = I² · R         pérdidas Joule (W)
U_caída = I · R_L  caída de tensión en línea (V)
R_L = ρ · L / S    resistencia del conductor (Ω)
```

Donde ρ es la resistividad del conductor (cobre: 0,01724 Ω·mm²/m a 20 °C),
L la longitud y S la sección.

---

## 4. TENSIONES NORMALIZADAS (UNE-EN 50163)

| Sistema | Tensión nominal | Rango continuo | Uso típico |
|---------|----------------|----------------|------------|
| **CC 750 V** | 750 V | 600–780 V | Metro, tranvía, tercer carril (red alimentación) |
| **CC 1,5 kV** | 1,5 kV | 1–1,8 kV | Zona norte de España (feeder), metros europeos |
| **CC 3 kV** | 3 kV | 2–3,6 kV | Red convencional española y parte de la europea |
| **CA 15 kV** | 15 kV | 11–18 kV | Alemania, Austria, Suiza, Suecia (16,7 Hz) |
| **CA 25 kV** | 25 kV | 17,5–27,5 kV | LAV España, Francia, alta velocidad mundial (50 Hz) |

**Nota operativa:** el rango continuo (2–3,6 kV en 3 kV CC) es clave: si el
pantógrafo ve menos de 2 kV en punta de rampa y bajo punta de tracción, hay que
reforzar el cantón (más alimentación o sección de feeder).

---

## 5. CORRIENTE CONTINUA FRENTE A CORRIENTE ALTERNA

### 5.1 CC (3 kV)

**Ventajas**
- No hay problemas de impedancia inductiva (los trayectos de retorno son más
  simples).
- Freno regenerativo natural (reversibilidad).
- Baja emisión de interferencias en vía (contactos, señalización).

**Inconvenientes**
- Tensiones limitadas (aislamiento y conmutadores): para subir de tensión hay que
  poner dos subestaciones en serie o usar secciones dobles.
- Corrientes altas → secciones de hilo grandes y pérdidas mayores a igual potencia.
- Convertidores y rectificadores voluminosos.

### 5.2 CA (25 kV / 50 Hz)

**Ventajas**
- Tensión alta → **corriente menor** → sección de catenaria menor y subestaciones
  mucho más separadas (60–100 km frente a 15–30 km en CC).
- Transformadores sencillos y baratos (25 kV nace directamente de la red
  eléctrica de 220/400 kV).
- Interoperable: es la tensión que exige la TSI ENE.

**Inconvenientes**
- **Reactancia inductiva** de la línea (la impedancia ya no es solo R).
- Retorno por carril complicado (las corrientes parásitas interfieren con la
  señalización de vía) → hay que blindar con transformadores de separación o
  retornos especiales.
- Fenómenos de resonancia y armónicos a 50 Hz y múltiplos.
- Interferencias electromagnéticas sobre circuitos de vía.

### 5.3 Cómo se elige

```
Potencia demandada alta + línea nueva + AV        → 25 kV CA
Línea convencional existente con 3 kV en la zona   → 3 kV CC (cambio es carísimo)
Metro / tranvía                                    → 750 V o 1,5 kV CC
Red de montaña centroeuropea                       → 15 kV 16,7 Hz
```

---

## 6. EL CANTÓN DE ALIMENTACIÓN Y SU CÁLCULO

### 6.1 Definiciones

- **Cantón de alimentación (sección de alimentación):** tramo de catenaria
  alimentado desde una misma subestación y sin posibilidad de conmutación interna.
- **Subestación de tracción (SET):** punto de inyección de energía; en CC suele
  tener **rectificador 3,3 kV**, en CA **transformador 25 kV**.
- **Dispositivo de protección de línea (DPL):** aparamenta (disyuntor, seccionador)
  que protege el cantón frente a sobreintensidades.
- **Seccionamiento:** división del cantón en tramos conmutables para explotación,
  mantenimiento o averías (postes con seccionadores aéreos).

### 6.2 Caída de tensión en un cantón de CC

En CC la caída depende solo de la **resistencia** del hilo + carril de retorno:

```
ΔU = I · (R_hilo + R_carril) · L
```

Con 3 kV y un límite del 20 % (600 V máx. de caída con margen de contacto):

- Un tren que demanda 4000 A a 15 km de la SET: ΔU = 4000 · 0,02 Ω/km · 15 =
  **1200 V → inviable** (por debajo del mínimo de 2 kV).
- Soluciones: reducir distancia a SET, aumentar sección del feeder, doble vía
  (cada vía con su propio retorno), o elevar tensión.

En **CA** se añade la **reactancia**:

```
ΔU ≈ I · (R·cosφ + X·sinφ) · L
```

La reactancia domina a 50 Hz (X ≈ 0,35 Ω/km en catenaria CA-160). Por eso en
25 kV las SET se separan mucho: la corriente es ~10 veces menor.

### 6.3 Ejemplo resuelto (CC 3 kV)

Un cantón de 12 km con hilo de contacto Cobre 107 mm² + hilo de contacto auxiliar
en feeder (sección equivalente 200 mm²). Resistencia total bucle ≈ 0,18 Ω/km.
Tren en punta de rampa demandando 3200 A a 10 km.

```
ΔU = 3200 A · 0,18 Ω/km · 10 km = 5760 V  → imposible
```

Conclusión: un cantón de CC no puede alimentar esa corriente a esa distancia;
la SET debe estar a < 3 km o el tren se alimenta de **doble vía** (dos alimentadores
paralelos dividen la corriente). Por eso las SET de CC españolas están a
**12–20 km** y las de 25 kV a **60–100 km**.

---

## 7. AUTOEVALUACIÓN

1. Nombra las cuatro tensiones normalizadas de EN 50163 y sus rangos.
2. ¿Por qué el 25 kV permite subestaciones más separadas que el 3 kV?
3. ¿Qué dos problemas nuevos introduce la CA frente a la CC en la catenaria?
4. Calcula la caída de tensión de un tren de 2400 A a 8 km de la SET con
   resistencia de bucle 0,2 Ω/km.
5. ¿Qué es el DPL y dónde se coloca?
6. ¿Por qué la EN 50163 limita la tensión mínima de contacto del 3 kV a 2 kV?
7. ¿Qué corriente es mayor para la misma potencia: la de 3 kV o la de 25 kV?
8. ¿Qué papel juega el freno regenerativo en un sistema de CC?
9. ¿Qué norma fija los rangos de tensión y quién la cita (EN/UNE-EN)?
10. ¿Cuál es la tensión de la red de alta velocidad española?

---

## 8. REFERENCIAS

- UNE-EN 50163: Tensiones de alimentación de los sistemas de tracción.
- UNE-EN 50119: Aplicaciones ferroviarias — Instalaciones fijas — Líneas aéreas
  de contacto.
- NAE 301 Parte 1 (diseño de la CA-220/3 kV) — límites de tensión de proyecto.
- ET 03.359.104.1 (rectificador 3,3 kV) y ET 03.359.501 (subestaciones CA).

---

*Siguiente: Módulo 1 · Lección 2 · La red española y sus componentes.*
