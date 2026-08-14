# MÓDULO 5 · LECCIÓN 15
# EL TELEMANDO DE ENERGÍA: CONTROL REMOTO DE SUBESTACIONES Y SECCIONAMIENTOS (ET 03.359)

## Documento base

> **ET 03.359.120.7** (1ª edición, febrero 2007), partes 2/9 y 9/9:
> - Parte 2/9: *«Prescripciones técnicas y funcionales para el suministro y montaje de telemandos de energía (Líneas Convencionales). Puesto Central»*.
> - Parte 9/9: *«Protocolo de comunicaciones entre centro de control y remotas (líneas convencionales). Perfil de interoperabilidad ADIF IEC 60870-5-101»*.
>
> **ET 03.359.501.8** (1ª edición, abril 2008):
> - *«Protocolo de comunicaciones entre centro de control y remotas en telemandos de energía de líneas de alta velocidad. Perfil de interoperabilidad ADIF IEC 60870-5-104»*.

> Documentos de apoyo: NAE 112 (esquemas eléctricos en CC), NAE 119 (esquemas eléctricos en CA) y ET 03.359.1xx/5xx (telemandos de energía y líneas de alta velocidad).

---

## 1. RESULTADO DE APRENDIZAJE

Al finalizar la lección, el alumno será capaz de:

- Explicar qué es el telemando de energía, qué infraestructuras eléctricas gobierna y por qué constituye el sistema de explotación de la electrificación ferroviaria.
- Describir la arquitectura del sistema de telemando de energía de ADIF (remotas, ramales de comunicación, puesto central, intranet) y el papel de cada nivel.
- Identificar las cuatro funciones clásicas de todo sistema de telemando —telemando, telemedida, telesupervisión y telealarma— y aplicarlas al control de subestaciones y seccionamientos.
- Conocer las maniobras de explotación que se ejecutan desde el puesto central (rearme, desconexión de emergencia, autorización de toma de mando, cambio de modo de funcionamiento) y sus requisitos de confirmación.
- Distinguir los perfiles de interoperabilidad IEC 60870-5-101 (líneas convencionales) e IEC 60870-5-104 (alta velocidad) definidos por ADIF, y comprender los conceptos de ASDU, causa de transmisión, origen de aplicación y direccionamiento.
- Entender los requisitos de alta disponibilidad, redundancia y seguridad que deben cumplir el puesto central y las instalaciones remotas.
- Relacionar el telemando con las ET 03.359.1xx/5xx (subestaciones y telemandos de líneas de alta velocidad) y con los esquemas eléctricos definidos en las NAE 112 y NAE 119.

---

## 2. RESUMEN EJECUTIVO

El telemando de energía es el sistema de control remoto desde el cual ADIF supervisa y maniobra la infraestructura de alimentación eléctrica del ferrocarril: subestaciones, centros de autotransformación o de línea, seccionamientos y telemandos asociados. Sustituye la explotación presencial en cada instalación por un control centralizado ejercido desde un puesto central, situado en los centros de control y telemandos.

El conjunto documental ET 03.359.120.7 define el telemando de energía de las líneas convencionales, tanto en lo relativo al puesto central (parte 2/9) como al protocolo de comunicaciones con las remotas (parte 9/9, perfil de interoperabilidad ADIF IEC 60870-5-101). Para las líneas de alta velocidad, la ET 03.359.501.8 define el perfil ADIF IEC 60870-5-104, basado en comunicaciones TCP/IP a través de una red WAN de muy alta disponibilidad.

La arquitectura se organiza en niveles: las instalaciones remotas (donde residen los elementos de campo), los ramales de comunicación (concentradores y canales), el puesto central y la intranet de ADIF, que integra la información con otras áreas. Desde el puesto central se realizan telemandos (apertura y cierre de seccionadores, conexión y desconexión de disyuntores), telemedidas, telesupervisión y telealarmas, además de maniobras de explotación como el rearme y la desconexión de emergencia.

El cumplimiento de la normativa es esencial: las prescripciones técnicas fijan disponibilidades muy exigentes (funciones de alta disponibilidad superiores al 99,98 % mensual y disponibilidad media anual superior al 99,5 %), capacidad de procesamiento sobredimensionada, tratamiento inequívoco de mando local frente a telemando y protocolos de interoperabilidad que garantizan que centros de control y remotas de distintos suministradores puedan intercambiar órdenes y señales de forma normalizada.

---

## 3. QUÉ ES EL TELEMANDO DE ENERGÍA Y PARA QUÉ SIRVE

### 3.1. Definición y alcance

El telemando de energía es el sistema mediante el cual, desde un puesto central, se controlan a distancia los equipos de una o varias instalaciones eléctricas de la infraestructura ferroviaria. En el entorno de ADIF, el telemando de energía comprende los siguientes tipos de instalación:

- **Subestaciones (SS/EE)**: puntos de conexión a la red de transporte o distribución (generalmente a 132 kV o 220 kV en la documentación de referencia) donde se transforma la energía y se alimenta la línea de tracción.
- **Estaciones (Z/N)**: instalaciones que pueden o no contener subestación asociada y que incluyen seccionamientos y equipos de maniobra.
- **Centros de línea de señales (L/S)**: instalaciones de seccionamiento y de apoyo a la alimentación de la línea de señales.
- **Seccionamientos**: elementos de corte sin carga que permiten aislar tramos, separar circuitos o conectar barras y pórticos de seccionadores.

