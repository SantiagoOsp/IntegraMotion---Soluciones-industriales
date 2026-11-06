# IntegraMotion · Soluciones industriales 5.0

**Ingeniería y automatización**

Proyecto integrador de Automatización de Procesos de Manufactura.

**Empresa integradora:** IntegraMotion  
**Cliente:** Lácteos Fúquene S.A.S.  
**Ubicación de la planta:** Ubaté, Colombia.

## Equipo de trabajo

| Integrante | Cargo | Responsabilidad |
|---|---|---|
| Santiago Ospina | CEO | Identidad empresarial y transformación digital. |
| Marco Morales | CTO | Transformación digital, modelos ISA-88 e ISA-95 y edición. |
| Dixon Cuesta | CFO | Gestión, administración y finanzas |
| Yesid Ojeda | COO | Simulación en Tecnomatix y diseño del layout. |
| Juan Andres Moreno | CDO | Identidad empresarial y transformación digital. |
| Carlos Guzmán | CCO | EDT del proyecto y estructuración de la información. |

---

## 1. Descripción general

IntegraMotion propone una solución de automatización y transformación digital para la planta de Lácteos Fúquene S.A.S., ubicada en Ubaté. La planta considera una alimentación de **25.000 L de leche por día**, distribuida entre yogur, quesos y productos UHT, con tres referencias por línea.

El desarrollo detallado de recetas, control y gemelo digital se concentra en la **línea de quesos: campesino, doble crema y mozzarella**. ISA-88 estructura sus equipos, secuencias y recetas. ISA-95 organiza la integración entre proceso, control, supervisión, gestión de operaciones y gestión empresarial, con una visión de las tres líneas y sus recursos compartidos.

La propuesta vincula órdenes, lotes, materiales, condiciones de fabricación y resultados de calidad mediante una arquitectura OT/IT. Las cantidades, capacidades y parámetros de este documento corresponden al **escenario de diseño**; los resultados de ejecución se registran por separado.


## 2. Objetivos de Transformación Digital Industrial

### Objetivo general

Diseñar la arquitectura de automatización e información de la planta, aplicando ISA-88 a la línea de quesos e ISA-95 a la integración entre operación y gestión.

### Objetivos específicos

- Caracterizar las tres líneas, sus referencias y recursos compartidos.
- Estructurar la celda de quesos, unidades, módulos de equipo y módulos de control.
- Definir recetas, cantidades por lote, secuencias y condiciones de ejecución.
- Identificar sensores, actuadores, variables críticas y confirmaciones manuales.
- Asignar responsabilidades a control, SCADA, funciones MES y ERP.
- Definir interfaces y registros de órdenes, consumos, calidad y trazabilidad.
- Establecer una base común de equipos, estaciones y parámetros para control y gemelo digital de quesos.

## 3. EDT del Proyecto

  ### Objetivo general
La EDT organiza el proyecto en entregables y paquetes de trabajo. Su alcance comprende desde la planeación inicial hasta la integración y validación de la solución propuesta. Estos objetivos se realizan de forma parcialmente paralela, en un periodo de 16 semanas.

```mermaid
flowchart TD
    P["Consultora de Ingeniería IntegraMotion<br/>25.000 L/día"]

    P --> A["1. Gestión<br/>del proyecto"]
    P --> B["2. Ingeniería<br/>de proceso"]
    P --> C["3. Automatización<br/>y control"]
    P --> D["4. Robótica<br/>y simulación"]
    P --> E["5. MES<br/>y ERP"]
    P --> F["6. Finanzas<br/>y oferta"]

    A --> A1["1.1 Inicio<br/>y planeación"]
    A --> A2["1.2 Seguimiento<br/>y compuertas"]
    A --> A3["1.3 Informe final<br/>y sustentación"]

    B --> B1["2.1 Análisis<br/>del problema"]
    B --> B2["2.2 EDT de la<br/>producción"]
    B --> B3["2.3 VSM de<br/>las líneas"]
    B --> B4["2.4 Medidas<br/>organizacionales"]
    B --> B5["2.5 Arquitectura<br/>ISA-95"]

    C --> C1["3.1 Instrumentación"]
    C --> C2["3.2 PLC<br/>e ISA-88"]
    C --> C3["3.3 SCADA"]

    D --> D1["4.1 Plant Simulation"]
    D --> D2["4.2 RobotStudio"]
    D --> D3["4.3 NX MCD"]

    E --> E1["5.1 Implementación<br/>MES"]
    E --> E2["5.2 Implementación<br/>ERP"]
    E --> E3["5.3 Integración<br/>y comunicación"]

    F --> F1["6.1 Modelo financiero<br/>y oferta"]
    F --> F2["6.2 Financiación"]

    classDef principal fill:#08045f,stroke:#08045f,color:#ffffff,stroke-width:2px;
    classDef nivelUno fill:#eeeeff,stroke:#6666cc,color:#17172f,stroke-width:1px;
    classDef paquete fill:#ffffff,stroke:#7777cc,color:#202020,stroke-width:1px;

    class P principal;
    class A,B,C,D,E,F nivelUno;
    class A1,A2,A3,B1,B2,B3,B4,B5,C1,C2,C3,D1,D2,D3,E1,E2,E3,F1,F2 paquete;
```

### 3.1 Desglose de tiempos
A continuación se presentan los tiempos estimados para cada etapa del proyecto:

#### Gestión del proyecto
| Código | Actividad | Duración | Objetivo |
|---|---|---:|---|
| 1.1 | Inicio y planeación | 2 semanas | Definir y aprobar el alcance, los requisitos, las responsabilidades y la EDT inicial del proyecto. |
| 1.2 | Seguimiento y compuertas | 16 semanas | Controlar el avance, los riesgos, los cambios y las decisiones mediante reuniones periódicas y revisiones de los hitos. |
| 1.3 | Informe final y sustentación | 2 semanas | Integrar los resultados de todos los frentes, preparar los anexos y presentar la sustentación final de la consultoría. |

#### Ingeniería de proceso
| Código | Actividad | Duración | Objetivo |
|---|---|---:|---|
| 2.1 | Análisis del problema | 2 semanas | Diagnosticar la situación actual de la planta e identificar la demanda, las capacidades, las restricciones y los criterios de diseño. |
| 2.2 | EDT de la producción | 3 semanas | Desglosar el proceso productivo en operaciones, equipos, recetas, secuencias y parámetros controlables. |
| 2.3 | VSM de las líneas | 3 semanas | Analizar los flujos de materiales e información para identificar desperdicios, tiempos de espera y oportunidades de mejora. |
| 2.4 | Medidas organizacionales | 2 semanas | Definir los roles, los turnos, las competencias y los procedimientos necesarios para implementar las mejoras propuestas. |
| 2.5 | Arquitectura ISA-95 | 3 semanas | Diseñar la arquitectura y los flujos de información entre los niveles operativos y los sistemas empresariales. |

#### Automatización y control
| Código | Actividad | Duración | Objetivo |
|---|---|---:|---|
| 3.1 | Instrumentación | 3 semanas | Seleccionar y especificar los instrumentos, sensores y actuadores requeridos para medir y controlar las variables del proceso. |
| 3.2 | PLC e ISA-88 | 4 semanas | Diseñar la lógica de control, las secuencias, las fases, los módulos y los interbloqueos de seguridad del proceso. |
| 3.3 | SCADA | 3 semanas | Diseñar las pantallas de supervisión, alarmas, tendencias e indicadores para monitorear y operar el proceso. |

#### Robótica y simulación
| Código | Actividad | Duración | Objetivo |
|---|---|---:|---|
| 4.1 | Plant Simulation | 4 semanas | Construir un modelo de eventos discretos que permita evaluar la capacidad, las rutas, los turnos, las fallas y diferentes escenarios productivos. |
| 4.2 | RobotStudio | 3 semanas | Diseñar y validar virtualmente una celda robotizada, considerando el alcance del robot, los patrones de estiba, el efector final y la seguridad. |
| 4.3 | NX MCD | 4 semanas | Crear un gemelo virtual mecatrónico para validar la cinemática, las señales, las secuencias y la interacción con un PLC virtual. |

#### MES y ERP

| Código | Actividad | Duración | Objetivo |
|---|---|---:|---|
| 5.1 | Implementación MES | 4 semanas | Diseñar el modelo MES para gestionar órdenes, recetas, lotes, trazabilidad e indicadores de producción. |
| 5.2 | Implementación ERP | 4 semanas | Definir la configuración funcional del ERP para integrar compras, inventarios, costos y ventas. |
| 5.3 | Integración y comunicación | 2 semanas | Diseñar y probar las interfaces de comunicación entre MES, ERP y SCADA. |

#### Finanzas y oferta

| Código | Actividad | Duración | Objetivo |
|---|---|---:|---|
| 6.1 | Modelo financiero y oferta | 12 semanas intermitentes | Evaluar la viabilidad económica del proyecto y construir el caso de negocio, el flujo de caja y el precio de la oferta. |
| 6.2 | Financiación | 3 semanas | Definir una estructura de financiación basada en los hitos de pago, el flujo de caja y alternativas como crédito o leasing. |


## 4. Planta, productos y selección de línea

| Línea | Referencias y presentación | Leche asignada por día | Participación |
|---|---|---:|---:|
| Yogur | Natural azucarado, fresa y mora. Vasos de 150 g. | 4.000 L | 16 % |
| **Quesos** | **Q1 campesino y Q2 doble crema, 500 g; Q3 mozzarella, 2,5 kg.** | **9.000 L** | **36 %** |
| UHT | Entera y deslactosada, 1 L; chocolate, 200 mL. | 12.000 L | 48 % |
| **Total** | **Tres líneas y nueve referencias.** | **25.000 L** | **100 %** |

```mermaid
flowchart TD
    REC["Recepción de leche<br/>25.000 L/día"]
    Y["Yogur: 4.000 L/día<br/>Natural, fresa y mora"]
    Q["Quesos: 9.000 L/día<br/>Línea seleccionada"]
    U["UHT: 12.000 L/día<br/>Entera, deslactosada y chocolate"]
    Q1["Q1 campesino<br/>4.500 L por lote diario"]
    Q2["Q2 doble crema<br/>3.000 L por lote diario"]
    Q3["Q3 mozzarella<br/>1.500 L por lote diario"]
    REC --> Y
    REC --> Q
    REC --> U
    Q --> Q1
    Q --> Q2
    Q --> Q3
    classDef seleccionado fill:#dff3e8,stroke:#19865b,color:#123b2c,stroke-width:2px;
    class Q,Q1,Q2,Q3 seleccionado;
```

### Justificación técnica de quesos

La selección se sustenta en rutas diferenciadas y recursos compartidos. Campesino requiere lavado, prensado y oreo; doble crema y mozzarella requieren acidificación de cuajada e hilado, con ingredientes y acondicionamiento diferentes.

