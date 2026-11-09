# Estado inicial de Lácteos Fúquene

Cómo está la empresa antes de las mejoras del proyecto: operación, finanzas, entorno, normas, flujo de valor de sus líneas, hallazgos del diagnóstico y la línea que se escogió para automatizar. Lácteos Fúquene es una empresa ficticia; sus cifras se construyeron con datos públicos de 2026.

## 1. La empresa
Lácteos Fúquene nació como una quesera familiar en Ubaté, la cuenca lechera del norte de Cundinamarca, y creció hasta procesar 25.000 litros de leche al día. Hace diez años montó una planta UHT con envasado aséptico en bolsa y después una línea de yogur. Compra la leche a unos 300 productores de las rutas de Ubaté, Carmen de Carupa, Susa, Simijaca y Fúquene. Vende en Cundinamarca, Boyacá y Bogotá a cadenas, tiendas, tiendas de descuento, colegios, pizzerías y casinos.

| Dato | Valor |
|---|---|
| Razón social | Lácteos Fúquene S.A.S. |
| Ubicación | Planta en Ubaté, Cundinamarca |
| Tamaño | Mediana empresa por ingresos de manufactura (Decreto 957 de 2019): ventas de \$30.457 M |
| Leche procesada | 25.000 L/día; 7.350.000 L/año en 294 días de operación |
| Jornada | Lunes a sábado, dos turnos; 42 horas semanales por trabajador desde el 15 de julio de 2026 |
| Personal | Unas 100 personas; nómina de \$300 M al mes, costo empresa |
| Líneas | Yogur, quesos y UHT, con tres referencias cada una |
| Sistemas | SAP Business One para facturación e inventario; producción y calidad en papel y Excel; la planta UHT tiene su propio PLC de fábrica, sin conexión con el resto |

## 2. Portafolio y producción
| Línea | Referencia | Leche (L/día) | Precio a distribuidor |
|---|---|---:|---:|
| Yogur | Y1 natural, vaso de 150 g | 1.400 | \$6.800/kg |
| | Y2 fresa, vaso de 150 g | 1.400 | \$7.100/kg |
| | Y3 mora, vaso de 150 g | 1.200 | \$7.100/kg |
| Quesos | Q1 campesino, 500 g | 4.500 | \$19.500/kg |
| | Q2 doble crema, 500 g | 3.000 | \$22.000/kg |
| | Q3 mozzarella, 2,5 kg | 1.500 | \$24.000/kg |
| UHT | L1 leche entera, bolsa de 1 L | 6.500 | \$3.100/L |
| | L2 deslactosada, bolsa de 1 L | 3.500 | \$3.600/L |
| | L3 bebida láctea de chocolate, 200 mL | 2.000 | \$5.250/L |
| Subproductos | Crema de leche al 40 % | | \$9.000/kg |
| | Suero a porcicultores | | \$30/kg |

Una sola recepción alimenta las nueve referencias. La descremadora deja cada leche con su grasa objetivo; la crema sobrante va al fundido del doble crema y el resto se vende. El yogur se incuba de noche y se llena en la mañana, los quesos se trabajan de día y la planta UHT corre en la mañana y queda libre en la tarde.

| Corriente | Cantidad al día |
|---|---:|
| Leche recibida | 25.000 L |
| Yogur | 4.785 kg (31.898 vasos) |
| Quesos | 1.095 kg |
| Leche UHT y bebida láctea | 11.609 L (9.627 bolsas y 9.908 porciones) |
| Crema vendida | 547 kg |
| Suero vendido | 8.188 kg |

## 3. Situación financiera (2026, \$ M)
| Rubro | \$ M/año | % de ventas |
|---|---:|---:|
| Ventas de UHT | 12.315 | |
| Ventas de quesos | 6.772 | |
| Ventas de yogur | 9.851 | |
| Crema y suero | 1.519 | |
| **Ventas totales** | **30.457** | **100 %** |
| Leche cruda | (14.553) | 47,8 % |
| Insumos y empaques | (5.168) | 17,0 % |
| Nómina | (3.600) | 11,8 % |
| Energía, agua, gas y químicos | (1.218) | 4,0 % |
| Mantenimiento | (457) | 1,5 % |
| Distribución y ventas | (2.437) | 8,0 % |
| Merma y devoluciones | (609) | 2,0 % |
| Otros gastos administrativos | (609) | 2,0 % |
| **EBITDA** | **1.806** | **5,9 %** |
| Depreciación | (600) | 2,0 % |
| Intereses | (252) | 0,8 % |
| Impuesto de renta | (334) | 1,1 % |
| **Utilidad neta** | **620** | **2,0 %** |