En la práctica operativa, el telemando de energía es el «lugar» desde el que se explota la red de alimentación: se vigila el estado de cada seccionador y disyuntor, se mide tensión e intensidad, se recibe cada alarma y se ejecuta cada maniobra solicitada por el mando de la circulación (MOA) o por los centros de control.

### 3.2. ¿Para qué sirve?

- **Centralizar la explotación**: un único puesto central supervisa y controla un gran número de subestaciones y seccionamientos repartidos a lo largo de la línea, evitando desplazamientos de personal a cada instalación para maniobras ordinarias.
- **Mejorar la seguridad**: permite la desconexión de emergencia de una subestación o tramo de forma rápida y coordinada ante incidencias en la infraestructura o en la circulación.
- **Acortar los tiempos de reposición**: el rearme telemando tras un disparo restablece el servicio sin esperar a la presencia física de personal, lo que reduce el impacto en la circulación de trenes.
- **Explotar con conocimiento del estado real**: la telesupervisión y la telemedida proporcionan al operador la información necesaria para decidir maniobras con criterio.
- **Registrar y auditar**: el registro de eventos y órdenes permite reconstruir la secuencia de maniobras ante incidencias, averías o reclamaciones.

### 3.3. Distinción entre telemando y otros sistemas

Conviene diferenciar el telemando de energía de otros sistemas próximos:

- El **CTC (control de tráfico centralizado)** gestiona la circulación de trenes; en la arquitectura de ADIF el CTC asociado se integra en la intranet, pero no forma parte del telemando de energía.
- La **gestión técnica (JTMI)** gestiona la energía contratada y el consumo; se relaciona con el telemando a través de la intranet.
- El **mando local** es la explotación de una instalación desde su propio armario o cuadro, sin intervención del puesto central; es la situación alternativa cuando el telemando no está disponible o se requiere intervención presencial.

---

## 4. ARQUITECTURA DEL SISTEMA (PUESTO DE MANDO, CENTRO DE CONTROL, RTU, CANAL)

### 4.1. Niveles de la arquitectura ADIF

La ET 03.359.120.7 parte 2/9 describe una arquitectura en cinco niveles. A efectos del telemando de energía, solo **tres niveles forman parte del propio telemando**; los otros dos son sistemas corporativos que se integran con él:

1. **Remotas**: conjunto de equipos instalados en cada subestación, estación o centro de línea. Incluyen la unidad terminal remota (RTU), los autómatas asociados, las señales de campo (estados de seccionadores, disyuntores, rearmadores, ruptofusibles) y los elementos de ejecución de órdenes.
2. **Ramales de comunicación**: los enlaces entre las remotas y el puesto central. Incluyen concentradores de remotas, gateways o pasarelas y los canales físicos (red de fibra o cables), suministrados en el entorno ADIF por **Telecomunicaciones de ADIF**.
3. **Puesto central**: el sistema que recibe la información de todas las remotas y desde el que el operador ejerce el control. Está situado en el centro de control y telemandos.

Por encima del puesto central se sitúan los dos niveles corporativos:

4. **Intranet de ADIF**: gestionada por **Servicios Informáticos de ADIF**. Integra la Base de Datos Central, la Gestión Técnica (JTMI) y el CTC asociado. La intranet no forma parte del telemando de energía propiamente dicho, pero consume y aporta información a través del puesto central.
5. **Nivel de gestión corporativa**: consumo de información y servicios por el resto de aplicaciones de ADIF (gestión de activos, mantenimiento, energía contratada, etc.).

En la arquitectura de los telemandos de líneas de alta velocidad (ET 03.359.501.8), los ramales de comunicación se apoyan sobre la **red WAN de muy alta disponibilidad** y en ella conviven, además de los centros de control, los **puestos locales externos** (hasta 254) conectados mediante routers.

### 4.2. El puesto central

El puesto central está formado por:

- **Puestos fijos de operación**: pantallas desde las que el operador visualiza el estado del sistema eléctrico y las alarmas, y desde las que envía órdenes.
- **Puestos volantes**: estaciones de operación adicionales para seguimiento o supervisión sin capacidad de mando, o con la que se les asigne.
- **Base de datos del sistema**: contiene el modelo de información (señales, equipos, direcciones, parámetros).
- **Registro histórico**: almacena eventos, alarmas y órdenes para consulta posterior.
- **Impresión**: salida de informes, listados de eventos y copias en papel de los mensajes relevantes.
- **Panel sinóptico**: representación sintética del esquema eléctrico de la red gobernada, que puede ser un panel físico o una reproducción en pantalla.

### 4.3. Configuración y capacidad

Las prescripciones de la ET 03.359.120.7 exigen que el puesto central sea capaz de **controlar y supervisar al menos el doble de los elementos del telemando** sin necesidad de modificar software, licencias ni configuración (criterio de capacidad de procesamiento). Esta sobredimensionada previsión permite crecimientos de la red sin obras de adaptación.

### 4.4. Modelo de información

El modelo de información del puesto central se compone de:

