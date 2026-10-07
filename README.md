# CAPÍTULO II: RECOPILACIÓN Y ANÁLISIS DE REQUISITOS

## 2.1. Entrevistas

### 2.1.1 Diseño de entrevistas

#### Segmento Objetivo 1: Gestores de Activos Comerciales e Industriales Ligeros (Pymes)

#### Descripción del segmento

Gerentes de operaciones, administradores o dueños de pymes en Lima Metropolitana o provincias con instalaciones solares de mediana escala (10 kW a 50+ kW) bajo tarifas comerciales reguladas. Requieren trazabilidad estricta del autoconsumo frente a la red eléctrica y detección inmediata de fallas para evitar sobrecostos operativos.

--- 

#### Batería de preguntas

#### Perfil Demográfico y Background:

- ¿Cuál es su cargo actual, edad, profesión y en qué distrito opera la sede o planta de su empresa?
- ¿Cuál es el giro comercial de la empresa y cómo está estructurado su equipo operativo o de mantenimiento?
- ¿Podría detallar su trayectoria en la administración de estas instalaciones y cuántos años lleva operando con energía solar en su negocio?

#### Personalidad, Marcas e Influencias:

- ¿Cómo definiría su estilo de gestión respecto al control de costos y la continuidad operativa (ej. preventivo, analítico, reactivo a reportes)?
- ¿Qué marcas de equipamiento solar (inversores, paneles) o referentes del sector energético utiliza o toma como estándar de confianza?
- ¿Qué plataformas de software de gestión industrial, monitoreo de energía o ERP utiliza habitualmente en su día a día? 

#### Tecnología, Dispositivos y Canales (Habilidades):

- ¿A través de qué dispositivos (laptop corporativa, PC de escritorio, smartphone) consulta con mayor frecuencia las operaciones y consumos del negocio?
- ¿Qué canales digitales emplea internamente para coordinar órdenes de trabajo y reparaciones con técnicos o cuadrillas de campo?
- Del 1 al 10, ¿qué tan cómodo se siente su equipo al adoptar plataformas en la nube o herramientas de telemetría IoT?
#### Extracción de Requisitos para la Base de Datos (Pain Points, Entidades y Atributos):

- Entidad Instalacion y Tarifa: ¿Qué datos exactos de su recibo eléctrico (tipo de tarifa ej. BT5A/BT5B, potencia contratada, distribuidora, costo unitario por kWh en Soles) necesita asociar a su instalación para auditar el ahorro real?
- Entidades Medicion y Consumo: ¿Con qué periodicidad o intervalos horarios (ej. cada 15 min, horario punta/fuera de punta) requiere cruzar la generación solar frente a la demanda de su maquinaria para evitar desperdicio energético?
- Entidades Incidencia, Alerta y Anomalia: Cuando ocurre una caída de tensión o fallo en un string completo, ¿qué información mínima necesita que guarde el sistema (panel afectado, pérdida económica estimada en Soles por hora, fecha/hora exacta)?
- Entidades Mantenimiento, Tecnico, Repuesto y Costo: Al contratar una reparación o mantenimiento, ¿qué registros exige documentar (técnico responsable, horas de trabajo, repuestos sustituidos, número de orden y costo total)?

#### Segmento Objetivo 2: Familias Residenciales con Sistemas Solares Activos

#### Descripción del segmento

Propietarios de viviendas unifamiliares en distritos con alta radiación o casas de playa/campo de Lima con kits solares de 3 kW a 10 kW. Se enfrentan a la acumulación de suciedad y polvo (soiling) y requieren monitoreo sencillo, traducción de métricas técnicas a dinero y coordinación confiable de mantenimiento.

---

#### Batería de preguntas

#### Perfil Demográfico y Background:

- ¿Podría indicarme su edad, distrito de residencia habitual y ocupación?   ¿Cómo está conformado su hogar y qué tipo de vivienda tiene (casa urbana, casa de campo, casa de playa)?
- ¿Cuánto tiempo lleva con su sistema solar instalado y cuántos paneles componen aproximadamente su techo fotovoltaico?

#### Personalidad, Marcas e Influencias:

