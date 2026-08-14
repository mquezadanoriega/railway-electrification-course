# VOLUMEN VIII: Curso de Electrificación Ferroviaria

## De la normativa a la práctica

---

> *"En electrificación ferroviaria no se diseña lo que se quiere: se diseña lo que la normativa permite."*

---

## TU OBJETIVO

Convertirte en la ingeniera de referencia en **sistemas de tracción eléctrica ferroviaria**, capaz de:

- **Diseñar la electrificación de una vía ferroviaria** de principio a fin
- Elegir el sistema correcto (25 kV CA / 3 kV CC / etc.) según la línea
- Seleccionar y dimensionar catenaria, subestaciones, protecciones y telemando
- Justificar cada decisión de diseño con la **normativa ADIF** correspondiente
- Aplicar los **gálibos** (especialmente el **gálibo de pantógrafo**) en el trazado
- Verificar el cumplimiento de las **ETI de Energía** (TSI ENE)

> **Método:** curso basado en **proyectos reales de electrificación**. Se diseña
> una vía completa y cada decisión se justifica citando la norma que la respalda.

---

## CÓMO SE DISEÑA UN PROYECTO DE ELECTRIFICACIÓN (FLUJO DE TRABAJO)

El curso sigue el proceso real de diseño de un proyecto de electrificación:

```
1. DATOS DE PARTIDA          ←  Trazado, gálibos, velocidad, tráfico, catenaria existente
        │
2. ELECCIÓN DEL SISTEMA      ←  25 kV CA (AV) vs 3 kV CC (convencional) vs 2x25 kV
        │
3. DISEÑO DE LA CATENARIA    ←  Selección del tipo: NAE 300 (CA-160), NAE 301 (CA-220),
        │                        NAE 302 (CA-160H/CA-200H) → postes, péndolas, tensado
        │
4. DISEÑO DE SUBESTACIONES   ←  Potencia, transformadores, rectificadores, protecciones,
        │                        cabinas (ET 03.359.xxx)
        │
5. RETORNO Y PROTECCIONES    ←  Cable de tierra/retorno, seccionamiento, puesta a tierra
        │
6. TELEMANDO Y CONTROL       ←  Control remoto, protocolos (ET Telemandos)
        │
7. VERIFICACIÓN ETI ENE      ←  Interoperabilidad: tensión, gálibo de pantógrafo, calidad
        │                        de la energía
        │
8. DOCUMENTACIÓN DEL PROYECTO←  Memoria, planos, pliegos, mediciones
```

Cada etapa se resuelve con un **caso práctico** y se justifica con la normativa correspondiente.

---

## CÓMO SE CONSTRUYE ESTE CURSO

Este curso se construye **de abajo hacia arriba**, a partir de los documentos normativos reales:

| Fase | Fuente | Qué se integra |
|------|--------|----------------|
| **Fase 1** | Normativa ADIF (la aporta la alumna) | Documentos base, ETI aplicables, especificaciones particulares |
| **Fase 2** | Normativa de gálibos | Gálibo de catenaria, gálibo de pantógrafo, gálibos de infraestructura |
| **Fase 3** | ETI de Energía | TSI ENE, interfaces con otras ETI, interoperabilidad |

Cada documento se procesa así:

1. **Lectura** → se vuelca el contenido esencial
2. **Resumen ejecutivo** → qué dice y por qué importa
3. **Tabla de datos clave** → valores, parámetros, rangos
4. **Preguntas de autoevaluación** → para verificar que se ha entendido
5. **Mapa mental / diagrama** → cómo se relaciona con el resto

---

## ESTRUCTURA DEL CURSO