- **Mensajes de tipo gráfico**: iconos de seccionadores, disyuntores, rearmadores y demás elementos del esquema unifilar, con su estado (abierto, cerrado, bloqueado) y color asociado.
- **Mensajes de tipo texto**: listados del histórico de eventos, alarmas y órdenes.

Cada señal del telemando queda identificada por un **mnemónico** normalizado y una **dirección** dentro del modelo de tablas de comunicaciones (ver lección 14 y el punto 10 de la parte 9/9).

### 4.5. Ramal de comunicación y canal

El ramal de comunicación enlaza cada remota (o concentrador de remotas) con el puesto central. En líneas convencionales se emplea el perfil **IEC 60870-5-101** (normalmente sobre enlaces serie o red), mientras que en líneas de alta velocidad se emplea el perfil **IEC 60870-5-104** sobre **TCP/IP** y una red WAN de muy alta disponibilidad. El canal físico es suministrado por ADIF Telecomunicaciones.

### 4.6. El concentrador de remotas

El **concentrador de comunicaciones** es el elemento del ramal que agrupa varias remotas y reenvía sus mensajes al puesto central. En el perfil ADIF IEC 60870-5-101, el concentrador tiene un papel decisivo en el direccionamiento: es el responsable de enviar las respuestas **directas** (interrogaciones `REQ`/`INROGEN` y confirmaciones `ACTCON`/`ACTTERM`) al centro de control que emitió la orden, identificado por el origen de aplicación (OA). De este modo, aunque convivan varios centros en la red, cada orden y su confirmación quedan inequívocamente asociadas.

### 4.7. Flujo de la información

1. La remota captura el estado de los elementos de campo y lo codifica en ASDU.
2. El ramal de comunicación transporta los ASDU hasta el concentrador y, desde este, al puesto central.
3. El puesto central actualiza el esquema, registra el evento y presenta la información al operador.
4. El operador emite una orden; el puesto central la codifica (ASDU + COT ACT + OA) y la envía por el ramal.
5. La remota ejecuta la maniobra, devuelve confirmación (ACTCON/ACTTERM) y el nuevo estado del elemento.
6. La intranet distribuye la información relevante al resto de sistemas (Base de Datos Central, JTMI, CTC).

---

## 5. FUNCIONES: TELEMANDO, TELEMEDIDA, TELESUPERVISIÓN, TELEALARMA

### 5.1. Telemando (control remoto)

Es la capacidad de enviar **órdenes** desde el puesto central a las instalaciones remotas y de recibir la **confirmación de ejecución**. Las órdenes normalizadas en el perfil ADIF IEC 60870-5-101 son las siguientes:

| Tipo | ASDU | Ejemplos de la tabla subestación |
|------|------|----------------------------------|
| Órdenes de dos posiciones (mando directo) | `C_SC_NA_1` | Cambio de modo Manual/Semiautomático/Automático (`AR___BMM`, `AR___BMS`, `AR___BMA`), desconexión general de emergencia (`AR___BDE`), rearme (`AR___BRE`), autorización de toma de mando (`ARSEBATM` para S/E, `ARLSBATM` para LS) |
| Órdenes de dos posiciones con doble mando (doble comando) | `C_DC_NA_1` | Apertura/cierre de seccionador tripolar de entrada (`LA11BAOA`/`LA11BAOC`), conexión/desconexión de disyuntor (`LA12BAOC`/`LA12BAOA`), órdenes de bloqueo/desbloqueo de seguridad (sufijo `B`/`D`) |

El ASDU `C_SC_NA_1` (single command) transmite una orden de una posición; el ASDU `C_DC_NA_1` (double command) transmite dos valores complementarios (p. ej. «abrir» y «cerrar»). En el perfil ADIF, cada orden lleva asociada su causa de transmisión (ACT/ACTCON/ACTTERM) y su origen de aplicación (OA).

### 5.2. Telemedida

Es la transmisión al puesto central de **medidas** (tensión, intensidad, potencia, energía, frecuencia) desde cada instalación. Permite al operador conocer la carga de cada subestación y tramo, detectar desequilibrios y prever la capacidad de servicio. En el modelo IEC 60870-5-101/104 se transmiten mediante ASDU de tipo medida (p. ej. `M_ME_NA_1`, medida normalizada; `M_ME_NC_1`, medida corta en coma flotante) con su factor de escala definido en el perfil de interoperabilidad.

Las telemedidas se agrupan en tres familias según su tratamiento en el puesto central:

| Tipo de medida | Tratamiento en el puesto central |
|----------------|----------------------------------|
| Periódica/cíclica (`PER/CYC`) | Refresco continuo de las magnitudes que el operador debe ver siempre actualizadas (tensiones de línea, intensidades de grupos y feeders). |
| Espontánea (`SPONT`) | Transmisión ante variación significativa de la magnitud, sin esperar al ciclo periódico. |
| Requerida (`REQ`) | Petición puntual del operador o del sistema (p. ej. lectura de energía para facturación o control). |

La escala y el factor de conversión de cada medida se fijan en el perfil de interoperabilidad, de modo que el valor mostrado en pantalla corresponde al valor real de la instalación.

### 5.3. Telesupervisión