- ¿Cómo se describiría al momento de cuidar la economía y el mantenimiento de su hogar (ej. meticuloso, práctico, desinteresado hasta que algo falla)?
- ¿Qué marcas de tecnología para el hogar o instaladores solares locales le generan mayor confianza y reputación?
- ¿Qué aplicaciones de servicios públicos (banca, app de luz de Enel/Luz del Sur) consulta con regularidad?

#### Tecnología, Dispositivos y Canales (Habilidades):

- ¿En qué dispositivo prefiere revisar el estado de su vivienda: smartphone personal, tablet o computadora familiar?
- ¿Qué canales digitales utiliza para comunicarse con el servicio técnico o proveedores de servicios del hogar (WhatsApp, llamadas, formularios web)?
- Del 1 al 10, ¿qué tan comprensible le resulta la interfaz de la aplicación actual que le entregó la empresa instaladora? 

#### Extracción de Requisitos para la Base de Datos (Pain Points, Entidades y Atributos):

- Entidades Medicion y Ahorro: En lugar de kilovatios o amperios, ¿qué campos comprensibles necesita ver registrados en su historial (soles ahorrados al mes, porcentaje de energía propia consumida, CO2 evitado)?
- Entidades Alerta y Anomalia: Si un panel baja su producción por polvo, suciedad o sombra, ¿qué descripción en lenguaje no técnico espera que guarde la alerta (ej. mensaje descriptivo, nivel de severidad, recomendación de limpieza)?
- Entidades Mantenimiento y Tecnico: Al solicitar un servicio de limpieza de paneles, ¿qué datos del técnico y de la visita le resulta indispensable registrar para su seguridad (nombre, empresa instaladora, calificación/reseñas, fecha y costo del servicio)?   

#### Segmento Objetivo 3: Hogares en Transición Energética (Compradores Potenciales)

#### Descripción del segmento

Jefes de hogar de Lima interesados en migrar a energía solar para reducir sus recibos de luz, pero detenidos por la falta de transparencia en costos, dimensionamiento y rentabilidad real en su distrito.

--- 

#### Batería de preguntas

#### Perfil Demográfico y Background:

- ¿Cuál es su edad, distrito de residencia y número de miembros que habitan en la vivienda?
- ¿Qué tipo de propiedad tiene (casa propia, departamento, casa campestre) y qué área de techo dispone aproximadamente?
- ¿Cuál es el promedio mensual que paga en su recibo de electricidad actualmente?

#### Personalidad, Marcas e Influencias:

- ¿Qué factores pesan más en su proceso de compra de tecnología para el hogar: el ahorro económico, la sostenibilidad ambiental o la reputación de la marca?
- ¿En qué tiendas o canales suele buscar referencias de equipamiento para el hogar (Promart, Sodimac, distribuidores técnicos, recomendaciones de conocidos)?
- Tecnología, Dispositivos y Canales (Habilidades):
¿Qué dispositivos utiliza prioritariamente cuando investiga productos de alto valor antes de comprarlos?
- ¿Qué medios digitales prefiere utilizar para recibir cotizaciones o diagnósticos técnicos (WhatsApp, correo electrónico, cotizadores interactivos en web)?
- Del 1 al 10, ¿qué tan dispuesto está a utilizar un simulador digital interactivo para calcular su consumo de energía?

#### Extracción de Requisitos para la Base de Datos (Pain Points, Entidades y Atributos):

- Entidades Consumo_Historico y Simulacion: Para calcular cuántos paneles necesita, ¿qué variables de su consumo estaría dispuesto a registrar (consumo en kWh de los últimos meses, inventario de electrodomésticos de alto consumo, horarios de permanencia en casa)?
- Entidad Catalogo_Panel: Al evaluar modelos de paneles en un catálogo, ¿qué atributos técnicos considera indispensables para comparar opciones (marca, potencia nominal en Watts, años de garantía, costo unitario, eficiencia de degradación)?
- Entidades Factor_Emision y Presupuesto: ¿Qué indicadores de impacto ambiental desearía ver reflejados en el cálculo final (árboles equivalentes, reducción estimada de huella de carbono, tiempo estimado de retorno de inversión en meses/años)?

### 2.1.2 Registro de entrevistas