El VSM identifica el hilado compartido como recurso limitante del escenario inicial. Para aproximadamente 552 kg/día, una tasa de 70 kg/h requiere 7,89 h de proceso; con 30 min de limpieza, 8,39 h frente a una ventana de 7,4 h. La propuesta considera 300 kg/h, equivalentes a 1,84 h de proceso más limpieza. Son **estimaciones del recurso**, no resultados de desempeño de toda la línea.

Esta línea permite relacionar la selección de recetas con la reserva de equipos, las condiciones de proceso y la trazabilidad de producto y suero.

## 5. Distribución y flujo de proceso

La distribución de diseño considera **67 × 30 m**, 22 estaciones y aproximadamente 192,9 m² de huellas de equipos. Las dimensiones de equipos constituyen la base de implantación. El siguiente diagrama representa conexiones funcionales, sin escala geométrica.

```mermaid
flowchart LR
    subgraph zonaLeche ["Zona A–B · Leche"]
        estRecepcion["E01 Recepción y filtro"]
        estSilos["E02 Silos 1 y 2"]
        estEstandarizacion["E03 Descremadora y remezcla"]
        estPasteurizador["E04 Pasteurizador HTST"]
        estRecepcion --> estSilos --> estEstandarizacion --> estPasteurizador
    end
    subgraph zonaTinas ["Zona C · Tinas"]
        estTinaCampesino["E05 Tina 1 · Q1"]
        estTinaDobleCrema["E06 Tina 2 · Q2"]
        estTinaMozzarella["E07 Tina 3 · Q3"]
    end
    subgraph zonaFormado ["Zona D · Formado"]
        estSalado["E08 Salado en masa"]
        estPrensa["E09 Moldeo y prensa"]
        estOreo["E10 Oreo y desmolde"]
        estAcidezDobleCrema["E11 Acidificación Q2"]
        estAcidezMozzarella["E12 Acidificación Q3"]
        estHiladora["E13 Hiladora-moldeadora"]
        estFrioDobleCrema["E14 Enfriamiento Q2"]
        estSalmuera["E15 Agua y salmuera Q3"]
    end
    subgraph zonaEmpaque ["Zona E · Empaque"]
        estTermoformadora["E16 Termoformadora Q1/Q2"]
        estEmpacadoraMozzarella["E17 Empacadora y túnel Q3"]
        estInspeccion["E18 Codificación, peso y metales"]
    end
    subgraph zonaDespacho ["Zona F · Despacho"]
        estEncajado["E19 Encajado"]
        estPaletizado["E20 Paletizado · etapa 3"]
        estCamaraFinal["E21 Cámaras de producto terminado"]
        estCargue["E22 Alistamiento y cargue"]
    end
    estPasteurizador --> estTinaCampesino
    estPasteurizador --> estTinaDobleCrema
    estPasteurizador --> estTinaMozzarella
    estTinaCampesino --> estSalado --> estPrensa --> estOreo --> estTermoformadora
    estTinaDobleCrema --> estAcidezDobleCrema --> estHiladora
    estTinaMozzarella --> estAcidezMozzarella --> estHiladora
    estHiladora --> estFrioDobleCrema --> estTermoformadora
    estHiladora --> estSalmuera --> estEmpacadoraMozzarella
    estTermoformadora --> estInspeccion
    estEmpacadoraMozzarella --> estInspeccion
    estInspeccion --> estEncajado --> estPaletizado --> estCamaraFinal --> estCargue
    classDef campesino fill:#e1f3e7,stroke:#278655,color:#123b2c;
    classDef pastaHilada fill:#fff0df,stroke:#c86b20,color:#60370c;
    classDef compartido fill:#e5eaf8,stroke:#536ba5,color:#1b2c50,stroke-width:2px;
    class estTinaCampesino,estSalado,estPrensa,estOreo campesino;
    class estTinaDobleCrema,estTinaMozzarella,estAcidezDobleCrema,estAcidezMozzarella,estFrioDobleCrema,estSalmuera,estEmpacadoraMozzarella pastaHilada;
    class estHiladora,estTermoformadora,estInspeccion,estEncajado,estPaletizado,estCamaraFinal,estCargue compartido;
```

Los equipos de recepción, silos, tratamiento inicial y servicios se coordinan con la planta. CIP es un servicio auxiliar fuera de la numeración E01–E22. E13 comparte capacidad entre Q2/Q3, E16 entre Q1/Q2 y E20 se plantea como recurso de paletizado compartido por las líneas.

<details>
<summary>Plano de distribución y referencia gráfica de estaciones</summary>

![Distribución de diseño de la planta de quesos de 67 por 30 metros](docs/tdi/imagenes/distribucion_planta_quesos.png)

![Flujo de referencia con las 22 estaciones de quesos](docs/tdi/imagenes/flujo_estaciones_quesos.png)

Los planos corresponden a la base de diseño del equipo. La numeración se conserva en los diagramas y las tablas de este documento.

</details>

## 6. Aplicación de ISA-88

### 6.1 Modelo físico

| Nivel | Aplicación |
|---|---|
| Empresa | Lácteos Fúquene S.A.S. |
| Sitio | Planta Ubaté. |
| Área | Fabricación de quesos. |
| Celda de proceso | PC-QUE: campesino Q1, doble crema Q2 y mozzarella Q3. |
| Unidades | Tinas, acidificación, prensa, hilado y acondicionamiento. |
| Módulos de equipo | Carga, dosificación, regulación térmica, agitación/corte y desuerado. |
| Módulos de control | Bomba, válvula, accionamiento de motor, mediciones y lazo térmico. |

```mermaid
flowchart TD
    EMP["Lácteos Fúquene S.A.S."] --> SIT["Planta Ubaté"]
    SIT --> AREA["Área de quesos"]
    AREA --> CEL["PC-QUE"]
    CEL --> T1["TQ-301 / E05 · Q1"]
    CEL --> T2["TQ-302 / E06 · Q2"]
    CEL --> T3["TQ-303 / E07 · Q3"]
    CEL --> UNI["Prensa E09, mesas E11/E12,<br/>hilado E13 y acondicionamiento E14/E15"]
    T1 --> CARGA["EM-301-Carga"]
    T1 --> TERM["EM-301-Térmico"]
    CARGA --> BOMBA["P-301 · Bomba"]
    CARGA --> VALV["XV-301 · Válvula"]
    CARGA --> MED["FT-301 · Caudal<br/>LT/LSHH-301 · Nivel"]
    TERM --> LAZO["TT-301 y regulación<br/>de la camisa térmica"]
```

| Unidad / estación | Función | Receta |
|---|---|---|
| TQ-301 / E05 | Tina 1, 5.000 L nominales; lote de 4.500 L. | Q1 |
| TQ-302 / E06 | Tina 2, 5.000 L nominales; lote de 3.000 L. | Q2 |
| TQ-303 / E07 | Tina 3, 5.000 L nominales; lote de 1.500 L. | Q3 |
| PR-305 / E09 | Moldeo y prensado de piezas de 500 g. | Q1 |
| AC-311 / E11 | Acidificación de cuajada; pH de diseño 5,1–5,3. | Q2 |
| AC-312 / E12 | Acidificación de cuajada; pH de diseño 5,1–5,3. | Q3 |
| HI-306 / E13 | Hilado y moldeo; incorporación de crema y sal en Q2. | Q2/Q3 |
| CF-314 / E14 | Enfriamiento de doble crema. | Q2 |
| SA-307 / E15 | Agua fría y salmuera para mozzarella. | Q3 |

IntegraMotion actúa como integradora de la solución; Lácteos Fúquene es la empresa representada en la jerarquía del proceso.

### 6.2 Modelo procedimental

| Nivel | Aplicación a campesino Q1 |
|---|---|
| Procedimiento | Fabricar un lote de campesino. |
| Procedimiento de unidad | Elaborar cuajada en TQ-301. |
| Operación | Preparar leche para coagulación. |
| Fases | Verificar disponibilidad, cargar, ajustar temperatura, dosificar y confirmar adiciones. |

| Producto | Ruta después del tratamiento inicial E01–E04 |
|---|---|
| Q1 | E05: elaboración; E08: salado; E09: moldeo/prensa; E10: oreo; E16: termoformado; E18–E22: inspección y despacho. |
| Q2 | E06: inoculación/coagulación; E11: acidificación; E13: hilado y crema; E14: enfriamiento; E16: termoformado; E18–E22: salida. |
| Q3 | E07: inoculación/coagulación/cocción; E12: acidificación; E13: hilado; E15: agua/salmuera; E17: vacío/encogimiento; E18–E22: salida. |

### 6.3 Recetas y formulación de diseño

Las recetas maestras son **RM-Q1-v3, RM-Q2-v3 y RM-Q3-v3**. La receta de control vincula la versión aprobada con orden, lote, cantidad, equipos y partidas de ingredientes.

Los cultivos se expresan como **cultivo líquido de trabajo**, no como concentrado DVS. El ejemplo de cuajo considera **200 IMCU/mL** y una dosis de diseño de **50 IMCU/L**. Los valores constituyen la base de formulación del proyecto, no una dosis universal para cualquier insumo.

| Ingrediente Q1 | Por 100 L de leche | Lote de 4.500 L |
|---|---:|---:|
| Leche pasteurizada, grasa 2,6 % | 100 L | 4.500 L |
| Cultivo mesófilo de trabajo | 0,50 L | 22,50 L |
| CaCl₂ equivalente | 15 g | 675 g |
| Cuajo, 200 IMCU/mL | 25 mL | 1.125 mL |
| Agua de lavado | 3 L | 135 L |
| Sal sobre cuajada escurrida | 1,5 kg/100 kg de cuajada | 0,015 × masa de cuajada |

| Ingrediente Q2 | Por 100 L de leche | Lote de 3.000 L |
|---|---:|---:|
| Leche entera pasteurizada, grasa 3,6 % | 100 L | 3.000 L |
| Cultivo mesófilo de trabajo, dosis de diseño | 0,50 L | 15 L |
| Cuajo, 200 IMCU/mL | 25 mL | 750 mL |
| Crema pasteurizada, grasa de diseño 40 % | 1 kg | 30 kg |
| Sal sobre cuajada escurrida | 1,5 kg/100 kg de cuajada | 0,015 × masa de cuajada |

| Ingrediente o recurso Q3 | Por 100 L de leche | Lote de 1.500 L |
|---|---:|---:|
| Leche pasteurizada, grasa 2,6 % | 100 L | 1.500 L |
| Cultivo termófilo de trabajo | 1 L | 15 L |
| CaCl₂ equivalente | 10 g | 150 g |
| Cuajo, 200 IMCU/mL | 25 mL | 375 mL |
| Medio de hilado | Agua apta a 75–80 °C | Según carga y equipo |
| Salmuera, concentración de diseño 20 % m/m | 20 kg de sal + 80 kg de agua | Recurso de proceso, no incorporación total al queso |

La asignación de leche indica la carga base; los ingredientes adicionales se contabilizan aparte. La autorización de carga considera capacidad útil, ingredientes y margen de operación. Los balances usan masa y densidad medida para conciliar queso, suero, efluentes y mermas.