Es la vigilancia del **estado de los equipos**: posición de seccionadores (abierto/cerrado), posición de disyuntores (conectado/desconectado), presencia de tensión, modo de funcionamiento de los rearmadores y de la subestación, disponibilidad de servicios auxiliares, estado de los ramales de comunicación y de los equipos del puesto central. Se materializa con señales de información de un bit (`M_SP_NA_1`), de dos bits (`M_DP_NA_1`) y con indicaciones temporizadas (`M_SP_TB_1`, `M_DP_TB_1`).

Las señales de supervisión se transmiten en tres situaciones:

- **Espontáneamente** cuando cambian de estado (causa `SPONT`).
- **Periódicamente** (causa `PER/CYC`) para refrescar el esquema y detectar caídas de comunicación.
- **Tras la interrogación general** (causa `INROGEN`) que el operador o el sistema lanza al iniciar sesión, al recuperarse una remota o periódicamente, para sincronizar todo el esquema.

Además de los estados de los aparatos, la telesupervisión incluye señales de **instalación** (p. ej. `P2 INSTALACIÓN EN MANDO`, con valores LOCAL/TELEMANDO) que condicionan la posibilidad de mando desde el puesto central.

### 5.4. Telealarma

Es la detección y presentación de **alarmas** por superación de umbrales, disparos de protecciones, fallos de comunicaciones o condiciones anómalas. Las alarmas se presentan con prioridad y tratamiento visual (iconos y colores) diferenciados, se registran en el histórico y pueden requerir reconocimiento explícito del operador. En el perfil IEC 60870-5-101 las alarmas se transmiten espontáneamente (causa de transmisión `SPONT`) y con retorno del estado tras su restablecimiento.

La gestión de alarmas en el puesto central incluye:

- **Jerarquía de prioridades**: cada alarma tiene asignado un nivel de importancia que determina su presentación (acústica, visual, número de pantallas).
- **Reconocimiento**: el operador confirma la toma de conocimiento; la alarma pasa de «activa sin reconocer» a «reconocida» y se archiva al desaparecer la causa.
- **Histórico de alarmas**: consulta por instalación, tipo, fecha o prioridad.
- **Alarmas de comunicaciones**: pérdida o recuperación de una remota, degradación de un ramal, fallo de un equipo del puesto central, que son alarmas del propio telemando y condicionan la fiabilidad de la información recibida.

### 5.5. Otras funciones operativas del puesto central

- **Registro de eventos y órdenes**: histórico de todas las señales, alarmas y maniobras con fecha y hora.
- **Reconocimiento de alarmas y gestión de avisos**: el operador confirma la toma de conocimiento de las alarmas.
- **Tratamiento del mando local**: si una instalación se encuentra en mando local, el puesto central lo indica y **no se permiten órdenes** hacia la misma (señal `P2 INSTALACIÓN EN MANDO`, valores LOCAL/TELEMANDO).
- **Interfaz con otros sistemas**: suministro de información a la intranet (Base de Datos Central, JTMI, CTC) y recepción de consignas.
- **Gestión de operadores**: identificación de cada operador, permisos de mando asignados y registro de las maniobras ejecutadas por cada uno (auditoría).
- **Visualización y navegación**: esquemas por instalación y por línea, vista general de la red y acceso directo a cada subestación, estación o seccionamiento.

### 5.6. Resumen de ASDU empleados en el perfil ADIF

| Tipo de tráfico | ASDU típicos | Sentido |
|-----------------|--------------|---------|
| Órdenes de mando directo | `C_SC_NA_1` | Centro → remota |
| Órdenes de doble mando | `C_DC_NA_1` | Centro → remota |
| Información de un bit | `M_SP_NA_1`, `M_SP_TB_1` | Remota → centro |
| Información de dos bits | `M_DP_NA_1`, `M_DP_TB_1` | Remota → centro |
| Medidas normalizadas | `M_ME_NA_1`, `M_ME_NC_1` | Remota → centro |
| Interrogación general | `C_IC_NA_1` / `INROGEN` | Centro ↔ remota |

El perfil ADIF no define ASDU no estándar: todas las señalizaciones se expresan con los ASDU de la norma IEC 60870-5, seleccionados y acotados en el perfil de interoperabilidad.

---

## 6. MANIOBRAS Y PROTECCIONES DESDE EL TELEMANDO

### 6.1. Maniobras ordinarias de subestación

Desde el puesto central se ejecutan las maniobras habituales de la subestación:

- **Cambio de modo de funcionamiento**: Manual (`AR___BMM`), Semiautomático (`AR___BMS`) y Automático (`AR___BMA`).
- **Autorización de toma de mando**: `ARSEBATM` (S/E) y `ARLSBATM` (LS). Permite a una subestación o centro de línea tomar el mando cuando corresponde (p. ej. tras una incidencia que exige pasar a local).
- **Llamada del operador a sirena**: `ARLLAMOS`, para avisar al personal presente en la instalación.
- **Apertura/cierre de seccionadores**: seccionador tripolar de entrada (LA1, LA2), seccionador de unión de barras BB/OO, seccionadores de salida de los grupos y feeders, seccionadores by-pass.
- **Conexión/desconexión de disyuntores**: disyuntores de las líneas de alta, disyuntores de los grupos de rectificadores, disyuntores extra-rrápidos de los feeders.
- **Conexión/desconexión de ruptofusibles e interruptores de BT**: interruptor de BT de servicios auxiliares, interruptor de BT de línea de señales, ruptoseccionadores de salida de transformador LS y de cada LS.