Las entrevistas fueron registradas en video y se organizaron según el segmento objetivo correspondiente. Cada registro incluye información básica del entrevistado, captura del video, enlace, timing, duración y un resumen descriptivo de sus respuestas, prestando especial atención a sus hábitos tecnológicos y pain points.

**Enlace del video consolidado de entrevistas:** [Entrevistas juntas]()

##### Segmento Objetivo 1: Gestores de Activos Comerciales e Industriales Ligeros (Pymes)

**Entrevista 1**
*   **Nombres y Apellidos:** Elias Coronel
*   **Edad:** 26 años
*   **Ocupación:** Ingeniero Industrial
*   **Distrito de residencia:** San Borja
*   **Inicio en el video (Timing):** 0:01
*   **Duración:** 6 minutos y 12 segundos
*   **Link de Video:** https://youtu.be/FVRP54Lk8DQ
*   **Screenshot:**
  ![Ruta_screenshot_entrevista_1](assets/Chapter-2/Screenshot_entrevista.png)
*   **Resumen descriptivo:** 	Elias comentó que es administrador de operaciones en una fábrica en Villa el Salvador, donde gestiona el mantenimiento con técnicos internos y externos. Mencionó que, con tres años de experiencia en energía solar, aplica un enfoque preventivo y analítico para controlar costos y evitar paradas en la producción. Explicó que priorizan equipos solares confiables y con buen soporte, gestionando la información mediante un ERP y Excel desde su laptop corporativa o celular. Señaló que su equipo se adapta bien a la tecnología, coordinando sus labores diarias de forma práctica por WhatsApp y correo. Reconoció que para auditar el impacto de los paneles necesita un historial detallado del consumo y tarifas, medido idealmente en intervalos de 15 minutos para ser preciso. También admitió que, ante cualquier falla, es vital que el sistema registre automáticamente el equipo afectado, el tiempo inactivo y la pérdida económica. Finalmente, indicó que toda intervención técnica debe quedar estrictamente documentada, detallando el responsable, los repuestos usados, las horas invertidas y el costo total de la reparación.


##### Segmento Objetivo 2: Familias Residenciales con Sistemas Solares Activos

**Entrevista 1** 
*   **Nombres y Apellidos:** Adriana Salazar
*   **Edad:** 24 años
*   **Ocupación:** Ingeniera Civil
*   **Distrito de residencia:** La Molina
*   **Inicio en el video (Timing):** 0:01
*   **Duración:** 5 minutos y 8 segundos
*   **Link de Video:** https://youtu.be/FVRP54Lk8DQ
*   **Screenshot:**
  ![Ruta_screenshot_entrevista_1](assets/Chapter-2/Screenshot_entrevista.png)
*   **Resumen descriptivo:** La ingeniera Salazar comentó que tiene 24 años y vive con su familia en La Molina. Mencionó que, con su perfil de ingeniera civil, mantiene un enfoque práctico y minucioso para controlar el mantenimiento de su hogar, buscando resolver problemas de forma rápida. Explicó que cuenta con 12 paneles solares instalados desde hace dos años y que, al elegir, se inclina por marcas reconocidas con buenas reseñas. Señaló que gestiona los servicios de su hogar utilizando las apps del banco y de la compañía eléctrica, y que, para el sistema solar, prefiere la comodidad de su smartphone para revisar su historial. Reconoció que, para coordinar servicios técnicos, WhatsApp es su principal canal por la facilidad de enviar imágenes o videos de forma rápida. También admitió que la aplicación de sus paneles solares es relativamente sencilla, pero que algunos de sus datos técnicos pueden resultar difíciles de interpretar. Finalmente, indicó que para llevar un buen registro de los paneles, le interesa conocer su ahorro en soles, el porcentaje de energía que utiliza de los mismos y que, si estos fallan, le gustaría recibir un mensaje sencillo y detallar la gravedad del problema.
  

##### Segmento Objetivo 3: Hogares en Transición Energética (Compradores Potenciales)

**Entrevista 1 - [Nombre del entrevistado]**
*   **Edad:** [rellenar campo]
*   **Distrito:**[rellenar campo]
*   **Ocupación:** [rellenar campo]
*   **Inicio en el video (Timing):** [rellenar campo]
*   **Duración:** [rellenar campo]
*   **Link de Video:** [Entrevista]()
*   **Screenshot:**
  ![Ruta_screenshot_entrevista_1](assets/Chapter-2/Screenshot_entrevista.png)