### 6.4 Condiciones de proceso

| Receta | Elaboración | Operación diferenciadora | Acondicionamiento |
|---|---|---|---|
| Q1 | Leche 34–35 °C; coagulación 30–40 min; corte 1,5–2 cm. | Lavado, salado, moldeo y prensa 30–60 min; referencia 45 min. | Oreo 4–6 °C, 2–4 h, hasta centro menor de 10 °C; E16. |
| Q2 | Leche 32–34 °C; cultivo hasta acidez 0,20–0,22 %; coagulación 30–40 min. | Acidificación E11 hasta pH 5,1–5,3; referencia 2,5 h; hilado 75–80 °C, crema y sal. | Enfriamiento E14 a 4–6 °C; referencia 6 h; E16. |
| Q3 | Leche 35–37 °C; cultivo termófilo; cocción hasta 38–40 °C. | Acidificación E12 hasta pH 5,1–5,3; referencia 3,5 h; hilado 75–80 °C. | Agua 4–8 °C, 1 h; salmuera 18–20 %, 6–8 h; E17. |

La pasteurización E04 considera 72–75 °C durante 15–20 s. El control supervisa temperatura, caudal y retención. El producto terminado se almacena en E21 a 2–4 °C.

Los tiempos son referencias de programación. El corte exige firmeza confirmada; el hilado exige pH medido y prueba de elasticidad satisfactoria. La temperatura del agua y la de la masa se registran como variables distintas.

### 6.5 Fases, permisos e interbloqueos

| Fase | Condición de inicio | Fin de fase | Respuesta ante fallo |
|---|---|---|---|
| Verificar | Orden y receta autorizadas. | Unidad disponible, limpia y sin CIP activo. | Bloquear inicio si faltan permisos. |
| Cargar | Ruta correcta y capacidad disponible. | Volumen programado alcanzado; bomba detenida y válvula cerrada. | Detener por nivel alto, medición inválida o falta de caudal. |
| Ajustar temperatura | Producto cargado y sensor válido. | Temperatura dentro del intervalo autorizado. | Retener por sensor inválido o sobretemperatura. |
| Dosificar | Temperatura permitida e ingredientes identificados. | Cantidad registrada y adición confirmada. | Bloquear avance sin confirmación. |
| Coagular/cortar | Cuajo registrado y agitación detenida. | Firmeza confirmada antes del corte. | Mantener espera y registrar decisión autorizada. |
| Acidificar/hilar | Cultivo identificado; recurso de hilado reservado. | Acidez/pH de receta y elasticidad aprobados. | Retener ante muestra inválida o condición no satisfactoria. |
| Empacar/liberar | Producto identificado y acondicionado. | Peso, sello y calidad registrados. | Rechazar o retener producto y registrar motivo. |

```mermaid
flowchart TD
    INI["Solicitud de carga Q1"] --> PER{"¿Tina limpia, disponible<br/>y ruta autorizada?"}
    PER -->|No| BLO["Bloquear inicio y registrar motivo"]
    PER -->|Sí| ACT["Abrir XV-301 y arrancar P-301"]
    ACT --> MED["Leer FT-301 y nivel LT/LSHH-301"]
    MED --> FAL{"¿Nivel alto o<br/>medición inválida?"}
    FAL -->|Sí| STOP["Detener bomba, cerrar válvula<br/>y generar alarma"]
    FAL -->|No| VOL{"¿Total alcanzado<br/>4.500 L?"}
    VOL -->|No| MED
    VOL -->|Sí| FIN["Detener bomba y cerrar válvula<br/>Registrar volumen y fin de fase"]
```

Las confirmaciones manuales, incluida firmeza y prueba de elasticidad, identifican operador, hora y lote. Grafcet, Ladder y las pruebas funcionales desarrollan esta especificación en los módulos de control y gemelo digital.

## 7. Instrumentación propuesta

| Señal o elemento | Función | Decisión asociada |
|---|---|---|
| FT-301 | Totalizar leche cargada en TQ-301. | Finalizar carga al volumen de receta. |
| LT/LSHH-301 | Medir nivel y detectar nivel alto. | Proteger contra sobrellenado. |
| TT-301 | Medir temperatura de tina. | Regular camisa y autorizar fases térmicas. |
| P-301 / XV-301 | Bombear y habilitar entrada. | Ejecutar o detener carga. |
| M-301 | Agitar y cortar. | Seleccionar modo y detener durante coagulación. |
| BAL-01 | Pesar ingredientes y cuajada. | Verificar dosis y calcular sal. |
| pH-M01 | Medición de muestra con equipo calibrado. | Autorizar hilado según pH y elasticidad. |
| Temperatura de E13 | Registrar agua y masa. | Supervisar hilado. |
| Temperatura y concentración de E15 | Supervisar agua fría y salmuera. | Controlar acondicionamiento Q3. |
| Inspección E18 | Peso, codificación y metales. | Rechazo y trazabilidad de empaque. |

Los identificadores de tina se replican para TQ-302 y TQ-303. Cada señal especifica origen físico, entrada manual o variable simulada. Los interbloqueos locales del PLC se conservan ante pérdida de comunicación con gestión.

## 8. Arquitectura de integración ISA-95

```mermaid
flowchart TD
    ERP["Nivel 4 · ERP<br/>Órdenes, materiales y planificación"]
    MES["Nivel 3 · Funciones MES<br/>Lotes, reservas, consumos y calidad"]
    SCADA["Nivel 2 · Ignition<br/>Supervisión, recetas, alarmas y tendencias"]
    PLC["Nivel 1 · PLC / Logix Emulate<br/>Fases, control y adquisición de señales"]
    PRO["Nivel 0 · Proceso<br/>Leche, cuajada, equipos y producto"]
    ERP -->|Órdenes y requerimientos| MES
    MES -->|Producción y consumos| ERP
    MES -->|Lote y receta autorizados| SCADA
    SCADA -->|Eventos y resultados| MES
    SCADA -->|Solicitud de ejecución y parámetros| PLC
    PLC -->|Aceptación, estados y mediciones| SCADA
    PLC -->|Actuación| PRO
    PRO -->|Mediciones| PLC
    classDef nivel fill:#e7f1fb,stroke:#1b609e,color:#08223f;
    class ERP,MES,SCADA,PLC,PRO nivel;
```

Los niveles indican responsabilidades funcionales. El PLC ejecuta control y secuencias; Ignition constituye la supervisión prevista para el módulo SCADA. Las funciones MES se representan mediante registros estructurados y gestión de lotes; SAP es una referencia conceptual de ERP.

### Interfaces y responsabilidades

| Interfaz | Información | Solución propuesta |
|---|---|---|
| PLC–Ignition | Variables, estados, permisos, comandos y confirmaciones. | Servidor OPC compatible con el controlador; interfaz OPC UA hacia supervisión. |
| Ignition–registro MES | Eventos, consumos, cantidades, paradas y resultados. | Base de datos SQL con identificadores comunes. |
| Gestión–integración | Órdenes y reportes de producción. | API mediante Node-RED. |
| Calidad–gestión | Muestra, ensayo, resultado y liberación/retención. | Registro identificado por lote y responsable. |

Node-RED apoya el intercambio de información. Ignition es el punto de despacho al control; el PLC mantiene la ejecución y los interbloqueos. La arquitectura describe la propuesta, sin afirmar una conexión funcional ya demostrada.

### Recorrido de una orden

```mermaid
sequenceDiagram
    participant ERP as ERP
    participant MES as Funciones MES
    participant I as Ignition
    participant P as PLC
    participant Q as Calidad
    ERP->>MES: OP-Q1-001, producto y cantidad
    MES->>MES: B-Q1-001, RM-Q1-v3, TQ-301 y reservas
    MES->>I: Despachar lote y parámetros autorizados
    I->>P: Solicitud de ejecución identificada
    P-->>I: Aceptación o rechazo con motivo
    loop Ejecución autorizada del lote
        P-->>I: Fase, estado, mediciones y alarmas
        I->>MES: Eventos, cantidades y confirmaciones
    end
    MES->>Q: Solicitar evaluación de lote
    Q-->>MES: Liberación o retención y resultados
    MES-->>ERP: Consumos, producción, rechazo y estado de calidad
```

Ejemplo de registro de planificación:

```json
{
  "order_id": "OP-Q1-001",
  "batch_id": "B-Q1-001",
  "product_id": "Q1",
  "recipe_id": "RM-Q1-v3",
  "unit_id": "TQ-301",
  "station_id": "E05",
  "planned_milk_quantity": 4500,
  "quantity_unit": "L"
}
```

Este esquema identifica un ejemplo de orden; no corresponde a una API específica de SAP ni a datos de fabricación real.

### Datos mínimos por lote

| Objeto | Campos principales |
|---|---|
| Orden | Identificador, producto, cantidad/unidad, prioridad y fecha requerida. |
| Receta de control | Versión maestra, lote, equipos, cantidades y partidas asignadas. |
| Evento de fase | Lote, equipo, fase, inicio/fin, valor/unidad y calidad de medición. |
| Consumo | Material, partida, cantidad real, unidad, fase y responsable. |
| Calidad | Muestra, ensayo, resultado, criterio, estado, responsable y hora. |
| Cierre | Producción real, empaque, suero, rechazos, mermas, duración y estado de calidad. |

## 9. Trazabilidad e integridad de la información

```mermaid
flowchart LR
    L["Partidas de leche"] --> B["B-Q1-001<br/>RM-Q1-v3 · TQ-301"]
    A["Partidas de cultivo,<br/>calcio, cuajo y sal"] --> B
    B --> P1["Partida de empaque 1"]
    B --> P2["Partida de empaque 2"]
    B --> S["Suero: cantidad,<br/>origen y destino"]
    P1 --> C["Calidad y estado de liberación"]
    P2 --> C
    C --> D["Producto disponible<br/>para despacho si está liberado"]
```

- Las divisiones y mezclas de lotes conservan sus vínculos de origen.
- Cada mensaje lleva identificador único, fecha/hora, origen, lote y versión de esquema.
- Los reintentos evitan duplicar consumos o ejecutar nuevamente una fase.
- Los comandos distinguen solicitud, aceptación, ejecución y finalización.
- La propuesta conserva registros localmente durante desconexión y sincroniza al recuperar el enlace.
- Los permisos distinguen operación, aprobación de recetas, calidad, mantenimiento y programación.

## 10. Articulación con los módulos del proyecto

| Módulo | Relación con el diseño TDI |
|---|---|
| Gestión y evaluación de producción | VSM, capacidades, tiempos y programación con las mismas estaciones y lotes. |
| Controladores industriales | Grafcet y Ladder para las fases, parámetros y permisos definidos. |
| Digital Factory | Gemelo digital detallado de quesos, sensores y actuadores virtuales, ejecución de recetas. |
| SCADA | Ignition, operación y supervisión, alarmas, tendencias y comunicación OPC. |
| Celda robotizada | Paletizado previsto en E20, flujo de cajas y coordinación con producción. |
| Planeación y evaluación de proyectos | Equipos y recursos de la propuesta como base de cronograma y evaluación económica. |