### 6.2. Bloqueos y desbloqueos de seguridad

Cada órgano de maniobra dispone de órdenes de **bloqueo de seguridad** (sufijo `B`) y **desbloqueo** (sufijo `D`): bloqueo del seccionador tripolar de entrada, del disyuntor de la línea de alta, de los seccionadores de salida, etc. El bloqueo de seguridad impide la maniobra del elemento desde el telemando (y en su caso desde local) hasta que se realice el desbloqueo. Estas órdenes son fundamentales para la protección de personas y bienes durante trabajos en la instalación.

### 6.3. El modelo de subestación en las tablas de comunicaciones

La parte 9/9 de la ET 03.359.120.7 define tres tablas de comunicaciones de subestación según su configuración, lo que muestra cómo crece el telemando con la instalación:

| Tipo de subestación | Configuración básica |
|---------------------|----------------------|
| Subestación tipo | Dos líneas de alta (LA1, LA2), un grupo de servicios auxiliares (SS/AA), tres líneas de señales (LS1, LS2, LS3), dos grupos (GR1, GR2) y tres feeders (F1, F3, F5). |
| Tipo con 1ª ampliación | La anterior más seis feeders (F1, F3, F5, F2, F4, F6) y un pórtico de seccionadores (PS-A1). |
| Tipo con 2ª ampliación | Tres líneas de alta (LA1, LA2, LA3), tres grupos (GR1, GR2, GR3), diez feeders y dos pórticos (PS-A1, PS-A2). |

Esta tabla define las señales y direcciones `IEC-IOA` de cada elemento (órdenes de apertura/cierre `...BAOA`/`...BAOC`, bloqueos `...BAOB`/`...BAOD`), de modo que el puesto central y la remota comparten un mismo mapeado y no se requiere programación ad hoc por instalación. Para estaciones (Z/N) se define una tabla común a ambos tipos (con o sin subestación), en la que algunas direcciones cambian de significado según el tipo de estación. Los centros de línea de señales (L/S) disponen de su propia tabla.

### 6.4. Rearme (ET 03.359.120.7 parte 2/9, punto 6.15.7.1)

El **rearme** (`AR___BRE`) es la maniobra que restaura el estado de la subestación tras la actuación de las protecciones. Tras un disparo, el operador, con la información de telemedidas y telesupervisión y previa verificación de que se han eliminado las causas, envía la orden de rearme para restablecer la alimentación. La orden se envía con causa de transmisión ACT y se confirma su ejecución (ACTCON/ACTTERM). El rearme puede aplicarse a la subestación completa o a elementos concretos.

### 6.5. Desconexión de emergencia (ET 03.359.120.7 parte 2/9, punto 6.15.7.2)

La **desconexión general de emergencia** (`AR___BDE`) es una orden de desconexión de la subestación ante una situación de peligro inminente para personas o bienes (p. ej. accidente en la catenaria, incendio, circulación insegura). Presenta un tratamiento visual específico: icono de emergencia en **amarillo** cuando no está activa y en **rojo intermitente** cuando se encuentra activada, y **requiere confirmación del operador** antes de ejecutarse, dado su efecto drástico sobre el suministro. El restablecimiento se realiza de forma controlada, habitualmente tramo a tramo, y solo cuando se ha garantizado la seguridad.

### 6.6. Maniobras de estaciones, seccionamientos y líneas de señales

Además de la subestación, el telemando gobierna la aparamenta repartida por la línea:

- **Estaciones (Z/N)**: bloqueo y desbloqueo de seguridad de los seccionadores de la estación, con la doble interpretación de direcciones según exista o no subestación asociada (p. ej. la dirección de bloqueo del seccionador ordinario S 6.6 corresponde, en una estación sin subestación, al seccionador S 2.6).
- **Centros de línea de señales (L/S)**: orden por T/M de cambio a modo Manual/Semiautomático/Automático (`AR_LSBOM`, `AR_LSBOS`, `AR_LSBOA`), autorización de toma de mando (`ARLSBATM`) y maniobra de sus seccionamientos y ruptoseccionadores.
- **Seccionamientos en vía**: conexión o desconexión de los seccionadores de tramo para aislar zonas de trabajo o para reconfigurar la alimentación.

### 6.7. Seguridad de las maniobras

- Las órdenes se transmiten con doble mando y confirmación: el equipo ejecuta la maniobra y devuelve el nuevo estado del elemento.
- La **causa de transmisión** distingue órdenes (ACT), confirmaciones (ACTCON) y terminaciones (ACTTERM), permitiendo al operador saber en todo momento si la maniobra se ha aceptado y ejecutado.
- Las instalaciones en **mando local** no pueden ser mandadas desde el telemando; la señal P2 INSTALACIÓN EN MANDO lo refleja en el puesto central.
- Los **bloqueos de seguridad** y los **enclavamientos** lógicos impiden maniobras indebidas (apertura de seccionador con carga, cierre con toma de tierra colocada, etc.).

### 6.8. Ciclo completo de una maniobra y actuación de las protecciones

El ciclo de una maniobra típica desde el telemando es el siguiente:

1. El operador selecciona el elemento en el esquema y solicita la maniobra (p. ej. cierre del seccionador tripolar de entrada LA1).
2. El puesto central verifica que la instalación está en telemando, que el elemento no está bloqueado y que el operador tiene permisos.
3. Se envía el ASDU de orden (`C_SC_NA_1` o `C_DC_NA_1`) con causa `ACT` y el origen de aplicación del centro.
4. La remota responde con la confirmación de actuación (`ACTCON`) y, tras ejecutarse, con la terminación (`ACTTERM`) y el nuevo estado del elemento.
5. El puesto central actualiza el esquema y registra la maniobra en el histórico.

Si la protección actúa (disparo), el proceso es inverso: la remota envía espontáneamente (`SPONT`) el cambio de estado del elemento protegido y las alarmas asociadas; el operador recibe la alarma, analiza las telemedidas y decide si procede el rearme o la intervención presencial.

---

## 7. REQUISITOS DE LAS ET (PROTOCOLOS, SEGURIDAD, FIABILIDAD, REDUNDANCIA)

### 7.1. Disponibilidad y fiabilidad del puesto central

La ET 03.359.120.7 parte 2/9 establece requisitos muy exigentes:

- **Funciones de alta disponibilidad**: disponibilidad mensual **superior al 99,98 %** y disponibilidad media anual **superior al 99,5 %**.
- **Redundancia**: los elementos críticos del puesto central se configuran de forma redundante (equipos de proceso duplicados, alimentación doble, enlaces de comunicaciones redundantes) de modo que una avería no produzca pérdida de la función.
- **Capacidad de procesamiento**: controlar y supervisar al menos el doble de elementos del telemando sin cambios de software, licencias o configuración.

### 7.2. Protocolo IEC 60870-5-101 (perfil ADIF, líneas convencionales)

La parte 9/9 de la ET 03.359.120.7 define el perfil de interoperabilidad ADIF basado en la norma IEC 60870-5-101. Aspectos clave:

- **ASDU** (Application Service Data Unit): unidades de datos que transportan las señales. El perfil ADIF emplea ASDU estándar de la norma (no se definen ASDU no estándar).
- **Causas de transmisión (COT)**: el bit de test no se utiliza (se fija a 0). Causas empleadas: `PER/CYC` (periódica/cíclica), `SPONT` (espontánea), `INIT` (inicialización), `REQ` (requerida), `ACT` (actuación de orden), `ACTCON` (confirmación de actuación), `ACTTERM` (terminación de actuación), `INROGEN` (interrogación general). En el sentido centro a remota, las causas 44 (tipo ASDU desconocido) y 45 (causa de transmisión desconocida) se utilizan como respuesta de error.
- **Origen de aplicación (OA)**: identifica al centro de control que envía la orden (valores 1 a 254 asignados por ADIF). El valor 0 se emplea para el resto de ASDU. El concentrador de comunicaciones envía las respuestas directas (REQ, INROGEN, ACTCON, ACTTERM) al centro que emitió la orden.
- **Direccionamiento IEC-IOA**: cada señal tiene una dirección única (p. ej. `009000` para la apertura del seccionador tripolar de entrada LA1). Las tablas del capítulo 10 (modelo de tablas de comunicaciones) definen los mapeados de subestación, estación y centro de línea de señales, diferenciando los tipos de subestación según su número de grupos y feeders.
- **Número máximo de objetos**: en el modelo ADIF se limitan los objetos IEC por ASDU (p. ej. máximo 127 objetos en los ASDU de interrogación), de modo que los mensajes no excedan el tamaño del buffer del canal.

### 7.3. Protocolo IEC 60870-5-104 (perfil ADIF, líneas de alta velocidad)

La ET 03.359.501.8 define el perfil de interoperabilidad ADIF para líneas de alta velocidad, basado en la norma **IEC 60870-5-104**. Aspectos clave:

- **Transporte TCP/IP**: los mensajes IEC 60870-5-101 se encapsulan sobre TCP/IP, lo que permite el uso de una red WAN de muy alta disponibilidad y baja latencia.
- **Número de secuencia**: los ASDU llevan número de secuencia que permite detectar pérdidas y duplicaciones de mensajes y recuperar la sincronización.
- **Sin etiqueta de tiempo en las órdenes**: el perfil ADIF no utiliza la etiqueta de tiempo en las órdenes; la secuencia numérica y los temporizadores de la norma (timeouts) son suficientes para garantizar la entrega y el orden.
- **Arquitectura**: se representan los centros de control, las remotas, los concentradores de remotas y los gateways/pasarelas. La norma no especifica las funcionalidades propias de centros de control y remotas (quedan fuera de su alcance), pero sí la interoperabilidad entre equipos de distintos suministradores.
- **Comparación con el modelo OSI**: el perfil 104 utiliza la pila TCP/IP sobre el modelo de referencia, frente a los perfiles serie del 101. Ambas normas comparten la semántica de las ASDU y de las causas de transmisión.
- **Direccionamiento y puestos externos**: se contemplan hasta **254 puestos locales externos** en los telemandos de alta velocidad (centros de control central y regional), manteniendo la asignación de OA de la norma 101.

### 7.4. Requisitos de seguridad