| Activos | \$ M | Pasivos y patrimonio | \$ M |
|---|---:|---|---:|
| Cuentas por cobrar | 2.503 | Cuentas por pagar (leche e insumos) | 1.206 |
| Inventarios | 800 | Impuestos por pagar | 334 |
| Caja y bancos | 1.000 | Deuda financiera | 1.400 |
| Activos fijos netos | 6.500 | Patrimonio | 7.864 |
| **Total** | **10.804** | **Total** | **10.804** |

El margen neto de 2,0 % es normal en la industria láctea colombiana: las medianas lácteas promediaron 1,6 % entre 2014 y 2019. Hay tres razones:
- **La leche no se compra más barata por volumen.** El precio al productor se paga por calidad (Resolución 017 de 2012).
- **La leche UHT es la mitad del volumen y deja poco por litro**, porque compite con las grandes marcas y con las marcas propias.
- **Los dueños trabajan en la empresa** y su salario está en la nómina.

Con este margen, una caída de 5,9 % en el precio promedio de venta deja el EBITDA en cero. Por eso un proyecto de automatización no debe salir de la caja de la empresa: conviene financiarlo con crédito de fomento a un plazo que acompase las cuotas con lo que él mismo produce.

## 4. El entorno
- **La leche define el negocio.** Es el 47,8 % de las ventas. El caso usa \$1.980 por litro puesto en planta.
- **El TLC con Estados Unidos.** Desde el 1 de enero de 2026, año 15 del acuerdo, la leche en polvo, los quesos, el yogur y los preparados lácteos de Estados Unidos entran a Colombia sin arancel y sin cupo. En 2025 Colombia importó 77.605 t de lácteos, el 53 % de Estados Unidos. En la otra dirección, el acuerdo le da al queso colombiano un cupo preferencial de 4.600 t al año.
- **Exposición de cada producto.**
  - La mozzarella para pizzerías está muy expuesta: compite con la importada.
  - La leche UHT, de forma indirecta, porque la leche en polvo puede reconstituirse.
  - El campesino y el doble crema, poco: son típicos, frescos y sin equivalente importado.
- **El mercado de quesos de la región.** Bogotá, Cundinamarca y Boyacá consumen entre 15.400 y 19.300 t de queso al año. Los hilados son cerca del 28 %. El consumo crece cerca de 4 % al año en volumen.
- **La jornada bajó a 42 horas** (Ley 2101 de 2021). Cubrir las mismas horas de operación exige relevos.
- **El dinero es caro, pero hay crédito de fomento.** Entre mayo y julio de 2026, el crédito ordinario a medianas empresas costó 15,7 % efectivo anual, y el de redescuento (Bancóldex, Finagro), 14,1 %.

## 5. Normas que condicionan el proyecto
| Tema | Norma | Cómo condiciona el proyecto |
|---|---|---|
| Inocuidad y buenas prácticas | Resolución 2674 de 2013 | Equipos de diseño sanitario; limpieza validada y registrada |
| Leche y derivados | Decreto 616 de 2006 | La pasteurización se registra y desvía el flujo si baja la temperatura |
| Pago de la leche | Resolución 017 de 2012 | El pago al productor se liquida por calidad |
| Esterilidad del UHT | NTC 4433 | Cada lote UHT espera hasta 10 días la prueba de esterilidad |
| Vertimientos | Resolución 631 de 2015 | El suero tiene una carga orgánica muy alta |
| Beneficios tributarios | Estatuto Tributario, arts. 255, 256-1 y 258-1 | Descuento ambiental, crédito fiscal por innovación e IVA de activos productivos |
| Garantías mobiliarias | Ley 1676 de 2013 | Los equipos financiados pueden darse en prenda |
| Jornada laboral | Ley 2101 de 2021 | 42 horas semanales |
| Despidos | Ley 50 de 1990, art. 67 | El proyecto no despide: capacita y reasigna |
| Seguridad y salud en el trabajo | Decreto 1072 de 2015; Resolución 0312 de 2019 | El hilado a 80 °C es el trabajo de mayor riesgo de la planta |

## 6. Cómo fluye el valor hoy
Las cuatro familias se mapearon con la EDT de la producción y el VSM del estado actual.

| Familia | Tiempo total | Proceso | Proceso / total | Cuello de botella |
|---|---:|---:|---:|---|
| Yogur | 4,5 días | 14,4 h | 13,3 % | Llenadora: 9,5 h en una ventana de 8 h |
| Queso campesino | 2,5 días | 11,3 h | 19,1 % | No hay; la termoformadora usa 7,9 de 10 h |
| Quesos hilados | 4,3 días | 16,6 h | 15,9 % | Hilado a mano: 8,4 h en una ventana de 7,4 h |
| UHT (L2) | 13,3 días | 7,2 h | 2,3 % | No hay; la planta trabaja 6,5 de 14 h |