# 11. Simulación de la planta en Tecnomatix Plant Simulation

A continuación se presenta el documento con la estructura de VSM que se tomó como base para la realización de la simulación [Ver Documentación y estructura de vsm](VSM/EDT_proceso_productivo%20(4)-2.pdf)
## 11.1. Objetivo y alcance de la simulación

La simulación de la planta de Lácteos Fúquene S.A.S. se desarrolló en Siemens Tecnomatix Plant Simulation, con el propósito de representar el flujo de materiales, evaluar la utilización de los recursos productivos e identificar posibles restricciones que afecten la continuidad de las operaciones.

El modelo integra las principales estaciones, equipos de procesamiento, tuberías, transportadores, buffers y recursos compartidos definidos para las líneas de queso campesino, queso doble crema y mozzarella. La simulación permite observar los estados operativos de los recursos y analizar cómo la disponibilidad de materia prima, las condiciones de transferencia entre estaciones y la planificación de la producción influyen en el comportamiento del sistema.

El análisis se complementa con la librería BottleneckAnalyzer, utilizada para examinar la distribución temporal de los estados de los recursos e identificar estaciones con altos porcentajes de espera, bloqueo o interrupción.

Los objetivos específicos son:

- Analizar la continuidad del flujo de materiales entre estaciones.
- Identificar recursos con tiempos elevados de espera o bloqueo.
- Examinar las restricciones derivadas de la disponibilidad de materia prima y de la programación de la producción.
- Estimar indicadores de disponibilidad, rendimiento, calidad y OEE para las estaciones seleccionadas.
- Proponer oportunidades de mejora en la coordinación entre equipos y en la planificación de los procesos.

Alcance: los resultados corresponden al comportamiento del modelo bajo los parámetros, tiempos y condiciones de operación configurados. Por tanto, constituyen resultados de simulación y no mediciones directas de una planta industrial en funcionamiento.

## 11.2. Modelado del flujo de producción

El modelo representa el desplazamiento de la materia prima y de las unidades de producción entre los recursos definidos para las líneas de queso. Las estaciones se conectan mediante objetos de transporte y transferencia, mientras que los equipos de procesamiento representan las operaciones correspondientes a cada producto.

Se consideran tres líneas principales:

| Línea | Producto | Producción diaria de referencia |
|---|---|---:|
| Q1 | Queso campesino | 4.500 L/día |
| Q2 | Queso doble crema | 3.000 L/día |
| Q3 | Mozzarella | 1.500 L/día |
| Total | Procesamiento de leche destinado a las tres líneas | 9.000 L/día |

Los volúmenes de la tabla corresponden a la asignación de leche definida para el escenario de producción del proyecto. No representan necesariamente el volumen de producto terminado, puesto que el rendimiento depende de la formulación, la humedad, el desuerado y las características de cada queso.

El modelo incorpora equipos compartidos entre líneas, como los recursos de hilado, moldeo, termoformado y paletizado, cuando corresponde a la configuración definida. Estos recursos requieren especial atención porque pueden introducir dependencias entre las secuencias de producción y limitar la capacidad de procesamiento si varias líneas los requieren simultáneamente.

![Figura 11.1. Representación general del sistema productivo](Imagenes/simulacionGeneral.png)

*Figura 11.1. Representación general del sistema productivo y de las conexiones entre recursos.*

![Figura 11.1. Representación general del sistema productivo](Imagenes/LineasQ123.png)

*Figura 11.2. Flujo de materiales y equipos compartidos entre las líneas de producción.*

## 11.3. Condiciones de operación y supuestos de simulación

La evaluación se realiza bajo las condiciones temporales y de suministro configuradas en el modelo. Para interpretar correctamente los resultados, se diferencia entre el horizonte total de simulación, el tiempo programado para producir y los periodos en los que la operación no está prevista.

La disponibilidad de materia prima no se considera necesariamente continua durante todo el horizonte. En particular, para la línea Q3 se contempla una ventana efectiva de producción determinada por la planificación de turnos, la asignación diaria de leche y la demanda del producto.

Los siguientes criterios se utilizan para interpretar los resultados:

| Parámetro | Criterio adoptado |
|---|---|
| Horizonte de simulación | Periodo total configurado en Tecnomatix Plant Simulation |
| Programación de turnos | Determina los intervalos en los que se requiere producción |
| Disponibilidad de materia prima | Depende de la asignación y del suministro definidos para cada línea |
| Demanda de producción | Determina la cantidad de producto que se necesita fabricar |
| Calidad | Se adopta un valor del 97 % como supuesto de modelado para el cálculo ilustrativo del OEE |
| Análisis de estados | Se utiliza BottleneckAnalyzer para evaluar la distribución temporal de los estados de los recursos |

El porcentaje del 97 % de calidad es un supuesto y no una medición de producto conforme obtenida de la simulación. Para calcular un OEE industrial validado, este valor deberá sustituirse por la proporción real o simulada de unidades conformes respecto del total producido.

## 11.4. Análisis de estados mediante BottleneckAnalyzer

La librería BottleneckAnalyzer permite examinar el porcentaje de tiempo que cada recurso permanece en los diferentes estados registrados durante la simulación. Esta información facilita la identificación de estaciones que trabajan durante una parte reducida del horizonte, permanecen esperando material o se encuentran bloqueadas por restricciones en el flujo.

Los principales estados considerados son:

| Estado | Interpretación |
|---|---|
| `Working` | El recurso ejecuta su operación productiva. |
| `Set-up` | El recurso realiza actividades de preparación o cambio de configuración. |
| `Waiting` | El recurso permanece esperando una entidad, material, condición o evento necesario para continuar. |
| `Blocked` | El recurso no puede transferir o liberar el material debido a una restricción aguas abajo o a una condición de salida. |
| `PoweringUpDown` | El recurso está en una transición de encendido o apagado. |
| `Disrupted` | El recurso se encuentra en un estado de interrupción definido por el modelo. |
| `Stopped` | El recurso está detenido según la lógica configurada. |
| `Pause` | El recurso se encuentra en un periodo de pausa definido en el modelo. |

La interpretación de estos estados depende de la lógica implementada en cada objeto. Por ejemplo, `Waiting` no representa necesariamente una falla ni una pérdida de eficiencia: puede corresponder a una espera normal por disponibilidad de materia prima o a una operación que todavía no necesita ejecutarse.

![Figura 11.1. Estadísticas de cada máquina](Imagenes/estadisticasRecursos.png)

*Figura 11.2. Estadísticas de cada máquina.*

### 11.4.1. Interpretación de las restricciones

#### a. Bloqueo en `DePortioner11`

El recurso presenta un 80,86 % de tiempo de trabajo y un 19,14 % de tiempo bloqueado. Este comportamiento indica que, durante una parte del horizonte, el equipo no puede continuar con normalidad debido a una restricción de salida o a la lógica de transferencia configurada.

Para determinar si el bloqueo está relacionado con la capacidad de la estación siguiente, el espacio disponible en un buffer o una condición de transferencia, es necesario revisar la conexión entre los objetos y los eventos ocurridos durante esos intervalos.

#### b. Espera en `TinaQuesoCampesino`

La tina registra un 80,86 % de espera y un 19,14 % de interrupción, sin tiempo de trabajo en la salida analizada. Este resultado indica que el recurso no está ejecutando la operación productiva durante el horizonte observado.

El patrón podría estar relacionado con la disponibilidad de entidades de entrada, la programación de la operación o las condiciones de activación del equipo. Sin embargo, el resultado no permite atribuir por sí solo la espera a una causa física específica. Se debe verificar si la tina recibe material, si los tiempos de proceso están correctamente configurados y si la lógica de inicio e interrupción corresponde a la secuencia productiva prevista.




## 11.5. Cálculo e interpretación del OEE

El indicador OEE (*Overall Equipment Effectiveness*) permite evaluar el desempeño de un equipo a partir de tres componentes: disponibilidad, rendimiento y calidad.

La expresión general es:

\[
OEE = D \times R \times C
\]

donde:

- \(D\): disponibilidad.
- \(R\): rendimiento.
- \(C\): calidad.

Para el análisis presentado se utilizan las siguientes expresiones:

\[
D = \frac{T_p-T_d}{T_p}\times100
\]

\[
R = \frac{T_w}{T_p-T_d}\times100
\]

donde:

- \(T_p\): tiempo programado de producción.
- \(T_d\): tiempo en estado `Disrupted` dentro de la ventana programada.
- \(T_w\): tiempo en estado `Working` dentro de la ventana programada.

Para combinar los tres componentes en la expresión del OEE, los porcentajes se convierten a valores entre 0 y 1. En esta estimación, el rendimiento se aproxima mediante la fracción de tiempo en estado `Working` respecto del tiempo programado disponible después de descontar `Disrupted`. Este procedimiento es una aproximación basada en estados del modelo; no sustituye el cálculo convencional del rendimiento a partir del tiempo de ciclo ideal y las unidades producidas.

### 11.5.1. Resultados de referencia para las moldeadoras

Los resultados previamente obtenidos para las moldeadoras son los siguientes:

| Indicador | Q1: MoldeadoraQ1 | Q2: MoldeadoraQ2 | Q3: MoldeadoraQ3 |
|---|---:|---:|---:|
| Tiempo programado utilizado, \(T_p\) | 43,75 % | 43,75 % | 14,00 % |
| Disponibilidad, \(D\) | 97,53 % | 93,76 % | 80,86 % |
| Rendimiento estimado, \(R\) | 70,82 % | 78,60 % | 74,73 % |
| Calidad asumida, \(C\) | 97,00 % | 97,00 % | 97,00 % |
| OEE estimado | 67,00 % | 71,49 % | 58,62 % |

*Nota: estos resultados provienen del análisis previo de las moldeadoras y utilizan ventanas de tiempo programado específicas. Deben conservarse únicamente si corresponden a la misma configuración, ejecución y definición de estados de la simulación. La tabla de BottleneckAnalyzer presentada en la sección 11.4 muestra una distribución diferente para `MoldeadoraQ1`, `MoldeadoraQ2` y `MoldeadoraQ3` (100 % en espera), por lo que es necesario verificar que ambas salidas correspondan a la misma corrida y al mismo intervalo antes de presentarlas como resultados directamente comparables.*

### 11.5.2. Justificación del tiempo programado de Q3

Para la línea Q3, correspondiente a mozzarella, se adoptó un tiempo programado de producción equivalente al 14 % del horizonte total de simulación.

Este valor se definió a partir del análisis del comportamiento de los recursos mediante la librería BottleneckAnalyzer y de la planificación operativa establecida para el escenario. En particular, se consideraron los turnos de producción, la asignación diaria de materia prima, el carácter no continuo del suministro de leche y la cantidad de mozzarella requerida de acuerdo con la demanda.