- **Seguridad funcional**: imposibilidad de maniobrar instalaciones en mando local, enclavamientos y bloqueos de seguridad, confirmación de órdenes.
- **Seguridad de la información**: acceso de los operadores controlado, registro de eventos y órdenes (auditoría) y protección de los enlaces de comunicaciones.
- **Seguridad de las personas y bienes**: desconexión de emergencia, órdenes de bloqueo para trabajos, sirenas de aviso al personal de instalación.

### 7.5. Redundancia y mantenibilidad

- Redundancia de equipos, alimentaciones y enlaces en el puesto central y en los elementos críticos de las remotas.
- Diagnosis del estado de los ramales de comunicación desde el puesto central.
- Diseño modular que permita sustituir equipos sin pérdida de información ni de funciones, y que facilite el crecimiento futuro (capacidad al doble de elementos).

---

## 8. COORDINACIÓN CON SSEE (ET 03.359.1XX/5XX) Y CON NAE 112/119 (ESQUEMAS)

### 8.1. Coordinación con las especificaciones de subestaciones y de alta velocidad

El telemando de energía no actúa en vacío: gobierna instalaciones cuyo diseño, montaje y protecciones se definen en otras especificaciones del sistema ET 03.359:

- **ET 03.359.1xx**: prescripciones de subestaciones de tracción (rectificadores, transformadores, servicios auxiliares, protecciones, aparamenta) en líneas convencionales.
- **ET 03.359.5xx**: especificaciones de los telemandos de energía de líneas de alta velocidad, incluyendo la ET 03.359.501.8 (protocolo 104) y las relativas a los centros de autotransformación (CAT) y puestos de autotransformación.
- **Seccionamientos**: los seccionamientos en vía, estaciones y centros de línea de señales se representan en las tablas de comunicaciones de la parte 9/9 (señales `LS...`, `Z/N`, `L/S`) y su explotación se coordina con el mando de la circulación.

La coordinación operativa significa que:

- El **diseño de cada subestación** debe reservar los elementos (seccionadores, disyuntores, rearmadores, transformadores de medida) y las señales que exige el modelo de tablas del telemando.
- Las **protecciones** actúan sobre los mismos elementos que maniobra el telemando: tras un disparo, el estado del elemento se comunica al puesto central y solo el rearme autorizado restablece la alimentación.
- Las **ampliaciones** (segundo o tercer grupo, nuevos feeders, pórticos de seccionadores) deben ser incorporables a las tablas de comunicaciones sin alterar el perfil de interoperabilidad.

### 8.2. Coordinación con las NAE 112 y NAE 119 (esquemas eléctricos)

Las NAE definen los esquemas eléctricos normalizados:

- **NAE 112**: esquemas eléctricos de los sistemas de tracción en **corriente continua** (3 kV CC).
- **NAE 119**: esquemas eléctricos de los sistemas de tracción en **corriente alterna** (25 kV 50 Hz y otras).

La relación con el telemando:

- El **esquema unifilar** que se visualiza en el puesto central reproduce, de forma simplificada e interactiva, el esquema eléctrico definido en las NAE: subestación, grupos de rectificación, feeders, seccionamientos y puntos de conexión a la línea de contacto.
- Los **iconos y estados** del puesto central (abierto, cerrado, bloqueado, sin tensión) corresponden a los elementos representados en los esquemas NAE, de modo que el operador ve en el telemando lo mismo que el mantenedor ve en el plano.
- Las **maniobras telemando** deben ser coherentes con las reglas de explotación que derivan del esquema eléctrico (por ejemplo, no abrir un seccionador con carga, respetar el orden de conexión de seccionadores y disyuntores).
- Tanto en CC como en CA, el telemando de energía es el instrumento que hace **operativo** el esquema: el esquema define cómo es la instalación y el telemando define cómo se maniobra.

### 8.3. Flujo de la información en la coordinación

1. La instalación (diseñada según ET 03.359.1xx/5xx y esquematizada según NAE 112/119) envía sus señales a la remota.
2. La remota codifica las señales en ASDU según el perfil 101 (convencional) o 104 (alta velocidad).
3. El ramal de comunicación transporta los ASDU hasta el concentrador y el puesto central.
4. El puesto central presenta la información en el esquema del operador, registra eventos y permite las órdenes.
5. Las órdenes regresan por el mismo camino hasta el elemento de campo, que ejecuta la maniobra y confirma.
6. La intranet distribuye la información relevante a la Base de Datos Central, la Gestión Técnica (JTMI) y el CTC.

---

## 9. AUTOEVALUACIÓN (10 PREGUNTAS)

1. **¿Qué es el telemando de energía y cuáles son los tres componentes que forman parte de él en la arquitectura de ADIF?**
   Es el sistema de control remoto de las instalaciones de alimentación eléctrica del ferrocarril. Forman parte de él: las remotas, los ramales de comunicación y el puesto central. La intranet de ADIF (Base de Datos Central, JTMI, CTC) se sitúa por encima y no pertenece al telemando propiamente dicho.

2. **¿Qué papel desempeñan el puesto central, el centro de control y la remota (RTU) en la arquitectura?**
   La remota (RTU) recoge las señales de campo y ejecuta las órdenes; el centro de control aloja el puesto central, que supervisa la red, presenta alarmas y medidas y permite enviar órdenes; el puesto central es el conjunto de equipos de explotación (puestos fijos, puestos volantes, base de datos, histórico, impresión, sinóptico).

