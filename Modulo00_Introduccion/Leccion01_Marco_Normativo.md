# MÓDULO 0 · LECCIÓN 1
# MARCO NORMATIVO DE LA ELECTRIFICACIÓN FERROVIARIA

## De la directiva europea al tornillo de la catenaria

---

## 1. RESULTADO DE APRENDIZAJE

Al terminar esta lección serás capaz de:

1. Explicar la **jerarquía normativa** europea y española que rige la
   electrificación ferroviaria
2. Identificar a los **actores** (ERA, Ministerio, ADIF, ADIF AV, CNMC, industria)
   y qué hace cada uno
3. Clasificar los **documentos normativos ADIF de energía** en sus 4 bloques y
   saber cuándo usar cada uno
4. Justificar una decisión de diseño con la **cadena normativa** completa
   (Directiva → ETI → Orden ministerial → NAE/ET)
5. Localizar el documento adecuado para un problema concreto del diseño

---

## 2. RESUMEN EJECUTIVO

No existe «una norma» de catenaria: existe una **pirámide normativa** que va desde
la Directiva europea de interoperabilidad hasta la especificación del material
concreto (p. ej. el aislador RT51). Cuando diseñas una línea de contacto:

- La **UE** fija los requisitos de interoperabilidad (tensión, gálibo, calidad).
- El **Ministerio** (hoy Ministerio de Transportes, antes Fomento/MITMA) aprueba
  las instrucciones ferroviarias de obligado cumplimiento (gálibos, energía,
  infraestructura) vía **BOE**.
- **ADIF** y **ADIF AV** desarrollan las normas de diseño (NAE 300/301/302), de
  montaje (NAE 100-199) y las especificaciones técnicas de materiales (ET).
- La **ETI de Energía (TSI ENE)** convierte la Directiva en requisitos técnicos
  concretos y verificables para la interoperabilidad.

La clave del curso: **toda decisión de diseño se justifica citando su documento
normativo**, y la pirámide te dice qué documento predomina si hay conflicto
(europeo > estatal > ADIF).

---

## 3. LA PIRÁMIDE NORMATIVA

```
            ┌─────────────────────────────┐
            │   DIRECTIVAS DE LA UE        │  Directiva (UE) 2016/797
            │   (interoperabilidad)        │  Directiva (UE) 2016/798 (seguridad)
            ├─────────────────────────────┤
            │   REGLAMENTOS / DECISIONES   │  Reglamentos ERA, Decisiones de la Comisión
            ├─────────────────────────────┤
            │   ETI / TSI                  │  TSI ENE (Energía), TSI INF, TSI OPE...
            ├─────────────────────────────┤
            │   ESTADO: ÓRDENES MINISTERIO │  FOM/1630/2015 (gálibos)
            │   (BOE)                      │  TMA/135/2023 (IFI + IFE)
            │                              │  TMA/698/2023 (REVINFE-23)
            ├─────────────────────────────┤
            │   GESTOR: ADIF / ADIF AV     │  NAE (normas), ET (especificaciones)
            │                              │  Instrucciones internas, Libros de LAC
            ├─────────────────────────────┤
            │   ESTÁNDARES TÉCNICOS        │  UNE, UNE-EN, EN, IEC, ISO
            └─────────────────────────────┘
```

**Regla de prevalencia:** en caso de conflicto manda el nivel superior; la
normativa ADIF **no puede** contradecir una ETI, y una ET no puede contradecir su
NAE de aplicación.

---

## 4. ACTORES Y SUS FUNCIONES

| Actor | Qué hace | Relevancia para el diseño |
|-------|----------|---------------------------|
| **ERA** (Agencia Ferroviaria de la UE) | Prepara y revisa las TSI; emite autorizaciones de vehículos | Decide los valores normativos de la TSI ENE |
| **Comisión Europea** | Adopta formalmente las TSI | Publica la versión vigente (rango «UE/...») |
| **Ministerio de Transportes** (España) | Aprueba instrucciones ferroviarias (BOE) y autoriza la puesta en servicio | IFI, IFE, gálibos, REVINFE: obligatorios en España |
| **CNMC** | Supervisa la competencia; regula cánones de acceso | No diseña, pero condiciona la explotación |
| **ADIF / ADIF AV** | Gestor de infraestructura; mantiene y desarrolla la red | Autor de las NAE y ET; dueño de las instalaciones |
| **Agencia Estatal de Seguridad Ferroviaria (AESF)** | Vigila la seguridad | Verifica la aplicación de las normas |
| **Industria / contratistas** | Diseña y construye siguiendo la normativa ADIF | Ejecuta lo que exige cada NAE/ET |

---

## 5. LOS DOCUMENTOS ADIF DE ENERGÍA (4 BLOQUES + BOE)

Todo el material normativo del curso se organiza así:

| Bloque | Referencia | Contenido | Ejemplo |
|--------|-----------|-----------|---------|
| **A · Normas NAE** | `NAE xxx` | Diseño funcional y montaje de la línea aérea | NAE 300 (CA-160), NAE 108 (tendido) |
| **B · ET LAC** | `ET 03.364.xxx` | Materiales y componentes de la catenaria | ET 03.364.291.9 (hilo ranurado) |
| **C · ET SSEE** | `ET 03.359.xxx` | Subestaciones de tracción (CC y CA) | ET 03.359.104.1 (rectificador 3,3 kV) |
| **D · ET Telemandos** | `ET 03.359.120.x / 501.x` | Control remoto y telegestión | ET 03.359.501.8 (protocolo 25 kV) |
| **E · BOE** | Órdenes ministeriales | Gálibos, IFI, IFE, REVINFE | FOM/1630/2015, TMA/135/2023 |

### Dentro de las NAE hay dos familias:

- **NAE 100-199 · Montaje y ejecución** (100 = campo general): NAE 101 (grifas),
  106 (cimentaciones), 107 (parámetros), 108 (tendido), 110 (feeder), 111
  (tierra/retorno), 115 (agujas), 116 (pendolado), 121 (avifauna)…
- **NAE 300-399 · Diseño funcional**: NAE 300 (CA-160/3 kV), NAE 301 (CA-220/3 kV),
  NAE 302 (CA-160H/CA-200H).

### Especificaciones Técnicas (ET) por familias:

- **ET 03.364.0xx** → piezas y herrajes (grifas, tensores, aisladores, poleas)
- **ET 03.364.1xx** → estructuras (postes, ménsulas, brazos) y conductores
- **ET 03.364.2xx** → grapas de anclaje, aisladores compuestos, verificadores
- **ET 03.359.1xx** → subestaciones de CC (3,3 kV y 1,5 kV)
- **ET 03.359.5xx** → subestaciones de CA (1x25 kV y 2x25 kV)

---

## 6. CÓMO SE JUSTIFICA UNA DECISIÓN (EJEMPLO REAL)

**Pregunta de diseño:** ¿qué aislador uso para suspender el hilo de contacto en la
CA-220/3 kV, y con qué línea de fuga?

Cadena de justificación:

```
1. Directiva (UE) 2016/797        → exige interoperabilidad y seguridad
2. TSI ENE (Decisión UE 2023/1697) → parámetro "sección de línea de contacto",
                                     tensiones EN 50163, gálibo del pantógrafo
3. IFE (Orden TMA/135/2023)       → reglas estatales de energía y mantenimiento
4. NAE 301 Parte 1 (CA-220)       → fuga ≥ 300 mm (3 kV), aislador de línea
5. ET 03.364.164.8 / 202.6        → material concreto: vidrio A11/RT51 o compuesto
6. UNE-EN 50149 / 50119           → fabricación y coef. de seguridad
```

Cada nivel responde a una pregunta distinta: **el EUROPEo dice qué requisito
interoperable debe cumplirse, el ESTADO cómo se aplica en España, el ADIF con qué
solución, y la ET con qué pieza exacta.**

---

## 7. CÓMO LOCALIZAR EL DOCUMENTO CORRECTO

1. **Define el problema** → ¿es de gálibo?, ¿de tensión?, ¿de montaje?, ¿de material?
2. **BOE primero** → si existe instrucción ministerial aplicable (gálibos, IFE),
   esa manda.
3. **NAE de diseño** → NAE 300/301/302 dan el parámetro de proyecto.
4. **NAE de montaje** → NAE 100-199 explican cómo se instala.
5. **ET de material** → la pieza concreta que cumple la NAE.
6. **Norma UNE/EN/IEC** → ensayos y métodos (citadas por las propias ET).

El **Registro_Documentos.md** del curso cataloga los 106 documentos con su
referencia, título, edición y estado de integración en las lecciones.

---

## 8. PREGUNTAS DE AUTOEVALUACIÓN

1. ¿Qué manda si una NAE contradice a la TSI ENE?
2. ¿Quién aprueba las ETI en la UE?
3. Diferencia entre ADIF y ADIF AV.
4. ¿Qué bloques de documentos ADIF de energía existen y qué cubre cada uno?
5. ¿En qué rango de números están las NAE de montaje y las de diseño?
6. ¿Qué es la IFE y quién la aprueba?
7. ¿Qué papel juega la AESF?
8. Da la cadena normativa completa para justificar la línea de fuga de un aislador
   de 3 kV.
9. ¿Qué norma europea fija las tensiones de contacto del sistema (EN)?
10. ¿Qué documento del curso cataloga los 106 documentos normativos?

---

## 9. REFERENCIAS

- Directiva (UE) 2016/797 (interoperabilidad) y 2016/798 (seguridad)
- TSI ENE (Reglamento (UE) 2023/1697) — Decisión de la Comisión
- Orden FOM/1630/2015 (gálibos), Orden TMA/135/2023 (IFI/IFE), Orden TMA/698/2023
  (REVINFE-23)
- NAE 300/301/302 (diseño), NAE 100-199 (montaje), ET 03.364/03.359 (materiales)
- `Registro_Documentos.md` del curso

---

*Siguiente lección: Módulo 1 · Fundamentos de la electricidad de tracción.*