A diferencia de un escenario de abastecimiento continuo, la línea Q3 no necesita permanecer produciendo durante todo el horizonte de simulación. Su operación se concentra en una ventana durante la cual existe materia prima disponible para fabricar la cantidad planificada. Una vez satisfecha la necesidad de producción o agotada la asignación de leche destinada a la línea, la operación se detiene porque no se requiere continuar procesando material durante el resto del periodo analizado.

Por esta razón, el tiempo restante se considera fuera del tiempo programado de producción únicamente bajo el supuesto de que la línea no tenía obligación de producir durante esos intervalos. Esta decisión evita contabilizar como pérdida operativa el tiempo en el que la producción no está planificada debido a la demanda y al esquema de suministro definido.

El 14 % constituye, por tanto, un criterio de planificación del modelo sustentado en el análisis de estados y en las condiciones de suministro y demanda, y no una medición directa del tiempo de operación. Para documentar adecuadamente esta decisión, se recomienda conservar como evidencia la salida de BottleneckAnalyzer, la programación de turnos y la asignación de materia prima a Q3.

La distinción es importante: si la estación estuviera programada para producir y no pudiera hacerlo por falta de leche, esa situación debería evaluarse como una pérdida de disponibilidad. En cambio, si el periodo se encuentra formalmente fuera del programa de producción, no debe incorporarse al denominador del OEE.

### 11.5.3. Interpretación comparativa

De acuerdo con los resultados de referencia de la sección 11.5.1, Q2 presenta el OEE estimado más alto, con 71,49 %, seguida de Q1, con 67,00 %. Q3 registra 58,62 % cuando se evalúa exclusivamente dentro de la ventana programada del 14 % del horizonte.

Estas diferencias deben interpretarse teniendo en cuenta que Q3 utiliza un denominador temporal distinto. Por ello, el OEE de Q3 no debe compararse de forma aislada con los de Q1 y Q2 sin verificar que las ventanas programadas, los criterios de clasificación de estados y las condiciones de operación sean consistentes.

Además, el porcentaje de calidad del 97 % es un supuesto de cálculo. Para obtener un OEE más representativo, se deberán incorporar el tiempo de ciclo ideal, las cantidades producidas y las unidades conformes de cada línea.

## 11.6. Oportunidades de mejora identificadas

A partir de los resultados de estados y del cálculo de indicadores, se proponen las siguientes acciones:

| Hallazgo | Acción recomendada | Objetivo |
|---|---|---|
| Bloqueo de `DePortioner11` | Revisar la capacidad de salida, las conexiones y las condiciones de transferencia. | Reducir bloqueos y mejorar la continuidad del flujo. |
| Espera elevada en `TinaQuesoCampesino` | Verificar las llegadas de material, los tiempos de proceso y la lógica de activación. | Determinar si la espera es normal o se debe a una restricción del modelo. |
| Baja utilización de `Track` | Revisar el ritmo de llegada de entidades y la sincronización con los recursos conectados. | Evitar esperas innecesarias y mejorar la coordinación del transporte. |
| Recursos con 100 % de espera o bloqueo | Comprobar la conectividad, las condiciones de liberación y la generación de entidades en cada línea. | Confirmar que todas las estaciones estén correctamente representadas. |
| Suministro no continuo de leche a Q3 | Alinear el tiempo programado con los turnos, la asignación de materia prima y la demanda. | Evaluar el desempeño dentro de la ventana real de producción prevista. |
| Calidad fijada en 97 % | Incorporar datos de unidades conformes y no conformes. | Obtener una estimación de calidad sustentada en datos del proceso. |
| Rendimiento calculado mediante estados | Incorporar el tiempo de ciclo ideal y la cantidad producida. | Aproximar el OEE al método convencional de cálculo. |

Estas acciones deben evaluarse mediante nuevas corridas de simulación y comparación de escenarios. No se considera suficiente aumentar la capacidad de un equipo únicamente porque registre una utilización elevada: también debe verificarse si la estación limita realmente la producción total del sistema.

## 11.7. Limitaciones del análisis

Los resultados están condicionados por los parámetros de entrada, la lógica de los objetos y el horizonte de simulación utilizado. Por ello, se reconocen las siguientes limitaciones:

1. Los estados de BottleneckAnalyzer describen la distribución temporal de los recursos, pero no identifican por sí solos la causa física de cada espera, bloqueo o interrupción.
2. Los recursos con 100 % de espera o bloqueo deben verificarse antes de interpretar sus resultados como evidencia de restricciones industriales.
3. El 14 % de tiempo programado para Q3 es un criterio adoptado para representar la ventana efectiva de producción del escenario; su trazabilidad depende de la planificación de turnos, la asignación de leche y la demanda.
4. La calidad del 97 % corresponde a un supuesto de modelado y no a un resultado medido de conformidad.
5. El rendimiento estimado a partir del estado `Working` es una aproximación temporal y no equivale necesariamente al rendimiento convencional calculado mediante el ciclo ideal.
6. Los resultados de OEE y BottleneckAnalyzer deben corresponder a la misma configuración y corrida de simulación, o sus diferencias deben explicarse expresamente.

# 12. Caso de estudio, producción y evaluación financiera

## 12.1. Documentos

| Documento | Contenido |
|---|---|
| [Documento del caso](Produccion%20y%20finanzas/Documento_del_caso.pdf) | Lácteos Fúquene (operación, estados financieros, hallazgos), entorno del sector, normas que condicionan el proyecto, IntegraMotion (constitución, normas, cómo y cuánto cobra), matriz de selección de la línea, alcance de la oferta y BOM. |
| [EDT del proceso productivo](Produccion%20y%20finanzas/EDT_proceso_productivo.pdf) | Desglose de las operaciones de las tres líneas, nivel de automatización actual y propuesto para la quesería, recursos y cuellos de botella. |
| [VSM de las líneas](Produccion%20y%20finanzas/VSM_lineas.pdf) | Mapas de flujo de valor del campesino, los hilados, el yogur y el UHT; recursos compartidos, OEE de los equipos de fin de línea e indicadores por familia. |
| [Modelo financiero de la quesería](Produccion%20y%20finanzas/Modelo_financiero_queseria.xlsx) | Supuestos, BOM del proyecto enlazado a la inversión, beneficios con su respaldo, flujo de caja de 2027 a 2037, crédito, escenarios, análisis de riesgo, compuertas con árbol de decisión, rentabilidad que exige el dueño (CAPM más primas por tamaño y riesgo propio), efecto en la empresa y costo de la ingeniería de IntegraMotion por capas, por contrato y por paquete de la EDT, y una hoja Resumen con los cuadros que se presentan. |
| [Propuesta económica](Produccion%20y%20finanzas/Propuesta_economica.pdf) | Oferta de IntegraMotion a Lácteos Fúquene: cifras clave y decisiones que se piden, alcance y contratos, propuesta de valor por medida, oportunidades con la condición que exige cada una y cómo se comprueba, tarifas por rol con el conocimiento que las respalda, composición del precio y precio por paquete de la EDT, forma de pago y control por valor ganado, presupuesto, flujo de caja, tablero de indicadores con la relación beneficio/costo, financiación y costo de capital, escenarios, decisión bajo riesgo y compuertas, sostenimiento y condiciones comerciales. |
| [Minuta del contrato](Produccion%20y%20finanzas/Minuta_contrato_IntegraMotion.pdf) | Minuta académica del contrato principal y sus dos otrosíes, con sus cuatro anexos: actividades, horas y criterios de aceptación medibles; tarifas por rol; cronograma, curva S e hitos de pago; y quién hace cada trabajo. Cada entregable se acepta solo contra su criterio, y las compuertas se miden con cifras. |
| [Medidas organizacionales y uso del MES](Produccion%20y%20finanzas/Medidas_organizacionales.pdf) | Hallazgos con causa organizacional, medidas escogidas con una matriz de criterios, roles, quién responde por cada función del MES, procedimientos, reuniones fijas, responsables de los datos, transición del personal, formación e indicadores del uso del MES. |
| [Casos de decisión en la pirámide](Produccion%20y%20finanzas/Casos_piramide.pdf) | Veintisiete situaciones de la quesería recorridas del PLC a la gerencia según ISA-95: ocho flujos normales y diecinueve excepciones; qué decide cada nivel, en qué plazo, qué dato entrega al siguiente y qué valor protege; mensajes entre niveles, frontera ERP–MES y lo que los casos le piden al ERP. |
| [P&ID de la planta y de la quesería](Produccion%20y%20finanzas/PID_planta_y_queseria.pdf) | Cuatro planos A3 según ANSI/ISA-5.1 (leyenda, planta completa y dos hojas de la quesería) con los tipos de proceso de cada unidad (continuo, por lote, discreto, inspección) y las transferencias ISA-88 entre unidades; memoria con unidades, transferencias, lazos, enclavamientos y lista de instrumentos. |
| [P&ID inteligente de las tinas en Plant 3D](Produccion%20y%20finanzas/PID_queseria_Plant3D.pdf) | Hoja P&ID-002 dibujada en AutoCAD Plant 3D con simbología PIP (ISA-5.1): tinas TQ-301/302/303, bombas, caudalímetros, válvulas de carga y de fondo e instrumentos con etiqueta en la base de datos del proyecto, de donde salen las listas de equipos, instrumentos y válvulas. |
| [VSM antes y después de la automatización](Produccion%20y%20finanzas/VSM_antes_y_despues.pdf) | Mapas de flujo de valor del campesino y de los hilados en el estado actual y en el estado futuro, con la misma demanda; tabla de indicadores antes y después (tiempos, carga del cuello de botella, OEE de la termoformadora, horas extra, operarios, sobrepeso y merma), capacidad que se libera y cómo se validan los valores proyectados. |

## 12.2. Oferta para la quesería

Al estudiar el mercado de la región encontramos la oportunidad que hace conveniente automatizar ahora: las cadenas de supermercados compran doble crema de marca propia, y Lácteos Fúquene puede ser su proveedor si da trazabilidad de cada lote, peso controlado, registros sanitarios digitales y entregas completas y a tiempo, que hoy la planta no puede dar. La automatización resuelve esas exigencias y, de paso, las pérdidas del diagnóstico.

Cada supuesto que no depende de la planta está escrito como una oportunidad que encontramos, con la condición que exige, por qué la empresa la cumple, cómo se comprueba y cuánto aporta al VPN (en millones):

| Oportunidad | Por qué Lácteos Fúquene la cumple | Aporte al VPN |
|---|---|---:|
| Contrato de marca propia con una cadena | Ya vende a cadenas; el MES, la controladora de peso y la hiladora cierran lo que la cadena exige | 152 |
| Crédito de fomento de Bancóldex | Es mediana empresa (Decreto 957 de 2019) con capacidad de pago | 68 |
| Prenda sobre los equipos en lugar del FNG | Tiene 6.500 millones en activos fijos y deuda de 0,8 veces el EBITDA | 100 |
| Crédito fiscal por innovación (art. 256-1) | El corte por coagulación, la grasa en línea y el MES son desarrollo nuevo | 243 |
| Venta del suero enfriado (opción, fuera de la oferta) | Deja 8.188 kg de suero al día, pero enfriarlo cuesta: a 45 $/kg resta 2 | −2 |