3. **¿Cuáles son las cuatro funciones clásicas del telemando y a qué se refiere cada una?**
   Telemando (envío de órdenes y confirmación), telemedida (transmisión de tensiones, intensidades y potencias), telesupervisión (estado de los equipos) y telealarma (detección y presentación de alarmas). A ellas se añaden el registro de eventos, el reconocimiento de alarmas y el tratamiento del mando local.

4. **¿Qué es la señal P2 INSTALACIÓN EN MANDO y qué consecuencias tiene en la explotación?**
   Es la señal que indica si una instalación se encuentra en mando local o en telemando. Si la instalación está en mando local, el puesto central lo refleja y **no se permiten órdenes** hacia la misma, garantizando la seguridad frente a maniobras simultáneas.

5. **Describa las maniobras de rearme y de desconexión de emergencia.**
   El rearme (`AR___BRE`) restaura el estado de la subestación tras un disparo y requiere verificar que se han eliminado las causas. La desconexión de emergencia (`AR___BDE`) es la orden general de desconexión ante peligro para personas o bienes; se representa en amarillo (no activa) y rojo intermitente (activada) y **requiere confirmación del operador**.

6. **¿Qué diferencia existe entre las órdenes `C_SC_NA_1` y `C_DC_NA_1`? Ponga ejemplos del perfil ADIF.**
   `C_SC_NA_1` (mando directo) transmite una orden de una posición: cambio de modo Manual/Semiautomático/Automático, rearme, desconexión de emergencia, autorización de toma de mando. `C_DC_NA_1` (doble mando) transmite dos valores complementarios: apertura/cierre de seccionadores y conexión/desconexión de disyuntores y ruptofusibles.

7. **¿Qué son el OA (origen de aplicación) y el COT (causa de transmisión) en el perfil IEC 60870-5-101 de ADIF?**
   El OA identifica al centro de control que emite la orden (valores 1-254 asignados por ADIF; 0 para el resto de ASDU) y permite al concentrador responder al centro correcto. El COT indica el motivo de la transmisión: PER/CYC, SPONT, INIT, REQ, ACT, ACTCON, ACTTERM, INROGEN, además de los errores 44 y 45.

8. **¿Qué mejoras aporta el perfil IEC 60870-5-104 de la ET 03.359.501.8 respecto al 101?**
   Utiliza TCP/IP sobre una red WAN de muy alta disponibilidad, incorpora número de secuencia para detectar pérdida o duplicación de mensajes, no emplea etiqueta de tiempo en las órdenes (bastan secuencia y timeouts) y permite hasta 254 puestos locales externos, manteniendo la misma semántica de ASDU y COT.

9. **¿Qué requisitos de disponibilidad, capacidad y seguridad fija la ET 03.359.120.7 para el puesto central?**
   Funciones de alta disponibilidad superiores al 99,98 % mensual y disponibilidad media superior al 99,5 % anual; capacidad de procesamiento para al menos el doble de elementos sin cambios de software o licencias; redundancia de equipos críticos, alimentación y enlaces; seguridad funcional (mando local, enclavamientos, confirmaciones) y registro de eventos y órdenes.

10. **¿Cómo se coordina el telemando con las ET 03.359.1xx/5xx y con las NAE 112/119?**
    Las ET de subestaciones (03.359.1xx) y de alta velocidad (03.359.5xx) definen los elementos que el telemando maniobra y sus señales; las NAE 112 (CC) y NAE 119 (CA) definen los esquemas eléctricos que el puesto central reproduce en su interfaz gráfica. El telemando convierte el esquema eléctrico en un sistema explotable a distancia, respetando las reglas de maniobra derivadas del esquema.

---

## 10. REFERENCIAS

- **ET 03.359.120.7**, *«Prescripciones técnicas y funcionales para el suministro y montaje de telemandos de energía (Líneas Convencionales). Puesto Central»*, parte 2/9. 1ª edición, febrero 2007. ADIF, D. Gestión Operativa de Activos, Área de Tecnología Operativa, Gabinete de Electrificación.
- **ET 03.359.120.7**, *«Protocolo de comunicaciones entre centro de control y remotas (líneas convencionales). Perfil de interoperabilidad ADIF IEC 60870-5-101»*, parte 9/9. 1ª edición, febrero 2007. ADIF, D. Gestión Operativa de Activos, Área de Tecnología Operativa, Gabinete de Electrificación.
- **ET 03.359.501.8**, *«Protocolo de comunicaciones entre centro de control y remotas en telemandos de energía de líneas de alta velocidad. Perfil de interoperabilidad ADIF IEC 60870-5-104»*. 1ª edición, abril 2008. Aprobada por el Presidente del Comité para la Gestión del Conocimiento (Madrid, 30 de abril de 2008).
- Normas del Comité IEC 60870-5-101 y IEC 60870-5-104, *Telecontrol equipment and systems — Transmission protocols*.
- **NAE 112**, esquemas eléctricos de los sistemas de tracción en corriente continua (Módulo 5, lección 5).
- **NAE 119**, esquemas eléctricos de los sistemas de tracción en corriente alterna (Módulo 5, lección 6).
- Módulo 5, lección 14: *Telemando de energía (I): introducción y normativa ET 03.359*.