*   **Resumen descriptivo:** [rellenar campo]


### 2.1.3 Análisis de entrevistas

El análisis de entrevistas permite identificar patrones recurrentes, características objetivas, características subjetivas, necesidades operativas y oportunidades de mejora relacionadas con el dominio tecnologico de SolarPulse IoT.

##### Resumen de entrevistas analizadas

| Segmento | Entrevistas analizadas | Cantidad |
| :--- | :--- | :--- |
| Gestores de Activos Comerciales e Industriales Ligeros | [Agregar nombre entrevistados] | 2 |
| Familias Residenciales con Sistemas Solares Activos | [Agregar nombre entrevistados] | 2 |
| Hogares en Transición Energética | [Agregar nombre entrevistados] | 2 |
| **Total** | — | **6** |

##### Segmento Objetivo 1: Gestores de Activos Comerciales e Industriales Ligeros

###### Análisis de características objetivas

| Característica objetiva | Evidencia identificada | Porcentaje |
| :--- | :--- | :--- |
| [Datos importantes] | [Evidencia concreta resaltada de las caracteristicas] | [porcenjate total %] |
| [Datos importantes] | [Evidencia concreta resaltada de las caracteristicas] | [porcenjate total %] |
| [Datos importantes] | [Evidencia concreta resaltada de las caracteristicas] | [porcenjate total %] |
| [Datos importantes] | [Evidencia concreta resaltada de las caracteristicas] | [porcenjate total %] |

###### Análisis de características subjetivas

| Característica subjetiva | Evidencia identificada | Porcentaje |
| :--- | :--- | :--- |
| [Datos importantes] | [Evidencia concreta resaltada de las caracteristicas] | [porcenjate total %] |
| [Datos importantes] | [Evidencia concreta resaltada de las caracteristicas] | [porcenjate total %] |
| [Datos importantes] | [Evidencia concreta resaltada de las caracteristicas] | [porcenjate total %] |

**Interpretación del segmento:**  
[Enunciado completo de los 2 analisis diseñasdos previamente]

##### Segmento Objetivo 2: Familias Residenciales con Sistemas Solares Activos

###### Análisis de características objetivas

| Característica objetiva | Evidencia identificada | Porcentaje |
| :--- | :--- | :--- |
| [Datos importantes] | [Evidencia concreta resaltada de las caracteristicas] | [porcenjate total %] |
| [Datos importantes] | [Evidencia concreta resaltada de las caracteristicas] | [porcenjate total %] |
| [Datos importantes] | [Evidencia concreta resaltada de las caracteristicas] | [porcenjate total %] |
| [Datos importantes] | [Evidencia concreta resaltada de las caracteristicas] | [porcenjate total %] |

###### Análisis de características subjetivas

| Característica subjetiva | Evidencia identificada | Porcentaje |
| :--- | :--- | :--- |
| [Datos importantes] | [Evidencia concreta resaltada de las caracteristicas] | [porcenjate total %] |
| [Datos importantes] | [Evidencia concreta resaltada de las caracteristicas] | [porcenjate total %] |
| [Datos importantes] | [Evidencia concreta resaltada de las caracteristicas] | [porcenjate total %] |

**Interpretación del segmento:**  
[Enunciado completo de los 2 analisis diseñasdos previamente]

##### Segmento Objetivo 3: Hogares en Transición Energética (Compradores Potenciales)

###### Análisis de características objetivas

| Característica objetiva | Evidencia identificada | Porcentaje |
| :--- | :--- | :--- |
| [Datos importantes] | [Evidencia concreta resaltada de las caracteristicas] | [porcenjate total %] |
| [Datos importantes] | [Evidencia concreta resaltada de las caracteristicas] | [porcenjate total %] |
| [Datos importantes] | [Evidencia concreta resaltada de las caracteristicas] | [porcenjate total %] |
| [Datos importantes] | [Evidencia concreta resaltada de las caracteristicas] | [porcenjate total %] |

###### Análisis de características subjetivas