Al hacer la cuenta descubrimos que el suero, a 45 $/kg, no paga el enfriador ni su energía. Queda como opción: el enfriador se compra solo si un comprador firma a 49 $/kg o más, el precio que lo paga aun sin el descuento ambiental del art. 255.

La propuesta se ejecuta por etapas: diagnóstico de la planta y línea base (etapa 0); tinas instrumentadas, control de peso y metales, medición de grasa en línea y SCADA, historiador y MES ligero de la quesería (etapa 1); hiladora-moldeadora continua y CIP del circuito de quesos (etapa 2). Dos compuertas deciden con datos medidos si se compra la etapa 1 y la etapa 2. La celda robotizada de paletizado se diseña y se valida en RobotStudio, y su compra queda para una etapa 3.

IntegraMotion contrata el trabajo en tres partes. Lo que paga Lácteos Fúquene es el costo de ingeniería del proyecto, en millones de pesos de 2026 sin IVA:

| Contrato | Alcance | Valor |
|---|---|---:|
| Contrato principal (16 semanas del semestre 2026-2) | Los 19 paquetes de la EDT del proyecto (sección 3): diagnóstico de la etapa 0, diseño, programación y validación virtual de todo el proyecto, celda en RobotStudio, MES con estado de máquinas y OEE enlazado al ERP, configuración funcional del ERP, matriz de competencias del personal, balance de sólidos y costo por lote en el MES, modelo de mezcla óptima de los quesos y BOM cotizado | 224,1 |
| Otrosí 1 (marzo y abril de 2027) | Implementación de la etapa 1: montaje supervisado, puesta en marcha, capacitación y soporte | 65,0 |
| Otrosí 2 (2028) | Ingeniería de detalle e implementación de la etapa 2 | 87,7 |
| **Costo de ingeniería del proyecto** | | **376,8** |

Por fase, la ingeniería conceptual (diagnóstico, VSM, línea base, arquitectura y modelo financiero) es el 11 % del costo; la básica (recetas ISA-88, hojas de datos, especificación funcional, BOM y cotizaciones), el 13 %; la de detalle (programas, planos de lazo, interfaces, pruebas y gemelo), el 31 %; la implementación en planta, el 19 %, y la gestión del proyecto, el 15 %. El resto son viajes e instrumentos de prueba.

Cada otrosí se firma solo si se supera la compuerta anterior, y cada compuerta se mide con cifras. Si la primera no se supera, la empresa paga el contrato principal, cuya ingeniería ya recibió, no compra equipos y pierde unos 38 millones con los ahorros conservadores de la etapa 0; comprar la etapa 1 sin esa información costaría 296. Con un árbol de decisión y 70 % de probabilidad de superar cada compuerta, las compuertas bajan el peor resultado de −256 a −38 millones con un valor esperado parecido (470 frente a 500). Si la segunda no se supera, la etapa 1 vale 371 millones por sí sola, y un prepago de unos 22 millones en 2027 mantiene su cobertura de la deuda en 1,2. IntegraMotion hace la ingeniería, la integración y la gerencia, y no vende equipos ni hace montajes: la instalación eléctrica, hidráulica y mecánica, los planos de detalle de obra y de reubicación de equipos, el tablero, la parametrización del ERP y la calibración acreditada los hacen terceros que contrata Lácteos Fúquene, con su costo dentro de la inversión, e IntegraMotion los especifica y supervisa. La inversión en equipos sale del BOM del proyecto: 53 ítems con tag, tomados de la instrumentación de la sección 7, del modelo físico ISA-88 y de la arquitectura ISA-95 de la sección 8, cada uno con precio, origen, instalación, paquete de la EDT y madurez del precio.

La implementación va en 2027 y 2028 y el proyecto se evalúa hasta 2037. Cifras en millones de pesos constantes de 2026:

| Indicador | Valor |
|---|---:|
| Costo total del proyecto (con imprevistos) | 1.590,1 |
| Equipos del BOM que paga la quesería, sin imprevistos | 973,1 |
| Beneficio anual en régimen | 568,1 |
| Costos operativos nuevos al año | 76,5 |
| Costo de capital del proyecto (pesos corrientes) | 12,8 % |
| TIR del proyecto en pesos corrientes / constantes | 24,3 % / 19,2 % |
| VPN | 824 |
| Relación beneficio/costo | 1,46 |
| VPN sin el crédito fiscal por innovación | 581 |
| VPN sin el contrato de la cadena | 672 |
| Recuperación / descontada | 4,7 / 6,0 años |
| TIR del inversionista (65 % financiado, 7 años, 14,1 % E.A.) frente al 19,5 % que exige el dueño (CAPM más primas por tamaño y riesgo propio) | 42,1 % |
| Cobertura mínima del servicio de la deuda | 1,34 |

El valor de la oferta sale sobre todo de la operación y del MES, no de la financiación: sin el crédito fiscal el VPN sigue en 581 millones. El contrato de la cadena entra como un segundo lote diario de doble crema con leche comprada al acopio: deja poco por litro porque la leche se compra, y su riesgo es el plazo de pago de 60 días, por eso la oferta propone pronto pago a 30 días; sin el contrato el VPN es 672 millones. El MES resuelve la información en islas del diagnóstico (registra el estado de las máquinas, los paros y el OEE, también en los equipos antiguos, y publica la capacidad disponible en el ERP para que Ventas prometa con la capacidad real, y la orden de mantenimiento crea en el ERP la solicitud de compra del repuesto). Además, con una matriz de criterios se escogieron tres usos de sus datos: el balance de sólidos y humedad por lote (cuánto queso sale de cada litro), el costo real por lote y la mezcla óptima de los tres quesos por programación lineal, con los límites de un estudio de mercado de la región (más doble crema; poca mozzarella más, porque compite con la importada). La trazabilidad por lote queda como herramienta comercial para certificarse y entrar a cadenas exigentes. Cada hallazgo del diagnóstico de la quesería tiene su medida y su beneficio; las pérdidas de yogur y UHT que la oferta no resuelve (unos 529 millones al año a precio de venta) quedan como base de la ampliación a esas líneas. Nadie sale de la empresa. En la etapa 0, la matriz de competencias mostró un décimo hallazgo: los puestos se asignan por costumbre y a la planta le faltan dos que nadie cubre. Con la matriz y el método húngaro asignamos los dos operarios que libera la hiladora: uno al control nocturno de la incubación del yogur y otro al mantenimiento autónomo. El ERP es SAP Business One, que la empresa ya tiene: frente a Odoo, migrar costaría unos 160 millones y se pagaría en más de cinco años. Los beneficios pueden caer 38 % o la inversión subir 71 % antes de que el VPN llegue a cero. La inversión se financia con las líneas de Bancóldex para mipymes, con prenda sobre los equipos. Dentro de la oferta, IntegraMotion negocia la prenda con el banco y postula el proyecto ante Minciencias para el crédito fiscal (art. 256-1 del Estatuto Tributario). Toda empresa asume riesgos; la oferta decide antes cómo responder: el modelo tiene un plan de respuesta a los riesgos (señal, estrategia, responsable y recursos), una matriz que dice cómo se mide cada beneficio y qué no incluye, las condiciones de cada beneficio tributario y el control del contrato principal por valor ganado. Los escenarios y los supuestos están en el modelo financiero.

## 12.3. Decisiones a través de la pirámide

Veintisiete situaciones de la quesería recorridas del PLC a la gerencia: ocho flujos normales, uno por cada actividad de gestión de operaciones de ISA-95 (parte 3), y diecinueve excepciones ordenadas por su origen. La regla es la misma en todas: **cada nivel resuelve lo que puede en su plazo y sube solo el dato que el nivel de arriba necesita para decidir.** En los diagramas, las flechas son datos entre sistemas y las notas son decisiones de personas. Las tablas de pasos, los diecinueve mensajes entre niveles con su categoría y su verbo de ISA-95, y la frontera entre el ERP y el MES están en el documento [Casos de decisión en la pirámide](Produccion%20y%20finanzas/Casos_piramide.pdf).

| Nivel | Sistema | Quién decide | Qué decide | Plazo |
|---|---|---|---|---|
| N4 | ERP (SAP Business One) | Gerencia, Ventas, planeación, compras y costos | Qué se vende y se produce, qué se compra, cuánto cuesta y en qué se invierte | Días a meses |
| N3 | MES de la quesería (Ignition con PostgreSQL) | Jefe de quesería, calidad, técnico de mantenimiento | Qué lote va en qué tina y cuándo, qué se libera o se retiene, qué se repara primero | Minutos a un turno |
| N2 | SCADA (Ignition) e historiador | Quesero y operadores | Cómo responder a una alarma: seguir, pasar a manual o retener | Segundos a minutos |
| N1 | PLC-300 (CompactLogix) y controladores de los equipos | Nadie: decide la lógica programada | Parar en estado seguro, mantener los enclavamientos, no dejar avanzar una fase sin sus permisos | Milisegundos |
| N0 | Proceso: instrumentos y actuadores | -- | Medir y actuar | Continuo |

**Flujos normales**

<details>
<summary><b>F1. Alta de un producto y de su receta</b></summary>

**Qué lo dispara:** La cadena firma el contrato de marca propia: hay que crear el doble crema con su empaque y su etiqueta, sin tocar la receta de proceso. **Actividad de ISA-95:** Gestión de definiciones (producción y calidad).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  Note over ERP: Comercial y costos crean el producto de marca propia
  ERP->>MES: Definición del producto y su lista de materiales
  Note over MES: Procesos crea la receta y calidad la aprueba con su firma
  MES->>SC: Receta aprobada con su versión
  SC->>PLC: Parámetros al despachar un lote
  PLC->>SC: Aceptación o rechazo con motivo
  MES->>ERP: Receta vigente para costear
  Note over ERP: Costos fija el costo estándar, Ventas ya puede vender
```

</details>

<details>
<summary><b>F2. Asignación diaria del personal por competencias</b></summary>

**Qué lo dispara:** Antes de cada turno, el MES cruza quién llegó con los puestos que pide el programa del día. **Actividad de ISA-95:** Gestión de recursos (producción).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  ERP->>MES: Personal disponible y matriz de competencias
  MES->>MES: Asignación propuesta por el método húngaro
  Note over MES: Jefe de quesería confirma o ajusta la asignación
  MES->>SC: Usuarios y permisos por puesto
  SC->>MES: Quién operó cada lote y cuánto tiempo
  MES->>ERP: Horas por lote para nómina y costos
  Note over ERP: Gestión humana actualiza la matriz con la formación
```

</details>

<details>
<summary><b>F3. Programa del día desde las órdenes del ERP</b></summary>