```
Volume8_RailwayElectrification/
│
├── README.md                    ← Estás aquí (índice del curso)
│
├── Modulo00_Introduccion/       ← Marco general, estructura de la normativa
├── Modulo01_Fundamentos/        ← Electricidad de tracción, AC vs DC, sistemas
├── Modulo02_Normativa_ADIF/     ← NAE 101/102/103/106/110/111/113/114/201 + ET materiales
├── Modulo03_Galibos/            ← Gálibos: catenaria, pantógrafo, infraestructura
├── Modulo04_ETI_Energia/        ← ETI de Energía / TSI ENE / IFE
├── Modulo05_Sistemas_Traccion/  ← Subestaciones, catenaria, retorno de corriente
└── Modulo06_Casos_Practicos/    ← Aplicación a proyectos reales
```

---

## CONTENIDO POR MÓDULO

### Módulo 0: Introducción (marco normativo)
- Estructura de la normativa española y europea
- Jerarquía: Directivas EU → ETI/TSI → Normativa ADIF → Especificaciones particulares
- Actores: ERA, Ministerio, ADIF, ADIF-AV, CNMC
- Cómo buscar y localizar documentos normativos

### Módulo 1: Fundamentos de la electrificación
- Por qué electrificar: energía, emisiones, capacidad
- Sistemas de tracción: CA 25 kV 50 Hz, CA 15 kV 16,7 Hz, CC 3 kV, CC 1,5 kV, CC 750 V
- La red española: 3 kV CC (red convencional) y 25 kV CA (alta velocidad)
- Componentes del sistema: subestaciones, catenaria, retorno, vehículos

### Módulo 2: Normativa ADIF (NAE + ET de materiales)
- Montaje, grifas y herrajes de la catenaria — NAE 101, NAE 102, NAE 201
- Cimentaciones y anclajes de postes — NAE 103, NAE 106, NAE 113
- Feeder, cable de tierra y retorno — NAE 110, NAE 111, NAE 114
- Materiales de LAC y herrajes — ET 03.364.xxx

### Módulo 3: Gálibos *(Fase 2)*
- Concepto de gálibo y tipos
- **Gálibo de pantógrafo** (el más importante)
- Gálibo de catenaria y de línea de contacto
- Gálibos de infraestructura (GHE, UIC, etc.)
- Interacciones: vía → catenaria → pantógrafo → vehículo

### Módulo 4: ETI de Energía
- Directiva 2016/797 de interoperabilidad
- TSI ENE: Especificación Técnica de Interoperabilidad de Energía (UE 2023/1697)
- IFE: Instrucción Ferroviaria de Energía (TMA/135/2023)
- Parámetros: tensión y frecuencia, secciones de línea de contacto, pantógrafos
- Interfaces con otras TSI (infraestructura, material rodante)

### Módulo 5: Sistemas de tracción
- Subestaciones eléctricas de tracción (SET)
- Seccionamiento y postes de seccionamiento
- Catenaria: tipos y composición
- Circuito de retorno y protección (telegestión, protecciones)

**Lecciones del módulo 5 (completas):**

| Lección | Contenido | Norma |
|---------|-----------|-------|
| Lección 1 | Parámetros de la LAC | NAE 107 |
| Lección 2 | Diseño funcional CA-160 / CA-220 / CA-160H-200H | NAE 300 / 301 / 302 |
| Lección 3 | Montaje y tensado del sustentador e hilo · Pendolado | NAE 108 · NAE 116 |
| Lección 4 | Agujas aéreas (P-50 cruzada · P-90 tangencial) | NAE 115 |
| Lección 5 | Esquemas eléctricos de LAC en CC | NAE 112 |
| Lección 6 | Esquemas eléctricos de LAC en 25 kV CA (1x25 / 2x25) | NAE 119 |
| Lección 7 | LAC en vías de tres carriles | NAE 117 |
| Lección 8 | Protección de la avifauna | NAE 121 |
| Lección 9 | Centros de transformación aéreos | NAE 400 |
| Lección 10 | Conductores de LAC | ET 03.364 |
| Lección 11 | Aisladores y aislamiento | ET 03.364 |
| Lección 12 | Soportes, estructuras y seccionadores | ET 03.364 |
| Lección 13 | Subestaciones de CC (3,3 kV / 1,5 kV) | ET 03.359 |
| Lección 14 | Subestaciones de 25 kV CA (1x25 / 2x25) | ET 03.359 |
| Lección 15 | Telemando de energía (IEC 60870-5-101/104) | ET 03.359 |