| Característica subjetiva | Evidencia identificada | Porcentaje |
| :--- | :--- | :--- |
| [Datos importantes] | [Evidencia concreta resaltada de las caracteristicas] | [porcenjate total %] |
| [Datos importantes] | [Evidencia concreta resaltada de las caracteristicas] | [porcenjate total %] |
| [Datos importantes] | [Evidencia concreta resaltada de las caracteristicas] | [porcenjate total %] |

**Interpretación del segmento:**  
[Enunciado completo de los 2 analisis diseñasdos previamente]

##### Conclusiones generales del análisis

[Conclusiones generales de todas las entrevistas realizadas]

## 2.2. Requisitos

#### Requisitos funcionales

| Código | Descripción | Entidad Directa Relacionada |
| ------ | -------     | ------    |
| US-01  | Registrar y gestionar los usuarios de la plataforma de acuerdo con su rol. | Usuario, Rol |
| US-02 | Registrar y gestionar las instalaciones fotovoltaicas. | Instalación |
| US-03 | Registrar los paneles solares asociados a una instalación fotovoltaica. | Panel Solar |
| US-04 | Registrar sensores IoT asociados a los paneles solares. | Sensor IoT |
| US-05 | Registrar las mediciones obtenidas por los sensores (Voltaje, corriente, temperatura). | Medición |
| US-06 | Identificar posibles anomalías a partir de las mediciones registradas. | Anomalía |
| US-07 | Identificar posibles anomalías a partir de las mediciones registradas. | Anomalía |
| US-08 | Generar alertas cuando se detecten condiciones anormales en paneles o instalaciones. | Alerta |
| US-09 | Registrar y gestionar las incidencias detectadas en paneles solares | Incidencia |
| US-10 | Generar órdenes de mantenimiento asociadas a una incidencia. | Orden de mantenimiento |
| US-11 |Asignar órdenes de mantenimiento a técnicos responsables. | Orden de mantenimiento, Técnico |
| US-12 | Registrar las actividades realizadas durante una intervención de mantenimiento. | Activador de mantenimiento |
| US-13 | Registrar los repuestos utilizados durante la actividad de mantenimiento | Repuesto, Detalle de presupuesto |
| US-14 | Registrar los costos relacionados con actividades de mantenimiento y repuestos utilizados. | Costo mantenimiento |
| US-15 | Consultar el historial de mantenimientos realizados sobre una instalación o panel. | Instalación, Panel Solar, Orden de mantenimiento, Activador de mantenimiento |


#### Requisitos No funcionales

| Código | Descripción | Propósito |
| ------ | ----------- | --------- |
| RNF-1 | Validar credenciales y permisos por rol en un tiempo máximo de 1.5 segundos, bloqueando el acceso al tercer intento fallido continuo  | Seguridad |
| RNF-2 | Ejecutar validaciones de integridad referencial y comprobación de esquemas en menos de 2 segundos por cada lote de mediciones entrantes. |  Integridad  |
| RNF-3 | Ingerir y persistir de manera continua más de 1,000 registros por segundo de telemetría sin degradar el rendimiento de lectura. | Escalabilidad |
| RNF-4 | Admitir un incremento anual del 100% en el volumen de almacenamiento de lecturas históricas manteniendo tiempos de consulta estables mediante particionamiento temporal. | Escalabilidad |
| RNF-5 | Retornar métricas analíticas agregadas (por día, mes o año) en menos de 3 segundos para tableros de control con más de 100 paneles. | Rendimiento |
| RNF-6 | Transformar y registrar cargas de telemetría de sensores IoT multimarca en menos de 5 segundos por trama entrante. | Interoperabilidad |
| RNF-7 | Recuperar la base de datos a su último estado consistente en un lapso máximo de 2 horas (RTO) ante fallos críticos del sistema gestor. | Recuperabilidad |
| RNF-8 | Mantener la operatividad de los servicios de lectura y persistencia durante al menos el 99.5% del tiempo anual. | Disponibilidad |
| RNF-9 | Registrar y enlazar automáticamente el identificador de la anomalía, la alerta y la incidencia técnica generada en no más de 2 segundos. | Trazabilidad |
| RNF-10 | Documentar en la base de datos el historial secuencial de intervenciones (orden de trabajo, técnico asignado, tareas y repuestos utilizados) en un tiempo menor a 3 segundos por evento. | Trazabilidad |