**Qué lo dispara:** Cada tarde se arma el programa de la quesería para el día siguiente. **Actividad de ISA-95:** Programación detallada (producción).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  Note over ERP: Planeador crea las órdenes con pedidos, inventario y mezcla
  ERP->>MES: Órdenes de producción por queso y fecha
  MES->>MES: Secuencia de lotes con tiempos del VSM
  Note over MES: Jefe de quesería resuelve choques y aprueba
  MES->>ERP: Órdenes confirmadas y capacidad libre
  Note over ERP: Planeador mueve lo que no cabe, protegiendo la cadena
  MES->>SC: Despacho de cada lote a su hora
```

</details>

<details>
<summary><b>F4. Despacho, ejecución y reporte de un lote</b></summary>

**Qué lo dispara:** Llega la hora de un lote del programa aprobado. Es el recorrido normal de la sección 8 del README, aquí con las decisiones de cada nivel. **Actividad de ISA-95:** Despacho, gestión de la ejecución, recolección de datos y seguimiento (producción).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  MES->>SC: Lote B-Q1-001, RM-Q1-v3, TQ-301 y partidas reservadas
  Note over SC: Quesero revisa y confirma el inicio
  SC->>PLC: Solicitud de ejecución
  PLC->>PLC: Verifica permisos y ejecuta las fases
  PLC->>SC: Estados, mediciones y alarmas
  Note over SC: Quesero confirma firmeza y pH
  SC->>MES: Eventos, consumos y confirmaciones
  MES->>MES: Cierre del lote y rendimiento frente a Van Slyke
  MES->>ERP: Consumos y producción retenida
```

</details>

<details>
<summary><b>F5. Muestreo y liberación de un lote</b></summary>

**Qué lo dispara:** Se cierra un lote: el MES pide sus muestras según el plan de muestreo. **Actividad de ISA-95:** Gestión de la ejecución y seguimiento (calidad).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  MES->>MES: Solicitud de muestras al cerrar el lote
  Note over MES: Calidad toma muestras y registra resultados
  MES->>MES: Comparación con la especificación
  Note over MES: Jefe de calidad libera o retiene con motivo
  MES->>ERP: Lote liberado y certificado
  Note over ERP: Ventas despacha con el certificado
```

</details>

<details>
<summary><b>F6. Mantenimiento preventivo programado</b></summary>

**Qué lo dispara:** La bomba P-301 llega a 2.000 horas de operación y le toca el cambio de sellos. **Actividad de ISA-95:** Programación detallada, despacho y ejecución (mantenimiento).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  SC->>MES: Horas de marcha de la P-301
  MES->>MES: Orden preventiva con tareas y repuesto
  MES->>ERP: Reserva o solicitud del kit de sellos
  Note over MES: Jefe de quesería y técnico acuerdan la ventana
  MES->>SC: Equipo en mantenimiento
  SC->>PLC: Bloqueo del arranque
  Note over MES: Técnico ejecuta y cierra la orden
  MES->>ERP: Costo y horas de la orden
  Note over ERP: Mantenimiento ajusta el plan cada mes
```

</details>

<details>
<summary><b>F7. Recepción de la leche y despacho del producto</b></summary>

**Qué lo dispara:** Llega un carrotanque de la ruta de Carmen de Carupa; en la tarde se despacha un pedido de la cadena. **Actividad de ISA-95:** Gestión de la ejecución y seguimiento (inventarios).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  Note over MES: Recepción analiza el carrotanque y calidad lo acepta
  MES->>MES: Partida de leche con ruta y análisis
  MES->>ERP: Entrada de leche por partida
  Note over ERP: Pago al productor por calidad
  Note over ERP: Ventas factura el pedido de la cadena
  ERP->>MES: Pedido a despachar
  MES->>ERP: Lotes liberados que vencen primero
  Note over ERP: Bodega despacha con los lotes en la remisión
```

</details>

<details>
<summary><b>F8. Cierre del turno y cierre del mes</b></summary>

**Qué lo dispara:** Termina un turno; termina un mes. **Actividad de ISA-95:** Análisis de desempeño (producción, calidad, mantenimiento e inventarios).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  PLC->>SC: Estados de marcha, paro y falla
  SC->>MES: Contadores y paros con causa
  MES->>MES: OEE por máquina y turno
  Note over MES: Reunión diaria fija acciones por causa
  MES->>ERP: Producción y consumos del mes
  Note over ERP: Costos cierra el costo real por queso
  Note over ERP: Ventas y operaciones deciden la mezcla
  Note over ERP: Gerencia revisa beneficios contra la línea base
```

</details>

**Excepciones: equipos**

<details>
<summary><b>E1. Falla del variador de las liras durante el corte</b></summary>

**Qué lo dispara:** El variador SC-301 (PowerFlex 525) de las liras de la tina TQ-301 se dispara por sobrecorriente en plena fase de corte de un lote de campesino. **Actividad de ISA-95:** Gestión de la ejecución y de recursos (producción y mantenimiento).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  PLC->>PLC: Falla de SC-301, liras detenidas, fase Cortar en espera
  PLC->>SC: Estado de la fase y código de falla
  Note over SC: Quesero decide rearmar una vez o cortar a mano
  SC->>MES: Paro de TQ-301 y corte manual del lote
  MES->>MES: Orden de mantenimiento correctivo
  Note over MES: Técnico decide reparar o cambiar el variador
  Note over MES: Jefe de quesería decide mover o aplazar el siguiente lote
  MES->>ERP: Capacidad del día recalculada
  Note over ERP: Ventas decide cubrir con inventario o avisar al cliente hoy
  MES->>ERP: Solicitud para reponer el variador de reserva
  Note over ERP: Gerencia, cada mes, decide reparar o reemplazar según las fallas
```

</details>

<details>
<summary><b>E2. Falla o deriva de un instrumento</b></summary>

**Qué lo dispara:** La sonda TT-301 de la tina entrega una señal fuera de rango (menos de 3,8 mA) mientras se calienta la leche. **Actividad de ISA-95:** Gestión de la ejecución (producción y mantenimiento).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  PLC->>PLC: TT-301 fuera de rango, fase retenida
  PLC->>SC: Medición inválida
  Note over SC: Quesero mide con referencia y sigue en manual o retiene
  SC->>MES: Lecturas manuales del lote
  MES->>MES: Lote marcado y orden correctiva
  Note over MES: Técnico cambia y verifica la RTD, calidad decide el lote
  MES->>ERP: Repuesto usado y costo de la orden
  Note over ERP: Mantenimiento ajusta el plan de calibración
```

</details>

<details>
<summary><b>E3. Falla de un servicio: el vapor</b></summary>

**Qué lo dispara:** La caldera se dispara y cae la presión de vapor mientras se pasteuriza y se calientan las tinas. **Actividad de ISA-95:** Gestión de la ejecución (producción y mantenimiento).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  PLC->>PLC: Desvío del pasteurizador y fases retenidas
  PLC->>SC: Alarmas en varios equipos
  SC->>SC: Agrupa con causa común vapor
  Note over SC: Operadores dejan los lotes en espera
  SC->>MES: Un solo paro con causa servicio
  Note over MES: Jefe de producción fija el orden de recuperación
  MES->>ERP: Lotes perdidos y capacidad reducida
  Note over ERP: Ventas reprograma, gerencia decide respaldo si se repite
```

</details>

**Excepciones: materiales**

<details>
<summary><b>E4. Falta de cuajo para un lote</b></summary>

**Qué lo dispara:** Al despachar el lote de mozzarella, el MES no puede reservar el cuajo: el inventario no alcanza para la dosis de la receta o la única partida disponible está vencida. **Actividad de ISA-95:** Gestión de recursos (inventarios).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  ERP->>MES: Inventario de cuajo por partida
  MES->>MES: Reserva de cuajo rechazada, lote no despachado
  PLC->>PLC: Dosificar no avanza sin ingredientes identificados
  Note over MES: Jefe de quesería decide partida alterna, otro orden o esperar
  Note over MES: Calidad autoriza la partida y ajusta la dosis en IMCU
  MES->>ERP: Solicitud de compra urgente
  Note over ERP: Compras compra y calidad libera en la recepción
  Note over ERP: Planeador y gerencia recalculan el punto de reorden
```

</details>

<details>
<summary><b>E5. Leche cruda rechazada en la recepción</b></summary>

**Qué lo dispara:** La prueba de antibióticos de un carrotanque de 4.000 L sale positiva. **Actividad de ISA-95:** Gestión de la ejecución (calidad e inventarios).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  Note over MES: Calidad rechaza el carrotanque con antibióticos
  MES->>MES: Leche disponible recalculada
  Note over MES: Jefe de producción reparte por compromisos y margen
  MES->>ERP: Rechazo por ruta y órdenes ajustadas
  Note over ERP: Acopio busca otra ruta, Ventas avisa a los clientes
  Note over ERP: Gerencia, plan de calidad con el proveedor
```

</details>

<details>
<summary><b>E6. Empaque defectuoso de un proveedor</b></summary>

**Qué lo dispara:** La termoformadora empieza a rechazar unidades por vacío insuficiente al cambiar a un rollo nuevo de película. **Actividad de ISA-95:** Recolección de datos y análisis de desempeño (calidad e inventarios).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  PLC->>SC: Rechazos por vacío insuficiente
  Note over SC: Operador cambia a un rollo de otra partida
  SC->>MES: Rechazos por hora
  MES->>MES: Rechazos ligados a la partida de película
  MES->>ERP: Partida bloqueada
  Note over MES: Calidad decide sobre lo ya empacado
  Note over ERP: Compras reclama con evidencia y compra al alterno
```

</details>

**Excepciones: proceso y calidad**

<details>
<summary><b>E7. Temperatura de pasteurización por debajo del límite</b></summary>

**Qué lo dispara:** La sonda del tubo de retención del pasteurizador (operación 1.4.1) baja de 72 °C mientras pasa la leche para los quesos. **Actividad de ISA-95:** Gestión de la ejecución y seguimiento (calidad).

```mermaid
sequenceDiagram
  participant PLC as N1 · Pasteurizador
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  PLC->>PLC: Retención bajo 72 °C, válvula de desvío al tanque de balance
  PLC->>SC: Temperatura y posición de la válvula
  Note over SC: Operador busca la causa y decide corregir o parar
  SC->>MES: Desviación del punto crítico con su duración
  MES->>MES: Partidas y lotes de esa ventana en revisión
  Note over MES: Calidad decide liberar o retener con el registro
  MES->>ERP: Lotes retenidos bloqueados
  Note over ERP: Ventas reprograma, merma con su causa
  Note over ERP: Gerencia, cada mes, decide la acción si se repite
```

</details>

<details>
<summary><b>E8. Lote con rendimiento fuera de la banda</b></summary>

**Qué lo dispara:** Al cerrar un lote de mozzarella, su rendimiento real queda por debajo de la banda que fijó la línea base frente al rendimiento teórico de Van Slyke. **Actividad de ISA-95:** Análisis de desempeño (producción y calidad).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  PLC->>SC: Leche cargada, temperaturas, corte y peso
  SC->>MES: Eventos de fase y confirmaciones
  MES->>MES: Rendimiento real frente a Van Slyke
  Note over MES: Jefe de quesería decide la corrección del siguiente lote
  Note over MES: Si se repite, procesos propone receta nueva y calidad aprueba
  MES->>SC: Receta RM-Q3-v4 para los lotes nuevos
  MES->>ERP: Producción, consumos y costo real del lote
  Note over ERP: Costos cierra el mes, la reunión mensual decide la mezcla