### Módulo 6: Casos prácticos
- Lección 1: Casos resueltos
  - Cálculo de gálibo de pantógrafo
  - Dimensionado de un cantón de 3 kV CC por caída de tensión
  - Verificación de la TSI ENE / IFE
  - Selección de catenaria y aisladores para 25 kV
  - Cadena normativa completa de cada decisión de diseño
- Lección 2: Caso completo de diseño de catenaria desde un trazado
  - Alturas del hilo, gálibo del pantógrafo y desviación lateral (apéndice E IFE)
  - Vanos, descentramientos y cantón de compensación por radio
  - Selección de postes y macizos de catálogo (MLS)
  - Detección de los casos que requieren **cálculo específico** (poste, macizo, pendolado)

---

## REGISTRO DE DOCUMENTOS NORMATIVOS

Todos los documentos de la normativa ADIF de Energía están catalogados en:

📄 **`Registro_Documentos.md`** (106 documentos)

Organizados en 5 bloques:

| Bloque | Contenido | Documentos |
|--------|-----------|-----------|
| A | Normas **NAE** — Línea Aérea de Contacto | 29 |
| B | **ET 03.364.xxx** — Materiales de LAC | 40 |
| C | **ET 03.359.1xx / 5xx** — Subestaciones (CC y CA) | 30 |
| D | **ET Telemandos** — Control y telegestión | 3 |
| E | **Normativa BOE** — Gálibos, IFI, IFE | 4 |

El procesamiento de cada documento sigue este flujo:

1. **Lectura** → se vuelca el contenido esencial
2. **Resumen ejecutivo** → qué dice y por qué importa
3. **Tabla de datos clave** → valores, parámetros, rangos
4. **Preguntas de autoevaluación** → para verificar que se ha entendido
5. **Mapa mental / diagrama** → cómo se relaciona con el resto

> **Estado actual:** documentación extraída, catalogada e integrada en los 7 módulos
> del curso (ver Dashboard).

---

## CÓMO SE USA

1. **Cada semana**, se procesa un documento normativo
2. Se actualiza el **Registro de documentos** al integrarlo
3. Se responden las **preguntas de autoevaluación** de cada módulo
4. Los **casos prácticos** se resuelven con los datos reales de las normas

---

## DASHBOARD DE SEGUIMIENTO

| Indicador | Objetivo | Estado |
|-----------|----------|--------|
| Documentos ADIF catalogados | 106 | ✔ (11/08/2026) |
| Documentos ADIF integrados en los módulos | 106 | ✔ (26/26 lecciones) |
| Lecciones del Módulo 2 (NAE + ET materiales) | 4 | ✔ |
| Gálibos dominados (pantógrafo, catenaria, instalaciones) | 4 | ✔ (2/2 lecciones) |
| Parámetros de la LAC dominados (NAE 107) | 1 | ✔ |
| Diseño funcional de catenarias (NAE 300/301/302) | 1 | ✔ |
| Montaje, tensado y pendolado (NAE 108/116) | 1 | ✔ |
| Esquemas eléctricos CC y CA (NAE 112/119) | 2 | ✔ |
| LAC de tres carriles (NAE 117) y avifauna (NAE 121) | 2 | ✔ |
| Conductores, aisladores, soportes (ET 03.364) | 3 | ✔ |
| Subestaciones CC y CA (ET 03.359) | 2 | ✔ |
| Telemando de energía (ET 03.359) | 1 | ✔ |
| ETI de Energía integradas (TSI ENE / IFE) | 1 | ✔ |
| Casos prácticos resueltos | 5 | ✔ (Módulo 6) |

---

*Curso construido a partir de la normativa real aportada por la alumna.*