| Recurso | Indicador | Valor |
|---|---|---:|
| Llenadora de yogur | OEE (0,70 × 0,82 × 0,97) | ≈ 56 % |
| Termoformadora (campesino y doble crema) | OEE (0,81 × 0,80 × 0,96) | ≈ 62 % |
| Hilado a mano (doble crema y mozzarella) | Carga sobre su ventana de 7,4 h | 114 % |
| Envasadoras asépticas UHT | Disponibilidad | ≈ 85 % |
| Tinas queseras | Rendimiento quesero y grasa en el suero | Sin registro |

En la termoformadora se pierden cada día unos 15 minutos en el arranque, 30 en el cambio de campesino a doble crema y 45 en fallas. El rendimiento de 0,80 viene de la carga manual de los alvéolos y de las microparadas de la lámina.

En las cuatro familias, la mayor parte del tiempo es espera. Parte la exige el producto (incubación, maduración, cuarentena) y parte depende de decisiones que hoy se toman por teléfono, a voz o con el criterio del operario.

## 7. Diagnóstico: los doce hallazgos
| | Hallazgo |
|---|---|
| H1 | La grasa se estandariza a mano: se dejan 0,08 puntos de más en cada referencia |
| H2 | El yogur se incuba de noche sin vigilancia: cerca del 2 % se sobreacidifica o se reprocesa |
| H3 | Se regala producto en el llenado: 2 % de más en los vasos de yogur y 1 % en las bolsas de UHT |
| H4 | El UHT pierde 1 % del volumen en las interfases de arranque y cambio |
| H5 | El hilado del doble crema y la mozzarella es manual, a 80 °C; es el cuello de botella de los quesos y el trabajo más riesgoso |
| H6 | Los registros críticos están en papel y no hay trazabilidad de lote a proveedor; la merma y las devoluciones suman 2 % de las ventas |
| H7 | La limpieza y el mantenimiento son manuales y correctivos |
| H8 | El suero se vende sin enfriar a \$30/kg |
| H9 | La información vive en islas: Ventas promete sin saber qué máquinas fallan, y el 1 % de los quesos sale tarde o incompleto |
| H10 | Los puestos se asignan por costumbre: nadie vigila de noche el yogur y falta un puesto de mantenimiento autónomo |
| H11 | No se sabe cuánto queso sale de cada litro, lote por lote |
| H12 | El costo y la mezcla de los quesos se deciden con promedios |

H1 a H9 salen del análisis de la planta. H10 a H12 los encontramos en la etapa 0, al levantar la matriz de competencias y los datos de cada lote.

## 8. La línea que se automatiza
| | Yogur | Quesos | UHT |
|---|---|---|---|
| Leche al día | 4.000 L | 9.000 L | 12.000 L |
| Ventas al año | \$9.851 M | \$6.772 M | \$12.315 M |
| Operaciones manuales | 11 de 18 (61 %) | 18 de 23 (78 %) | 8 de 18 (44 %) |
| Cuello de botella | Llenadora: 9,5 h en 8 h | Hilado a mano: 8,4 h en 7,4 h | No hay |
| Seguridad y ergonomía | Encajado manual | Amasado a mano a 80 °C; cajas de 10 kg | Estiba de paquetes de 6,3 kg |

| Criterio | Peso | Yogur | Quesos | UHT |
|---|---:|---:|---:|---:|
| Productos con rutas de proceso distintas | 25 % | 2 | 5 | 2 |
| Operaciones manuales hoy | 20 % | 4 | 5 | 2 |
| Cuello de botella que exige automatizar | 20 % | 3 | 5 | 1 |
| Beneficio económico directo | 15 % | 5 | 4 | 2 |
| Seguridad y ergonomía del trabajo | 10 % | 2 | 5 | 2 |
| Riqueza para la simulación (continuo, lote y discreto) | 10 % | 3 | 5 | 2 |
| **Puntaje ponderado** | | **3,15** | **4,85** | **1,80** |

La quesería gana aunque todos los criterios pesen lo mismo. Solo pierde en beneficio directo: el yogur tiene ahorros rápidos, pero son de control y de orden, y no tiene un cuello de botella que obligue a automatizar.

## Documentos
| Documento | Contenido |
|---|---|
| [EDT del proceso productivo](../Produccion%20y%20finanzas/EDT_proceso_productivo.pdf) | Desglose de las operaciones de las tres líneas, nivel de automatización actual y propuesto, recursos y cuellos de botella |
| [VSM de las líneas](../Produccion%20y%20finanzas/VSM_lineas.pdf) | Mapas de flujo de valor del estado actual del campesino, los hilados, el yogur y el UHT |
| [Documento del caso](../Produccion%20y%20finanzas/Documento_del_caso.pdf) | Versión completa del caso, con la empresa integradora y la propuesta |