```

</details>

<details>
<summary><b>E9. Metal detectado en la estación E18</b></summary>

**Qué lo dispara:** El detector de metales de la E18 expulsa dos unidades de doble crema en diez minutos. **Actividad de ISA-95:** Gestión de la ejecución y seguimiento (calidad).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  PLC->>PLC: E18 expulsa y detiene la banda
  PLC->>SC: Detecciones de metal
  Note over SC: Operador guarda lo expulsado y verifica con patrones
  SC->>MES: Detecciones con hora y lote
  MES->>MES: Retiene desde la última verificación correcta
  Note over MES: Calidad y mantenimiento buscan la fuente
  MES->>ERP: Inventario bloqueado o destruido
```

</details>

<details>
<summary><b>E10. Unidades fuera de peso en la estación E18</b></summary>

**Qué lo dispara:** El peso promedio de las unidades de 500 g de campesino baja turno a turno y empiezan los rechazos por bajo peso. **Actividad de ISA-95:** Gestión de la ejecución y análisis de desempeño (calidad).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  PLC->>PLC: E18 pesa y expulsa bajo peso
  PLC->>SC: Pesos y rechazos
  SC->>SC: Tendencia del promedio
  Note over SC: Operador ajusta el corte y verifica con patrones
  SC->>MES: Peso y rechazos por lote
  Note over MES: Calidad verifica el contenido declarado
  MES->>ERP: Sobrepeso del mes
  Note over ERP: Costos mide el beneficio de H3
```

</details>

<details>
<summary><b>E11. Queja de un cliente o retiro de producto</b></summary>

**Qué lo dispara:** La cadena reporta un empaque de doble crema con un cuerpo extraño e informa el lote impreso. **Actividad de ISA-95:** Seguimiento y análisis de desempeño (calidad).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  Note over ERP: Servicio al cliente registra la queja con el lote
  ERP->>MES: Consulta de trazabilidad del lote
  MES->>ERP: Hacia atrás y hacia adelante en menos de 4 h
  Note over MES: Jefe de calidad define el alcance
  Note over ERP: Comité decide el retiro y avisa al INVIMA
  ERP->>MES: Bloqueo de los lotes afectados
  Note over MES: Causa raíz y acción correctiva
```

</details>

**Excepciones: personal**

<details>
<summary><b>E12. Falta el quesero de un turno</b></summary>

**Qué lo dispara:** El quesero del turno de la mañana avisa una incapacidad de tres días. **Actividad de ISA-95:** Gestión de recursos (producción).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  Note over ERP: Gestión humana registra la incapacidad
  ERP->>MES: Personal disponible
  MES->>MES: Reemplazos calificados según la matriz
  Note over MES: Jefe de quesería asigna el reemplazo
  MES->>SC: Permisos del puesto al reemplazo
  SC->>MES: Quién operó cada lote
  Note over ERP: Gestión humana forma un segundo quesero si se repite
```

</details>

**Excepciones: demanda**

<details>
<summary><b>E13. Pedido urgente de doble crema</b></summary>

**Qué lo dispara:** Una cadena pide 100 kg adicionales de doble crema para entregar dentro de dos días. **Actividad de ISA-95:** Programación detallada (producción e inventarios).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  Note over ERP: Ventas registra el pedido de 100 kg de doble crema
  MES->>ERP: Capacidad publicada de tinas e hiladora
  Note over ERP: Planeador mueve 375 L diarios del campesino al doble crema
  Note over ERP: Gerente comercial decide aceptar con su margen
  ERP->>MES: Órdenes de producción ajustadas
  Note over MES: Jefe de quesería despacha los lotes, calidad programa el muestreo
  MES->>SC: Lote TQ-302 de 3.375 L con RM-Q2
  SC->>PLC: Solicitud de ejecución
  PLC->>SC: Fases cumplidas
  SC->>MES: Eventos y cantidades
  MES->>ERP: Producción liberada
  Note over ERP: Ventas despacha y factura
```

</details>

<details>
<summary><b>E14. Cancelación de un pedido con producto que vence</b></summary>

**Qué lo dispara:** Un cliente mayorista cancela 200 kg de campesino, que vence en 15 a 20 días. **Actividad de ISA-95:** Programación detallada (inventarios y producción).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  Note over ERP: Ventas registra la cancelación
  ERP->>ERP: Campesino sin destino con su vencimiento
  Note over ERP: Planeador decide reasignar, vender con descuento o producir menos
  ERP->>MES: Órdenes ajustadas
  MES->>MES: Menos campesino, más doble crema dentro de límites
  Note over ERP: Comercial revisa la cláusula de cancelación
```

</details>

<details>
<summary><b>E15. Llega más o menos leche de la planeada</b></summary>

**Qué lo dispara:** Por las lluvias, el acopio del día llega con 1.500 L menos de lo planeado (o, en verano, con 2.000 L más). **Actividad de ISA-95:** Programación detallada (inventarios y producción).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  Note over MES: Recepción registra la leche real del día
  MES->>MES: Mezcla del día por programación lineal
  Note over MES: Jefe de producción y planeador aprueban el reparto
  MES->>ERP: Órdenes ajustadas a la leche real
  Note over ERP: Si sobra, se vende cruda antes de producir sin venta
  Note over ERP: Acopio y gerencia revisan la estacionalidad
```

</details>

**Excepciones: información**

<details>
<summary><b>E16. Caída del enlace con el MES y el ERP</b></summary>

**Qué lo dispara:** El servidor del MES (SRV-01) o la red entre la planta y el ERP dejan de responder durante el turno. **Actividad de ISA-95:** Recolección de datos (todas).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  Note over MES: Servidor o red fuera de servicio
  PLC->>PLC: Fases en curso terminan con enclavamientos locales
  PLC->>SC: Estados y mediciones
  SC->>SC: Historiador guarda en disco local
  Note over SC: Jefe de quesería decide terminar lotes y pasar a papel
  Note over ERP: Capacidad marcada sin actualizar, Ventas no promete
  Note over MES: Sistemas restablece el servicio
  SC->>MES: Eventos guardados, sin duplicados
  Note over MES: Papel cargado en 24 h, calidad libera esos lotes
  MES->>ERP: Consumos y producción pendientes
```

</details>

<details>
<summary><b>E17. Dato inconsistente entre el MES y el ERP</b></summary>

**Qué lo dispara:** El ERP rechaza un reporte de consumo de cultivo porque dejaría el inventario en negativo. **Actividad de ISA-95:** Recolección de datos y seguimiento (inventarios).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  MES->>ERP: Consumo de cultivo del lote
  ERP->>MES: Rechazo, inventario insuficiente
  MES->>MES: Mensaje guardado en error
  Note over MES: Usuario clave busca la causa
  Note over ERP: Bodega cuenta y registra la recepción faltante
  MES->>ERP: Reenvío con el mismo identificador
  Note over ERP: Costos revisa los errores del mes
```

</details>

<details>
<summary><b>E18. Acceso no autorizado a la red de planta</b></summary>

**Qué lo dispara:** El firewall FW-01 detecta un intento de conexión desde la red de oficinas al servidor del SCADA. **Actividad de ISA-95:** Gestión de recursos (sistemas) (todas).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  Note over MES: Firewall bloquea el acceso y avisa a sistemas
  Note over MES: Sistemas aísla la red de planta
  PLC->>PLC: Sigue con su lógica local
  PLC->>SC: Estados y mediciones dentro de la planta
  Note over SC: Jefe de quesería pasa al respaldo manual si hace falta
  Note over MES: Sistemas revisa, cambia claves y reconecta
  MES->>ERP: Datos pendientes al reconectar
  Note over ERP: Gerencia aprueba mejoras de seguridad
```

</details>

**Excepciones: seguridad**

<details>
<summary><b>E19. Paro de emergencia o accidente en el hilado</b></summary>

**Qué lo dispara:** Un operario se quema con agua del hilado y su compañero oprime el paro de emergencia de la hiladora. **Actividad de ISA-95:** Gestión de la ejecución (producción).

```mermaid
sequenceDiagram
  participant PLC as N1 · PLC
  participant SC as N2 · Ignition
  participant MES as N3 · MES
  participant ERP as N4 · ERP
  PLC->>PLC: Paro por el circuito de seguridad
  PLC->>SC: Evento de paro de emergencia
  Note over SC: Brigada atiende y asegura el área
  SC->>MES: Paro con causa seguridad
  Note over MES: Jefe de producción decide reanudar y el lote
  Note over MES: Seguridad y salud reporta e investiga
  MES->>ERP: Costo del paro y del accidente
  Note over ERP: Gerencia aprueba acciones correctivas
```

</details>

| Función de ISA-95 | ERP (nivel 4) | MES (nivel 3) | Casos |
|---|---|---|---|
| 1.0 Procesamiento de pedidos | Pedidos, contrato de la cadena, promesa con la capacidad publicada | Publica la capacidad disponible | F7, E13, E14 |
| 2.0 Programación de la producción | Plan semanal y órdenes por queso y fecha | Programa detallado del día por tina, hiladora y CIP | F3, E15 |
| 3.0 Control de la producción | -- | Despacho, ejecución, recetas con versión, paros y OEE, con el SCADA y el PLC | F1, F4, F8, E1, E2, E3 |
| 4.0 Control de materiales y energía | Inventario de insumos y punto de reorden | Reserva por lote, consumo real, partida de leche | F7, E4, E5, E17 |
| 5.0 Compras | Solicitud, aprobación por monto, orden de compra y recepción | Crea la solicitud desde la orden de mantenimiento o la reserva fallida | F6, E1, E4, E6 |
| 6.0 Aseguramiento de calidad | Especificación del producto, bloqueo de inventario, certificado al cliente | Muestreo, resultados, liberación y trazabilidad por lote | F5, E7, E8, E9, E10, E11 |
| 7.0 Inventario de producto | Disponible, vencimientos y despachos | Lotes liberados y salida de lo que vence primero | F7, E14 |
| 8.0 Costos | Costo real por lote y por queso, merma por causa | Consumos y horas reales de cada lote | F8, E8 |
| 9.0 Despachos | Remisión y factura con los lotes | -- | F7 |
| 10.0 Mantenimiento | Costo de repuestos y órdenes, tiempo medio entre fallas para la gerencia | Órdenes preventivas y correctivas, contador de horas, registro de fallas | F6, E1, E2, E3 |
| Ingeniería y desarrollo | Lista de materiales del producto | Receta maestra con su versión, aprobada por calidad | F1, E8 |
| Gestión humana (fuera del modelo) | Nómina, novedades y matriz de competencias | Asignación por puesto y horas por lote | F2, E12 |
