

---

**UNIVERSIDAD PERUANA DE CIENCIAS APLICADAS**

**Ingeniería de Software**  
**Ingenieria de Sistema de Información**

**Período**: 2026-20  
**Curso**: 1ASI0787 | Base de datos  
**NRC**: 15869  
**Docente**:  Rafael Oswaldo Castro Veramendi

---

**INFORME DE TRABAJO FINAL**

**Nombre del startup: Heliosync Technologie**

**Nombre del producto: SolarPulse IoT**

**Relación de integrantes**

| Código | Apellidos y Nombres |
| :---- | :---- |
| U20211A574 | Navarro Flores Renzo Jesus |
| U20221f624 | Bravo Castillo Rojo Miguel Alejandro |
| U20241B647 | Quispe Vargas Juan Carlos |
| U202410464 | Martínez Zeta José Alonso  |
| U20221A006 | Soto Vásquez, María Fernanda |
| U202313231 | Flores Masias Adriel Jose |

# **Registro de versiones** {#registro-de-versiones}

| Versión | Fecha | Autores | Descripción de modificaciones |
| :---: | :---: | ----- | ----- |
| TP | 9/10/2026 | Renzo Jesus, Navarro Flores Miguel Alejandro, Bravo Catillo Rojo Juan Carlo, Quispe Vargas José Alonso, Martínez Zeta  María Fernanda, Soto Vásquez Flores Masias Adriel Jose | Desarrollo de nuestro diseño complementario de la base de datos de SolarPulse IoT en base a las entrevistas obtenidas, se plantea el diseño del diagrama de entidad-relación lógico, diagrama de entidad-relación físico y se determina que software de base de datos vamos a usar |

# **Tabla de contenidos** {#tabla-de-contenidos}

**[Registro de versiones	2](#registro-de-versiones)**

[**Tabla de contenidos	3**](#tabla-de-contenidos)

[**Student outcome	4**](#student-outcome)

[**1\. CAPÍTULO I: INTRODUCCIÓN	5**](#capítulo-i:-introducción)

[1.1. Startup profile	5](#startup-profile)

[1.1.1. Descripción de startup	5](#descripción-de-startup)

[1.1.2. Perfiles de integrantes del grupo	6](#perfiles-de-integrantes-del-grupo)

[1.2. Solution Profile	8](#solution-profile)

[1.2.1. Antecedentes y problemáticas	8](#antecedentes-y-problemáticas)

[1.2.2. Propuestas de valor	10](#propuestas-de-valor)

[1.3. Segmentos objetivo	13](#segmentos-objetivo)

[**2\. CAPÍTULO II: RECOPILACIÓN Y ANÁLISIS DE REQUISITOS	16**](#capítulo-ii:-recopilación-y-análisis-de-requisitos)

[2.1. Entrevistas	16](#entrevistas)

[2.1.1. Diseño de entrevistas	16](#diseño-de-entrevistas)

[2.1.2. Registro de entrevistas	19](#registro-de-entrevistas)

[2.1.3. Análisis de entrevistas	19](#análisis-de-entrevistas)

[2.2. Requisitos	20](#requisitos)

[Requisitos funcionales	20](#requisitos-funcionales)

[Requisitos No funcionales	21](#requisitos-no-funcionales)

[**3\. CAPÍTULO III: DISEÑO DE BASE DE DATOS	21**](#capítulo-iii:-diseño-de-base-de-datos)

[3.1. Entidades	21](#entidades)

[3.2. Atributos	23](#atributos)

[3.3. Enfoque relacional	23](#enfoque-relacional)

[3.3.1. Diagrama entidad-relación lógico	23](#diagrama-entidad-relación-lógico)

[**4\. CAPÍTULO IV: IMPLEMENTACIÓN DE BASE DE DATOS	23**](#capítulo-iv:-implementación-de-base-de-datos)

[4.1. Sistemas de gestión de base de datos	23](#sistemas-de-gestión-de-base-de-datos)

[4.1.1. Evaluación y elección del sistema de gestión de base de datos relacional	23](#evaluación-y-elección-del-sistema-de-gestión-de-base-de-datos-relacional)

[4.2. Diagramas de datos	23](#diagramas-de-datos)

[4.2.1. Diagrama entidad-relación físico	23](#diagrama-entidad-relación-físico)

[**Conclusiones	24**](#conclusiones)

[**BIBLIOGRAFÍA	25**](#bibliografía)

[**ANEXOS	25**](#anexos)

# **Student outcome** {#student-outcome}

| Criterio específico | Acciones realizadas | Conclusiones |
| ----- | ----- | ----- |
| 7.c1. Actualiza conceptos y conocimientos necesarios para su desarrollo profesional y en especial para su proyecto en soluciones de ingeniería de software. |  |  |
| 7.c2. Reconoce la necesidad del aprendizaje permanente para el desempeño profesional y el desarrollo de proyectos en soluciones de tecnologías de ingeniería de software. |  |  |

1. # **CAPÍTULO I: INTRODUCCIÓN** {#capítulo-i:-introducción}

   1. ## **Startup profile** {#startup-profile}

      1. ### Descripción de startup {#descripción-de-startup}

         Somos “**Heliosync Technologie**” una Startup de base tecnológica especializada en telemetría IoT y arquitecturas de datos en la nube para optimizar activos fotovoltaicos distribuidos en tiempo real.

         **Misión:**

         Maximizar la eficiencia operativa y el retorno de inversión de instalaciones solares residenciales, comerciales e industriales mediante la centralización de datos IoT, analítica predictiva y gestión automatizada del mantenimiento.

         **Visión:**

         Consolidarse como el ecosistema estándar de observabilidad e inteligencia operativa para microrredes y sistemas solares distribuidos en América Latina, acelerando la transición hacia matrices energéticas descarbonizadas y confiables.

         

         

         

         

         

         

         

         

         

         

         

         

         

         

         

         

         

         

         

         

         

         

         

      2. ### Perfiles de integrantes del grupo {#perfiles-de-integrantes-del-grupo}

|  | Nombre y Apellidos: Renzo Jesus Navarro Flores Código estudiante: U20211A574 Carrera: Ingeniería de Software Habilidad y conocimientos: Soy estudiante de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas. Cuento con conocimientos de desarrollo de documentación, requisitos y requerimientos, arquitectura de software y manejo de redes con cisco packet tracer y arduino. Dentro de SolarPulse IoT, aportaré mi lógica de análisis para buscar vulnerabilidades en el sistema y preparar contramedidas, responsabilidad y trabajo colaborativo. |
| :---- | :---- |
|  | **Nombre y Apellidos:** Bravo Castillo Rojo Miguel Alejandro **Código estudiante:** u20221f624 **Carrera:** Ingeniería de Software  **Habilidad y conocimientos:** Estudiante de la carrera de ingeniería de Software siento que puedo aportar al equipo con mis conocimientos acerca ux/ui y conocimientos en el lenguaje de programación C++ además siendo autocrítico con nuestra iniciativa para asi poder alcanzar un alto grado de satisfacción en el proyecto. |
| Foto | **Nombre y Apellidos:** Soto Vásquez, María Fernanda **Código estudiante:** u20221a006 **Carrera:** Ingeniería de Software **Habilidad y conocimientos:** Me considero una estudiante comprometida y responsable, con muchas ganas de seguir aprendiendo y creciendo tanto a nivel académico como personal. Me gusta trabajar en equipo, aportar ideas y apoyar a mis compañeros para lograr objetivos en conjunto. |
| Foto | **Nombre y Apellidos:** Martínez Zeta, José Alonso **Código estudiante:** U202410464 **Carrera:** Ingeniería de Software **Habilidad y conocimientos:** Poseo conocimientos en los lenguajes de programación C++, Python, y JS. Tambien tengo una capacidad analita buena, creatividad y adaptabilidad, los cuales me ayudaran al desarrollo de mi carrera y experiencia.   |
|  | **Nombre y Apellidos:** Juan Carlos Quispe Vargas  **Código estudiante:** U20241N647 **Carrera:** Ingeniería de Software **Habilidad y conocimientos:** Conocimientos en C++, Python, estructuras de datos, algoritmos, bases de datos, redes, arquitectura de computadores y desarrollo de software. Capacidad para resolver problemas, analizar requerimientos y desarrollar proyectos académicos aplicando fundamentos de ingeniería de software. |
| Foto | **Nombre y Apellidos:** Adriel Jose, Flores Masias **Código estudiante:** U202313231 **Carrera:** Ingeniería de Software **Habilidad y conocimientos:** |

       


2. ## **Solution Profile** {#solution-profile}

   SolarPulse IoT es una plataforma en la nube (SaaS) que funciona como el "médico de cabecera" de cualquier instalación solar. Mediante pequeños sensores conectados a internet, monitoreamos la salud de cada panel en tiempo real.  
* Monitoreo panel por panel: Sabemos exactamente cuánto produce cada módulo (voltaje, corriente y temperatura) segundo a segundo.  
* Detección temprana de problemas: Si un panel genera menos energía de lo normal o levanta demasiada temperatura, el sistema genera una alerta antes de que se convierta en una avería costosa.  
* Todo en una sola pantalla: El cliente ve en su celular cuánta energía produce, cuánta consume en su casa o negocio y cuánto dinero y emisiones de CO2 está ahorrando.  
* Soporte técnico directo: Conectamos la falla detectada con técnicos autorizados para coordinar mantenimientos preventivos rápidos y con costos transparentes.

  1. ### Antecedentes y problemáticas {#antecedentes-y-problemáticas}

1. **Quiénes están involucrados (Who):**

   Afecta principalmente a empresas instaladoras de paneles solares, técnicos de mantenimiento de campo y propietarios de activos fotovoltaicos (ya sean pymes comerciales o familias residenciales).

2. **Qué problema resuelve la solución (What):**

   Existe una carencia de visibilidad operativa granular en los sistemas fotovoltaicos, lo que impide detectar a tiempo caídas de eficiencia y fallas tempranas en paneles específicos.

3. **Cuándo ocurre el problema (When):**

   Ocurre de manera continua durante la operación diaria de los paneles solares, específicamente en el periodo entre que ocurre una falla silenciosa (como acumulación de suciedad o degradación térmica) y el momento en que se detecta en la facturación o revisión.

4. **Dónde ocurre el problema (Where):**

   En instalaciones de sistemas solares distribuidos en América Laina, con un enfoque inicial en Lima Metropolitana, donde factores climáticos como alta humedad, polvo y hollín urbano afectan los paneles.

   

5. **Por qué es relevante este problema (Why):**

   Porque las soluciones actuales provistas por los fabricantes de inversores son cerradas, no interoperables y solo detectan anomalías a nivel macro. Esto oculta fallas individuales a nivel de panel y evita un diagnóstico preciso.

6. **Cómo se gestiona actualmente el problema (How)**

   El problema se manifiesta mediante pérdidas energéticas que pasan desapercibidas y obligan a los instaladores a realizar visitas técnicas “a ciegas” para diagnosticar problemas en toda la red, saturando a las cuadrillas de mantenimiento.

7. **Cuánto impacta el problema (How much)**

   • **Inversión:** Comprende los costos de sensores físicos, conectividad (celular o satelital) y consumo de computación en la nube para consolidar un centro de datos unificado en tiempo real. Los costos de sensores IoT, dispositivos de borde y plataformas SaaS han disminuido entre 60% y 70% desde 2015, haciendo económicamente viable el monitoreo granular incluso en instalaciones pequeñas. Las plataformas basadas en nube típicamente cuestan entre USD 0.50 y 2.00 por kW al año, y reducen el costo total de propiedad entre 30% y 40% frente a soluciones on‑premise en períodos de cinco años. Para instalaciones comerciales, los sistemas completos de monitoreo suelen requerir inversiones de entre USD 5,000 y 25,000, dependiendo de la complejidad y el nivel de granularidad.

   • **Retorno/Impacto:** La implementación de un sistema de monitoreo panel por panel con capacidades predictivas se traduce en una reducción de hasta un 30–35% en los costos de operación y mantenimiento (O\&M) frente a estrategias reactivas, gracias a la disminución de fallas no planificadas y a una mejor programación de las intervenciones. Asimismo, permite un incremento de hasta un 5% en la producción energética anual (yield), con potenciales mayores (5–15%) en instalaciones con sombreado parcial, suciedad o configuraciones complejas. Esta optimización tecnológica posibilita migrar de una gestión reactiva a una estrategia predictiva basada en inteligencia artificial y sensores IoT, lo que reduce los costos de mantenimiento entre un 8% y un 12% en comparación con esquemas preventivos tradicionales. De este modo, se maximiza el retorno de inversión (ROI) y se mitiga el riesgo financiero de los proyectos fotovoltaicos distribuidos.

   

   

   2. ### Propuestas de valor {#propuestas-de-valor}

      En el desarrollo de productos digitales y plataformas IoT, el principal riesgo no radica en la complejidad técnica de conectar sensores a una base de datos, sino en construir un sistema con funcionalidades que el mercado no esté dispuesto a adoptar o pagar. Los enfoques tradicionales de diseño basados en extensos documentos de requisitos asumen certezas operativas que, en etapas tempranas, son solo suposiciones sin validar.

      Para el desarrollo de SolarPulse IoT, adoptamos el marco del Lean UX Canvas (propuesto por Jeff Gothelf) por tres razones fundamentales:

* Enfoque centrado en resultados (Outcomes sobre Outputs): Cambia la prioridad de "cuántas tablas o pantallas programamos" a "qué impacto real generamos" (como reducir el tiempo de detección de fallas o los costos de mantenimiento correctivo).

* Mitigación de riesgos mediante hipótesis: Permite estructurar la interoperabilidad de hardware, la telemetría granular y el modelo de negocio SaaS como supuestos contrastables antes de comprometer recursos masivos de ingeniería.

* Alineación continua con el usuario real: Conecta las necesidades operativas de instaladores, técnicos y dueños de activos directamente con el diseño de la arquitectura de datos, asegurando un ciclo rápido de retroalimentación, aprendizaje y validación de valor en el mercado.


  **Business Problem (Problema del Negocio)**

  El despliegue de sistemas fotovoltaicos distribuidos carece de visibilidad operativa granular. Las soluciones actuales de los fabricantes de inversores son cerradas, no interoperables y solo detectan anomalías a nivel macro, ocultando fallas individuales como acumulación de suciedad (soiling), microfisuras o degradación térmica.

  Esto genera pérdidas silenciosas de entre 8% y 15% en la generación energética anual, encarece el mantenimiento correctivo hasta en un 30% frente al preventivo y prolonga el tiempo medio de detección de fallas (MTTD) de 15 a 45 días, erosionando el ROI del usuario y saturando a los instaladores con visitas técnicas a ciegas.

  **Business Outcomes (Resultados del Negocio)**

  Adopción: Lograr que el 60% de los nuevos clientes de empresas instaladoras (EPCs) aliadas se den de alta en el SaaS durante los primeros 6 meses.

  Retención (Bajo Churn): Mantener un churn rate mensual menor al 1.5%, impulsado por el valor continuo del historial de fallas y mantenimientos.

  Expansión B2B: Captar al menos 15 empresas instaladoras/mantenedoras en el primer año que gestionen carteras de más de 50 instalaciones activas en la plataforma.

  Métricas de Salud Operativa: Reducir el tiempo promedio de diagnóstico remoto de incidencias técnicas en un 70%.

  **Users & Customers (Usuarios y Clientes)**

  Cliente B2B (Comprador principal): Empresas instaladoras de paneles solares (EPCs) y gestores de mantenimiento de activos que administran flotas fotovoltaicas.

  Usuario Técnico (Operativo): Ingenieros de campo y técnicos de soporte solar que necesitan diagnosticar la causa raíz de las averías antes de desplazarse.

  Usuario Final / Propietario (B2C o B2B corporativo): Dueños de viviendas o gerentes de operaciones en pymes que buscan proteger su inversión y validar el ahorro en su factura eléctrica.

  **User Outcomes & Benefits (Beneficios para el Usuario)**

  Para el Instalador/Técnico: Reducción de visitas en falso (truck rolls) y optimización de cuadrillas gracias a diagnósticos que identifican el panel y sensor exacto con fallo.

  Para el Propietario/Inversor: Garantía de máxima generación energética diaria, alertas tempranas al teléfono antes de pérdidas acumuladas y reportes claros de CO2 evitado y ahorro monetario.

  Transparencia: Registro fidedigno del historial técnico y costos de cada mantenimiento para validar garantías de equipos.

  **Solutions (Ideas de Solución)**

  Motor de Ingestión Agnóstico IoT: Recepción de telemetría (voltaje, corriente, temperatura) vía MQTT/HTTPS y persistencia estructurada en base de datos (paneles, sensores, mediciones).

  Algoritmo de Detección de Anomalías: Comparación en tiempo real entre paneles de un mismo arreglo para levantar registros automáticos en fallas ante caídas de potencia o sobrecalentamiento.

  Módulo Operativo de Mantenimiento: Interfaz para que el instalador asigne órdenes de trabajo a técnicos, documente repuestos, registre costos y cierre incidencias.

  Dashboard Multi-Inquilino (SaaS): Vistas diferenciadas con métricas financieras y ambientales para el dueño, y telemetría avanzada por string/panel para la empresa operadora.

  **Hypotheses (Hipótesis)**

  H1 (Interoperabilidad): Creemos que centralizar datos de múltiples marcas en una sola base de datos normalizada resolverá la fragmentación para las empresas instaladoras. Sabremos que tuvimos éxito cuando el 75% de las empresas piloto conecte al menos dos marcas de hardware distintas en un mismo panel.

  H2 (Eficiencia Operativa): Creemos que alertar sobre desvíos térmicos y caídas de corriente a nivel panel reducirá el gasto operativo (OPEX). Sabremos que tuvimos éxito cuando el costo de visitas de emergencia de los técnicos aliados se reduzca en un 25% en los primeros 90 días de uso.

  H3 (Retención de Usuarios): Creemos que mostrar el balance neto entre generación y consumo en tiempo real aumentará el compromiso del dueño del activo. Sabremos que tuvimos éxito cuando el propietario revise la aplicación al menos 3 veces por semana.

  **What’s the Most Important Thing We Need to Learn First? (Supuesto más riesgoso)**

  ¿Están las empresas instaladoras dispuestas a migrar de las aplicaciones gratuitas provistas por los fabricantes de inversores a una suscripción SaaS de terceros a cambio de telemetría granular y diagnósticos predictivos?

  **What’s the Least Amount of Work Needed to Learn It? (MVP / Experimento)**

  Experimento: Implementar un piloto cerrado con 3 empresas instaladoras medianas monitoreando entre 5 y 10 instalaciones críticas con sensores IoT comerciales de bajo costo ya integrados al esquema central (mediciones y fallas).

  Criterio de Validación: Durante 60 días, medir si las alertas automatizadas detectaron al menos 2 anomalías reales no visibles en la app del inversor y si el instalador aceptaría pagar una tarifa recurrente mensual por panel para mantener el servicio activo.

  **Lean UX Canvas**

  El Lean UX Canvas sintetiza los principales elementos del modelo de aprendizaje de SolarPulse IoT y relaciona el problema de negocio con los usuarios, resultados, supuestos, soluciones e hipótesis que serán evaluadas.

![][image1]

3. ## **Segmentos objetivo** {#segmentos-objetivo}

   **Segmento Objetivo 1: Gestores de Activos Comerciales e Industriales Ligeros (Pymes de Alto Consumo)**

   Perfil y Cobertura Geográfica: Gerentes de operaciones, administradores de finanzas o dueños de pymes en Lima Metropolitana (talleres de manufactura en Ate o San Juan de Lurigancho, centros logísticos en Huachipa, colegios privados, clínicas y almacenes refrigerados). Operan con contratos comerciales o residenciales de alta demanda (tarifas reguladas tipo BT5B/BT5A de Luz del Sur o Pluz Energía).

   Contexto Operativo: Cuentan con arreglos fotovoltaicos de mediana escala (10 kW a 50+ kW) instalados por integradores locales (como Novum Solar o SolarTech Perú). Su modelo económico depende 100% del autoconsumo inmediato en horario diurno para reducir la compra de energía a la red distribuidora.

   **Puntos de Dolor (Pain Points):** 

* Falta de sincronización entre los picos de consumo de sus maquinarias y las ventanas horarias de máxima irradiación solar.  
* Inexistencia de reportes financieros automatizados en moneda local (Soles) que demuestren a gerencia el ahorro real frente a la facturación de la red.  
* Miedo a paradas no planificadas de inversores o bancos de paneles que deriven en sobrecostos imprevistos de electricidad comercial.

  Propuesta de Valor / Beneficio Buscado: Certeza financiera del retorno de inversión (ROI), balance neto de energía en tiempo real y detección inmediata de ineficiencias operativas antes del cierre mensual de facturación.

  **Requerimientos Mandatorios para la Base de Datos:**

* Instalaciones: Atributos para la tarifa eléctrica local contratada (moneda, costo unitario por kWh en soles, distribuidora y potencia contratada).  
* Consumos vs. Mediciones: Indexación temporal estricta por intervalos horarios (15-60 min) para contrastar demanda de carga vs. generación y calcular el porcentaje de autoconsumo e inyección/desperdicio.  
* Fallas: Categorización técnica de incidencias críticas que impacten strings completos de paneles, con registro de pérdidas económicas estimadas en soles durante el tiempo de inactividad.

  **Segmento Objetivo 2: Familias Residenciales con Sistemas Solares Activos (Propietarios Urbanos y Campestres)**

  Perfil y Cobertura Geográfica: Propietarios de viviendas residenciales unifamiliares en distritos con alta radiación o casas de campo/playa de Lima (La Molina, Cieneguilla, Chosica, Pachacámac, Lurín y balnearios del sur de Lima). Cuentan con instalaciones de autoconsumo de 3 kW a 10 kW (de 6 a 24 paneles).

  Contexto Operativo: Adquirieron sus kits solares llave en mano mediante empresas instaladoras residenciales (como Waira Energía o Ecovoltaica). Se enfrentan al clima particular de la costa de Lima: alta humedad y acumulación constante de polvo/hollín urbano, lo que produce degradación silenciosa (soiling).

  **Puntos de Dolor (Pain Points):**

* "Abandono posventa": el instalador original entrega una aplicación en inglés llena de variables eléctricas abstractas (amperios, voltios) que la familia no comprende ni revisa.  
* Incertidumbre estacional: desconocen si una baja producción se debe a la nubosidad habitual de Lima o a suciedad/avería física en un panel específico.  
* Falta de una red confiable y accesible de técnicos para servicios de limpieza y mantenimiento correctivo.

  Propuesta de Valor / Beneficio Buscado: Tranquilidad de que el techo solar funciona de forma óptima, visualización de métricas en soles ahorrados y alertas preventivas simples que indican cuándo conviene limpiar o revisar un panel puntual.

  **Requerimientos Mandatorios para la Base de Datos:mediciones:** 

* Algoritmo de normalización que traduzca la potencia instantánea a métricas comprensibles para el usuario final (ahorro acumulado en soles y porcentaje de autosuficiencia energética).  
* Fallas: Campo de descripción en lenguaje natural no técnico (ej. "Panel 4: Se detecta reducción de corriente compatible con acumulación de polvo o sombra").  
* Mantenimientos y técnicos: Trazabilidad de órdenes de servicio para documentar limpiezas de paneles, revisiones de cableado, costo del servicio y calificación del técnico.

  **Segmento Objetivo 3: Hogares en Transición Energética (Compradores y Evaluadores Potenciales)**

  Perfil y Cobertura Geográfica: Jefes de hogar y familias de sectores socioeconómicos B y C+ de Lima con vivienda propia, conscientes del impacto ambiental o frustrados por los incrementos continuos en los recibos de luz. Evalúan activamente pasarse a la energía solar o compran kits básicos en cadenas de mejoramiento del hogar (Promart, Sodimac) y distribuidores eléctricos locales.

  Contexto Operativo: Tienen la intención de compra pero están paralizados en la fase de decisión por falta de información transparente, miedo a sobrecostos de instalación y desconfianza técnica hacia proveedores informales.

  **Puntos de Dolor (Pain Points):**

* Inseguridad sobre la rentabilidad real de la tecnología solar en el microclima de su distrito (ej. creen erróneamente que en Lima "no sale a cuenta" por los inviernos nublados).  
* Dificultad para saber cuántos paneles realmente necesitan según sus electrodomésticos y hábitos de consumo diario.  
* Ausencia de métricas tangibles de sostenibilidad que validen el aporte ambiental de su inversión.

  Propuesta de Valor / Beneficio Buscado: Certeza y acompañamiento técnico antes de comprar. Poder ingresar sus consumos históricos para recibir un dimensionamiento fidedigno basado en datos reales de instalaciones vecinas, con proyección de ahorro y métricas ambientales claras.

  **Requerimientos Mandatorios para la Base de Datos:**

* Consumos: Capacidad de registrar patrones de consumo típicos de viviendas (curvas de carga históricas) para ejecutar simulaciones de dimensionamiento.  
* Paneles: Catálogo normalizado de especificaciones de hardware comercial (marca, modelo, potencia nominal de fábrica y coeficientes de degradación térmica) para contrastar alternativas del mercado.  
* Instalaciones: Parámetros de factores de emisión locales (kg CO2/kWh) para calcular equivalencias tangibles (árboles equivalentes plantados y emisiones evitadas) como factor motivacional de adopción.

2. # **CAPÍTULO II: RECOPILACIÓN Y ANÁLISIS DE REQUISITOS** {#capítulo-ii:-recopilación-y-análisis-de-requisitos}

   1. ## **Entrevistas** {#entrevistas}

      1. ### Diseño de entrevistas {#diseño-de-entrevistas}

         **Segmento Objetivo 1: Gestores de Activos Comerciales e Industriales Ligeros (Pymes)**

         **Descripción del segmento**

         Gerentes de operaciones, administradores o dueños de pymes en Lima Metropolitana o provincias con instalaciones solares de mediana escala (10 kW a 50+ kW) bajo tarifas comerciales reguladas. Requieren trazabilidad estricta del autoconsumo frente a la red eléctrica y detección inmediata de fallas para evitar sobrecostos operativos.

         **Batería de preguntas**

         **Perfil Demográfico y Background:**

* ¿Cuál es su cargo actual, edad, profesión y en qué distrito opera la sede o planta de su empresa?

* ¿Cuál es el giro comercial de la empresa y cómo está estructurado su equipo operativo o de mantenimiento?

* ¿Podría detallar su trayectoria en la administración de estas instalaciones y cuántos años lleva operando con energía solar en su negocio?

  **Personalidad, Marcas e Influencias:**

* ¿Cómo definiría su estilo de gestión respecto al control de costos y la continuidad operativa (ej. preventivo, analítico, reactivo a reportes)?

* ¿Qué marcas de equipamiento solar (inversores, paneles) o referentes del sector energético utiliza o toma como estándar de confianza?

* ¿Qué plataformas de software de gestión industrial, monitoreo de energía o ERP utiliza habitualmente en su día a día? 

  **Tecnología, Dispositivos y Canales (Habilidades):**

* ¿A través de qué dispositivos (laptop corporativa, PC de escritorio, smartphone) consulta con mayor frecuencia las operaciones y consumos del negocio?

* ¿Qué canales digitales emplea internamente para coordinar órdenes de trabajo y reparaciones con técnicos o cuadrillas de campo?

* Del 1 al 10, ¿qué tan cómodo se siente su equipo al adoptar plataformas en la nube o herramientas de telemetría IoT?

  **Extracción de Requisitos para la Base de Datos (Pain Points, Entidades y Atributos):**

* Entidad Instalacion y Tarifa: ¿Qué datos exactos de su recibo eléctrico (tipo de tarifa ej. BT5A/BT5B, potencia contratada, distribuidora, costo unitario por kWh en Soles) necesita asociar a su instalación para auditar el ahorro real?  
* Entidades Medicion y Consumo: ¿Con qué periodicidad o intervalos horarios (ej. cada 15 min, horario punta/fuera de punta) requiere cruzar la generación solar frente a la demanda de su maquinaria para evitar desperdicio energético?  
* Entidades Incidencia, Alerta y Anomalia: Cuando ocurre una caída de tensión o fallo en un string completo, ¿qué información mínima necesita que guarde el sistema (panel afectado, pérdida económica estimada en Soles por hora, fecha/hora exacta)?  
* Entidades Mantenimiento, Tecnico, Repuesto y Costo: Al contratar una reparación o mantenimiento, ¿qué registros exige documentar (técnico responsable, horas de trabajo, repuestos sustituidos, número de orden y costo total)?

  **Segmento Objetivo 2: Familias Residenciales con Sistemas Solares Activos**

  **Descripción del segmento**

  Propietarios de viviendas unifamiliares en distritos con alta radiación o casas de playa/campo de Lima con kits solares de 3 kW a 10 kW. Se enfrentan a la acumulación de suciedad y polvo (soiling) y requieren monitoreo sencillo, traducción de métricas técnicas a dinero y coordinación confiable de mantenimiento.

  **Batería de preguntas**

  **Perfil Demográfico y Background:**

* ¿Podría indicarme su edad, distrito de residencia habitual y ocupación?   ¿Cómo está conformado su hogar y qué tipo de vivienda tiene (casa urbana, casa de campo, casa de playa)?

* ¿Cuánto tiempo lleva con su sistema solar instalado y cuántos paneles componen aproximadamente su techo fotovoltaico?

  **Personalidad, Marcas e Influencias:**

* ¿Cómo se describiría al momento de cuidar la economía y el mantenimiento de su hogar (ej. meticuloso, práctico, desinteresado hasta que algo falla)?

* ¿Qué marcas de tecnología para el hogar o instaladores solares locales le generan mayor confianza y reputación?

* ¿Qué aplicaciones de servicios públicos (banca, app de luz de Enel/Luz del Sur) consulta con regularidad?

  **Tecnología, Dispositivos y Canales (Habilidades):**

* ¿En qué dispositivo prefiere revisar el estado de su vivienda: smartphone personal, tablet o computadora familiar?

* ¿Qué canales digitales utiliza para comunicarse con el servicio técnico o proveedores de servicios del hogar (WhatsApp, llamadas, formularios web)?

* Del 1 al 10, ¿qué tan comprensible le resulta la interfaz de la aplicación actual que le entregó la empresa instaladora? 

  **Extracción de Requisitos para la Base de Datos (Pain Points, Entidades y Atributos):**

* Entidades Medicion y Ahorro: En lugar de kilovatios o amperios, ¿qué campos comprensibles necesita ver registrados en su historial (soles ahorrados al mes, porcentaje de energía propia consumida, CO2 evitado)?

* Entidades Alerta y Anomalia: Si un panel baja su producción por polvo, suciedad o sombra, ¿qué descripción en lenguaje no técnico espera que guarde la alerta (ej. mensaje descriptivo, nivel de severidad, recomendación de limpieza)?

* Entidades Mantenimiento y Tecnico: Al solicitar un servicio de limpieza de paneles, ¿qué datos del técnico y de la visita le resulta indispensable registrar para su seguridad (nombre, empresa instaladora, calificación/reseñas, fecha y costo del servicio)?   


  **Segmento Objetivo 3: Hogares en Transición Energética (Compradores Potenciales)**

  **Descripción del segmento**

  Jefes de hogar de Lima interesados en migrar a energía solar para reducir sus recibos de luz, pero detenidos por la falta de transparencia en costos, dimensionamiento y rentabilidad real en su distrito.

  **Batería de preguntas**

  **Perfil Demográfico y Background:**

* ¿Cuál es su edad, distrito de residencia y número de miembros que habitan en la vivienda?

* ¿Qué tipo de propiedad tiene (casa propia, departamento, casa campestre) y qué área de techo dispone aproximadamente?

* ¿Cuál es el promedio mensual que paga en su recibo de electricidad actualmente?

  **Personalidad, Marcas e Influencias:**

* ¿Qué factores pesan más en su proceso de compra de tecnología para el hogar: el ahorro económico, la sostenibilidad ambiental o la reputación de la marca?

* ¿En qué tiendas o canales suele buscar referencias de equipamiento para el hogar (Promart, Sodimac, distribuidores técnicos, recomendaciones de conocidos)?

  **Tecnología, Dispositivos y Canales (Habilidades):**

* ¿Qué dispositivos utiliza prioritariamente cuando investiga productos de alto valor antes de comprarlos?

* ¿Qué medios digitales prefiere utilizar para recibir cotizaciones o diagnósticos técnicos (WhatsApp, correo electrónico, cotizadores interactivos en web)?

* Del 1 al 10, ¿qué tan dispuesto está a utilizar un simulador digital interactivo para calcular su consumo de energía?   

  **Extracción de Requisitos para la Base de Datos (Pain Points, Entidades y Atributos):**

* Entidades Consumo\_Historico y Simulacion: Para calcular cuántos paneles necesita, ¿qué variables de su consumo estaría dispuesto a registrar (consumo en kWh de los últimos meses, inventario de electrodomésticos de alto consumo, horarios de permanencia en casa)?

* Entidad Catalogo\_Panel: Al evaluar modelos de paneles en un catálogo, ¿qué atributos técnicos considera indispensables para comparar opciones (marca, potencia nominal en Watts, años de garantía, costo unitario, eficiencia de degradación)?

* Entidades Factor\_Emision y Presupuesto: ¿Qué indicadores de impacto ambiental desearía ver reflejados en el cálculo final (árboles equivalentes, reducción estimada de huella de carbono, tiempo estimado de retorno de inversión en meses/años)?

  2. ### Registro de entrevistas {#registro-de-entrevistas}

       
* **Segmento Objetivo 1: Gestores de Activos Comerciales e Industriales Ligeros (Pymes)**

  **Entrevista 1:**

| Nº Registro | Datos del Entrevistado: | Screenshot  |
| :---- | :---- | :---- |
| 1 | URL:[https\://youtu.be/FVRP54Lk8DQ](https://youtu.be/FVRP54Lk8DQ)  Nombre y Apellidos: Elias CoronelEdad: 26Distrito: San Borja Ocupación: Ingeniero Industrial |  |

   **Resumen:**

  El entrevistado es un administrador de operaciones de 26 años, ingeniero industrial, que trabaja en una empresa ubicada en Villa El Salvador y tiene aproximadamente 3 años de experiencia trabajando con energía solar. Se caracteriza por tener un enfoque preventivo y analítico, buscando evitar fallas que puedan afectar la producción.

  Actualmente utiliza ERP, Excel y la plataforma del inversor, además de WhatsApp y correo para coordinar mantenimientos. Considera importante contar con información centralizada sobre consumo, generación solar, tarifas, incidencias, pérdidas económicas y mantenimientos. También considera útil recibir alertas sobre fallas y conocer el historial de técnicos, repuestos y costos.


  


  


  


  


* **Segmento Objetivo 2: Familias Residenciales con Sistemas Solares Activos**


  **Entrevista 1:**

| Nº Registro | Datos del Entrevistado: | Screenshot  |
| :---- | :---- | :---- |
| 1 | URL:[https\://youtu.be/lwn3OLEs3s8](https://youtu.be/lwn3OLEs3s8)  Nombre y Apellidos: Adriana SalazarEdad: 24Distrito: La Molina Ocupación: Ingeniera Civil |  |

   **Resumen:**

  La entrevistada es una mujer de 24 años, ingeniera civil, que vive en La Molina con su familia. Su vivienda cuenta con aproximadamente 12 paneles solares y una capacidad de 4 kW, instalados hace unos dos años.

  Se considera una persona práctica y cuidadosa con los gastos del hogar, además de interesarse por el mantenimiento preventivo. Utiliza principalmente su smartphone para revisar el sistema y prefiere comunicarse con los técnicos mediante WhatsApp. Considera que la aplicación actual es relativamente comprensible, pero algunos datos técnicos son difíciles de interpretar.

  Sus principales intereses son conocer cuánto dinero ahorra, cuánto consume de energía solar y cuándo existe algún problema con los paneles. Prefiere recibir alertas en lenguaje sencillo, indicando el problema, su gravedad y qué acción debería realizar. También considera importante conocer los datos del técnico, empresa, reseñas, fecha y costo del mantenimiento.


  


  


  





* **Segmento Objetivo 3: Hogares en Transición Energética (Compradores Potenciales)**

  **Entrevista 1:**

| Nº Registro | Datos del Entrevistado: | Screenshot  |
| :---- | :---- | :---- |
| 1 | URL: Nombre y Apellidos:Edad:Distrito:  Ocupación: |  |

   **Resumen:**


  


  

  3. ### Análisis de entrevistas {#análisis-de-entrevistas}

     \*\* En Desarrollo

  2. ## **Requisitos** {#requisitos}

### **Requisitos funcionales** {#requisitos-funcionales}

| REQUISITOS FUNCIONALES |  |  |
| ----- | ----- | :---: |
| **Código** | **Descripción** | **Entidad Directa Relacionada** |
| US-01 | Registrar y gestionar los usuarios de la plataforma de acuerdo con su rol. | Usuario, Rol |
| US-02 | Registrar y gestionar las instalaciones fotovoltaicas. | Instalación |
| US-03 | Registrar los paneles solares asociados a una instalación fotovoltaica. | Panel Solar |
| US-04 | Registrar sensores IoT asociados a los paneles solares. | Sensor IoT |
| US-05 | Registrar las mediciones obtenidas por los sensores (Voltaje, corriente, temperatura). | Medición |
| US-06 | Identificar posibles anomalías a partir de las mediciones registradas. | Anomalía |
| US-07 | Identificar posibles anomalías a partir de las mediciones registradas. | Anomalía |
| US-08 | Generar alertas cuando se detecten condiciones anormales en paneles o instalaciones. | Alerta |
| US-09 | Registrar y gestionar las incidencias detectadas en paneles solares. | Incidencia |
| US-10 | Generar órdenes de mantenimiento asociadas a una incidencia.  | Orden de mantenimiento |
| US-11 | Asignar órdenes de mantenimiento a técnicos responsables. | Orden de mantenimiento, Técnico |
| US-12 | Registrar las actividades realizadas durante una intervención de mantenimiento. | Activador de mantenimiento |
| US-13 | Registrar los repuestos utilizados durante la actividad de mantenimiento | Repuesto, Detalle de presupuesto |
| US-14 | Registrar los costos relacionados con actividades de mantenimiento y repuestos utilizados. | Costo mantenimiento |
| US-15 | Consultar el historial de mantenimientos realizados sobre una instalación o panel. | Instalación, Panel Solar, Orden de mantenimiento, Activador de mantenimiento |

### 

### **Requisitos No funcionales** {#requisitos-no-funcionales}

| REQUISITOS FUNCIONALES |  |  |
| ----- | ----- | :---: |
| **Código** | **Descripción** | **Propósito** |
| RNF-1 | Validar credenciales y permisos por rol en un tiempo máximo de 1.5 segundos, bloqueando el acceso al tercer intento fallido continuo  | Seguridad |
| RNF-2 | Ejecutar validaciones de integridad referencial y comprobación de esquemas en menos de 2 segundos por cada lote de mediciones entrantes. | Integridad |
| RNF-3 | Ingerir y persistir de manera continua más de 1,000 registros por segundo de telemetría sin degradar el rendimiento de lectura. | Escalabilidad |
| RNF-4 | Admitir un incremento anual del 100% en el volumen de almacenamiento de lecturas históricas manteniendo tiempos de consulta estables mediante particionamiento temporal. | Escalabilidad |
| RNF-5 | Retornar métricas analíticas agregadas (por día, mes o año) en menos de 3 segundos para tableros de control con más de 100 paneles. | Rendimiento |
| RNF-6 | Transformar y registrar cargas de telemetría de sensores IoT multimarca en menos de 5 segundos por trama entrante. | Interoperabilidad |
| RNF-7 | Recuperar la base de datos a su último estado consistente en un lapso máximo de 2 horas (RTO) ante fallos críticos del sistema gestor. | Recuperabilidad |
| RNF-8 | Mantener la operatividad de los servicios de lectura y persistencia durante al menos el 99.5% del tiempo anual. | Disponibilidad |
| RNF-9 | Registrar y enlazar automáticamente el identificador de la anomalía, la alerta y la incidencia técnica generada en no más de 2 segundos. | Trazabilidad |
| RNF-10 | Documentar en la base de datos el historial secuencial de intervenciones (orden de trabajo, técnico asignado, tareas y repuestos utilizados) en un tiempo menor a 3 segundos por evento. | Trazabilidad |

3. # **CAPÍTULO III: DISEÑO DE BASE DE DATOS** {#capítulo-iii:-diseño-de-base-de-datos}

   1. ## **Entidades** {#entidades}

      Realizamos el diseño de entidades para armas nuestras tablas necesarias y comenzar nuestro diagrama según los datos obtenidos de nuestros usuarios entrevistas y adaptando algunas tablas fundamentales que son pertinentes para el sistema.

      

| Usuario | Es necesaria para identificar a las personas que utilizan la plataforma y gestionar su acceso según el rol que desempeñen dentro de SolarPulse IoT. |
| :---- | :---- |
| Rol | Es importante para diferenciar los tipos de usuarios y controlar el acceso a la información y funcionalidades de acuerdo con los permisos asignados. |
| Instalación | Es fundamental porque representa el sistema fotovoltaico que será monitoreado por la plataforma. Permite centralizar la información relacionada con cada instalación solar. |
| Panel Solar | Es necesaria para identificar y controlar individualmente cada panel de una instalación, permitiendo detectar problemas específicos y conocer su rendimiento. |
| Sensor IoT | Es fundamental para obtener los datos provenientes de los paneles solares, permitiendo realizar el monitoreo de variables como voltaje, corriente y temperatura. |
| Medición | Es necesaria para almacenar los datos obtenidos por los sensores a lo largo del tiempo y permitir el análisis del comportamiento de los paneles. |
| Anomalía | Permite registrar las condiciones anormales detectadas a partir de las mediciones, facilitando la identificación temprana de posibles problemas. |
| Alerta | Es necesaria para comunicar oportunamente al usuario la detección de una condición anómala en un panel o instalación. |
| Incidencia | Permite registrar y realizar seguimiento a los problemas detectados que requieren una intervención o solución técnica. |
| Orden mantenimiento | Es necesaria para organizar y gestionar las actividades que deben realizarse para solucionar una incidencia detectada. |
| Tecnico | Permite identificar al responsable de realizar las intervenciones de mantenimiento y mantener trazabilidad sobre quién ejecutó cada trabajo. |
| Actividad mantenimiento | Es necesaria para registrar las acciones realizadas durante una intervención y conservar el historial de mantenimiento de la instalación o panel. |
| Repuesto | Permite controlar los componentes utilizados durante las actividades de mantenimiento y llevar un registro de los recursos empleados. |
| Detalle presupuesto | Es necesario registrar específicamente los repuestos utilizados en cada actividad de mantenimiento y relacionarlos con el trabajo realizado. |
| Cliente | Es necesaria para representar a las personas naturales o jurídicas propietarias de las instalaciones fotovoltaicas y gestionar su información fiscal y de contacto. |
| Costo mantenimiento | Permite registrar y controlar los costos asociados a las actividades de mantenimiento y a los repuestos utilizados, facilitando la trazabilidad económica. |

      

   2. ## **Atributos** {#atributos}

Los atributos definidos a continuación no han sido concebidos de manera aislada, sino que emergen del análisis exhaustivo y la síntesis de las necesidades detectadas en las entrevistas aplicadas a cada uno de nuestros segmentos objetivo (gestores comerciales, familias residenciales y evaluadores en transición energética). Cada campo ha sido rigurosamente seleccionado para responder a dolores específicos expresados por los usuarios “como la necesidad de auditar ahorros en soles, interpretar alertas en lenguaje no técnico, trazar costos de mantenimiento y supervisar la telemetría en tiempo real”. Este levantamiento de información garantiza que la estructura de datos sea 100% representativa de la operación real, sirviendo como base sólida y validada para la construcción del diagrama de entidad-relación lógico y la posterior implementación del sistema.

| Usuario |  |
| ----- | ----- |
| Atributos | Descripción |
| id\_usuario  | Identificador único.  |
| id\_rol  | Clave foránea que define los permisos y nivel de acceso  |
| nombre\_completo  | Nombre y apellidos del usuario.  |
| email  | Correo electrónico institucional o personal (usado para login y notificaciones).  |
| password | la contraseña.  |
| telefono  | Número de contacto para avisos de emergencia.  |
| estado  | Estado de la cuenta (activo, suspendido, inactivo).  |

| Rol  |  |
| ----- | ----- |
| Atributos | Descripción |
| id\_rol  | Identificador único del rol.  |
| nombre\_rol  | Nombre del rol  |
| descripcion  | Detalle del alcance y responsabilidades del perfil.  |
| permisos  | Conjunto o matriz de permisos del sistema (lectura, escritura, asignación de órdenes, etc.).  |

| Cliente |  |
| ----- | ----- |
| Atributos | Descripción |
| id\_cliente | Identificador único del cliente. |
| razon\_social | Nombre o razón social de la persona natural o jurídica propietaria. |
| ruc | Número de Registro Único de Contribuyente o documento de identidad. |
| direccion\_fiscal | Dirección del domicilio fiscal o legal del cliente. |
| telefono\_contacto | Número telefónico principal de contacto. |
| email\_contacto | Correo electrónico corporativo o personal para facturación y avisos. |

| Instalación  |  |
| ----- | ----- |
| Atributos | Descripción |
| id\_instalacion  | Identificador único de la instalación.  |
| nombre  | Nombre descriptivo de la planta o sede.  |
| id\_cliente  | Referencia al usuario o empresa propietaria.  |
| ubicacion\_lat | Coordenadas GPS (latitud, longitud) y dirección física.  |
| ubicacion\_long | Coordenadas GPS (latitud, longitud) y dirección física.  |
| direccion | ubicacion en calles  |
| capacidad\_nominal\_kw  | Potencia pico teórica total diseñada para la instalación (kWp).  |
| fecha\_puesta\_marcha  | Fecha de inicio de operaciones.  |
| estado\_operativo  | Estado general (operativa, en mantenimiento parcial, fuera de servicio).  |

| Panel Solar  |  |
| ----- | ----- |
| Atributos | Descripción |
| id\_panel  | Identificador único del panel.  |
| id\_instalacion  | Instalación a la que pertenece.  |
| codigo\_serie  | Número de serie del fabricante.  |
| marca\_modelo  | Fabricante y modelo técnico  |
| potencia\_nominal\_w  | Potencia nominal de diseño en vatios (Wp).  |
| angulo\_inclinacion  | Configuración física de montaje (azimut e inclinación).  |
| orientacion | orientacion(Norte,sur,este,oeeste) |
| estado  | Condición actual (óptimo, degradado, dañado, desconectado).  |

| Sensor IoT  |  |
| ----- | ----- |
| Atributos | Descripción |
| id\_sensor  | Identificador único del sensor.  |
| id\_panel  | Panel o inversor específico al que está acoplado (si aplica).  |
| id\_instalacion  | Instalación en la que opera.  |
| identificador\_hardware  | Identificador físico de red o dispositivo.  |
| tipo\_sensor  | Variable principal medida (corriente/voltaje DC, temperatura de celda, irradiancia solar, ambiental).  |
| mac\_address | identificador único  |
| frecuencia\_muestreo\_seg  | Intervalo de tiempo configurado entre cada telemetría.  |
| estado\_conexion  | Estado de conectividad (online, offline, batería baja).  |

| Medición  |  |
| ----- | ----- |
| Atributos | Descripción |
| id\_medicion  | Identificador único del registro de telemetría.  |
| id\_sensor  | Sensor emisor de la lectura.  |
| timestamp\_registro | Fecha, hora exacta y zona horaria de la captura.  |
| voltaje\_v  | Tensión eléctrica registrada.  |
| corriente\_a  | Intensidad de corriente registrada.  |
| potencia\_calculada\_w  | Potencia instantánea calculada |
| temperatura\_celda\_c  | Temperatura medida en la superficie del panel.  |
| irradiancia\_w\_m2  | Nivel de radiación solar capturada en el momento.  |

| Anomalía  |  |
| ----- | ----- |
| Atributos | Descripción |
| id\_anomalia  | Identificador único de la anomalía.  |
| id\_panel  | Componente donde se detectó el comportamiento inusual.  |
| id\_sensor | id del sensor |
| fecha\_deteccion  | Momento exacto en que el algoritmo o regla la identificó.  |
| tipo\_anomalia  | Categoría del fallo (hotspot, sombreado constante, degradación acelerada, circuito abierto).  |
| valor\_esperado  | Métricas de comparación para auditoría.  |
| valor\_leido  | Métricas de comparación para auditoría.  |
| severidad  | Nivel de criticidad (baja, media, alta, crítica).  |

| Alerta  |  |
| ----- | ----- |
| Atributos | Descripción |
| id\_alerta  | Identificador único de la alerta.  |
| id\_anomalia  | Anomalía que originó la alerta (si fue gatillada automáticamente).  |
| id\_instalacion  | Instalación afectada.  |
| fecha\_generacion  | Fecha y hora de emisión.  |
| mensaje  | Texto claro describiendo la advertencia.  |
| canal\_envio  | Vía de notificación empleada (SMS, correo, webhook, push).  |
| estado  | Ciclo de vida del aviso (no leída, atendida, silenciada).  |

| Incidencia  |  |
| ----- | ----- |
| Atributos | Descripción |
| id\_incidencia  | Identificador único de la incidencia (ticket).  |
| id\_alerta  | Alerta previa que derivó en la incidencia (opcional).  |
| id\_instalacion  | Instalación impactada.  |
| titulo  | : Resumen conciso del problema.  |
| descripcion\_detallada  | Contexto técnico de la falla reportada.  |
| prioridad  | Urgencia de resolución (baja, media, alta, urgente).  |
| estado  | Flujo de trabajo (abierta, en diagnóstico, en mantenimiento, resuelta, cerrada).  |
| fecha\_apertura  | Marcas de tiempo del ciclo de vida del ticket.  |
| fecha\_cierre  | Marcas de tiempo del ciclo de vida del ticket.  |

| Orden de Mantenimiento  |  |
| ----- | ----- |
| Atributos | Descripción |
| id\_orden  | Identificador único de la orden de trabajo (OT).  |
| id\_incidencia  | Incidencia asociada (si es correctivo).  |
| id\_instalacion  | Ubicación donde se efectuará el trabajo.  |
| tipo\_mantenimiento  | Clasificación del trabajo (preventivo, correctivo, predictivo/limpieza).  |
| fecha\_programada  | Fecha estimada para la ejecución.  |
| fecha\_ejecucion  | Fecha real de intervención.  |
| estado  | Estado de la OT (pendiente, asignada, en progreso, completada, cancelada).  |

| Técnico  |  |
| ----- | ----- |
| Atributos | Descripción |
| id\_tecnico  | Identificador único del técnico.  |
| id\_usuario  | Vínculo con la entidad Usuario para login y credenciales.  |
| codigo\_empleado  | Acreditación profesional o certificación técnica.  |
| especialidad  | Área de dominio (alta tensión, montaje mecánico, redes IoT, instrumentación).  |
| disponibilidad  | Estado laboral actual (disponible, en ruta, en servicio, de baja).  |

| Actividad de Mantenimiento  |  |
| ----- | ----- |
| Atributos | Descripción |
| id\_actividad  | Identificador único de la tarea.  |
| id\_orden  | Orden de mantenimiento a la que pertenece.  |
| id\_tecnico  | Técnico responsable de ejecutar la tarea.  |
| descripcion\_tarea  | Procedimiento específico realizado.  |
| tiempo\_estimado\_min  | Duración de la actividad para control de horas hombre.  |
| tiempo\_real\_min  | Duración de la actividad para control de horas hombre.  |
| resultado  | Resultado de la acción (exitosa, incompleta, requiere segunda visita).  |
| observaciones  | Comentarios técnicos adicionales o hallazgos secundarios.  |

| Repuesto  |  |
| ----- | ----- |
| Atributos | Descripción |
| id\_repuesto  | Identificador único del componente.  |
| codigo\_sku  | Código de inventario o catálogo del fabricante.  |
| nombre  | Denominación del repuesto (ej. fusible DC 15A, cable solar 4mm², conector MC4).  |
| stock\_actual  | Cantidad de unidades disponibles en bodega.  |
| costo\_unitario\_estandar  | Valor unitario monetario del ítem.  |

| Detalle de Presupuesto  |  |
| ----- | ----- |
| Atributos | Descripción |
| id\_detalle\_presupuesto  | Identificador de la partida o renglón.  |
| id\_orden  | Orden de trabajo a la que se cotiza.  |
| id\_repuesto  | Repuesto cotizado (nullable si es mano de obra o servicio).  |
| concepto  | Descripción del ítem presupuestado (ej. "Reemplazo de conectores MC4")  |
| cantidad  | Unidades o número de horas cotizadas.  |
| precio\_unitario  | Tarifa aplicada por unidad.  |
| subtotal  | Total calculado ($cantidad\times precio\_unitario$).  |

| Costo Mantenimiento  |  |
| ----- | ----- |
| Atributos | Descripción |
| id\_costo\_mantenimiento  | Identificador del cierre contable de la orden.  |
| id\_orden  | Orden de trabajo liquidada.  |
| costo\_mano\_obra  | Suma acumulada de las horas hombre de los técnicos.  |
| costo\_materiales\_repuestos  | Gasto real en piezas y consumibles utilizados  |
| costo\_adicional\_viaticos  | Gastos por traslado, grúas o equipamiento de seguridad.  |
| costo\_total  | Suma total monetaria liquidada para la orden.  |
| moneda  | Código monetario de facturación (USD, PEN, EUR, etc.).  |
| fecha\_registro\_costo  | Fecha en que se cerró y aprobó la liquidación.  |

En conclusión, la selección de atributos para cada entidad responde de forma directa a las necesidades identificadas en las entrevistas de cada segmento objetivo. Esta estructura no solo garantiza la captura de datos clave para la gestión técnica y económica, sino que también asegura la consistencia y solidez necesarias para el desarrollo del modelo lógico.

3. ## **Enfoque relacional** {#enfoque-relacional}

   El diagrama entidad-relación conceptual utiliza la notación de Chen para representar de manera clara y visual las entidades, atributos y relaciones derivadas de las entrevistas. Se eligió esta notación debido a su alta claridad conceptual y su énfasis en los atributos y la naturaleza de las relaciones binarias y numéricas, lo que facilita la comprensión inicial del modelo antes de pasar al diseño lógico y físico.  
     
      
     
   

   1. ### Diagrama entidad-relación lógico  {#diagrama-entidad-relación-lógico}

      El diagrama de entidad-relación lógico constituye la representación estructurada de la arquitectura de datos del sistema SolarPulse IoT. En esta etapa, el modelo integra detalladamente los atributos identificados y definidos previamente (tales como datos de identificación personal, credenciales, correos electrónicos y parámetros operativos técnicos entre otros), estableciendo las claves primarias y foráneas que formalizan las dependencias y tipos de relación entre cada entidad. Esta especificación lógica permite validar la coherencia conceptual de la información antes de proceder con el diseño e implementación de la base de datos a nivel físico.  
      

4. # **CAPÍTULO IV: IMPLEMENTACIÓN DE BASE DE DATOS** {#capítulo-iv:-implementación-de-base-de-datos}

   1. ## **Sistemas de gestión de base de datos** {#sistemas-de-gestión-de-base-de-datos}

      1. ### Evaluación y elección del sistema de gestión de base de datos relacional {#evaluación-y-elección-del-sistema-de-gestión-de-base-de-datos-relacional}

         \*\*En Desarrollo

   2. ## **Diagramas de datos** {#diagramas-de-datos}

      1. ### Diagrama entidad-relación físico {#diagrama-entidad-relación-físico}

         \*\*En Desarrollo

# **CONCLUSIONES** {#conclusiones}

# **BIBLIOGRAFÍA** {#bibliografía}

- Wiley Online Library. (2025). Intelligent maintenance approaches for improving photovoltaic performance. *Solar RRL*. [https\://onlinelibrary.wiley.com/doi/full/10.1002/solr.202500289](https://onlinelibrary.wiley.com/doi/full/10.1002/solr.202500289)  
- SurgePV. (2026, mayo 3). *Predictive maintenance solar 2026: AI, IoT & cost reduction*. [https\://www\.surgepv.com/blog/predictive-maintenance-solar](https://www.surgepv.com/blog/predictive-maintenance-solar)  
- IEOM Society. (2025). A hybrid cost-optimized maintenance strategy for solar-wind systems. *Proceedings of the International Conference on Industrial Engineering and Operations Management*, París. [https\://ieomsociety.org/proceedings/paris2025/374.pdf](https://ieomsociety.org/proceedings/paris2025/374.pdf)   
- DataIntelo. (2025). *Solar performance monitoring market research report 2033*. [https\://dataintelo.com/report/solar-performance-monitoring-market](https://dataintelo.com/report/solar-performance-monitoring-market)

  # **ANEXOS** {#anexos}

* **Anexo 1\. Fuente sobre tecnología y gestión de activos de energía renovable**  
  Visualización del sistema para probar un demo directo correspondiente al sistema de gestión de energía renovable que ya existen.  
    
* **Anexo 2\. Registro del contenido audiovisual creados o implementados en el proyecto**

| Sección | Características del video | Sobre el contenido | Integración y entrega |
| :---: | ----- | ----- | ----- |
| Entrevistas | **Cantidad de videos:** 6 **Nomenclatura:** upc-pre-202610-1asi0787-15869-Heliosync\_Technologie-needfinding-TP1 **Formato:** .mp4 **Duración:** En función a cantidad de entrevistas (considerar edición de 3 a 5 minutos por entrevista).   | Lorem Ipsum | Subir el video en YouTube con enlace privado. Incluir en el informe screenshot del video con enlace al mismo. Incluir redacción de introducción a la sección y análisis de cada entrevista, así como el análisis general donde se identifican las variables y los valores representativos a nivel objetivo y subjetivo que servirán de base para la definición de los User Persona  |
| About the team | **Cantidad de videos:** 1 **Nomenclatura:** upc-pre-202610-1asi0787-15869-Heliosync\_Technologie-needfinding-TP1 **Formato:** .mp4 **Duración:** En función al contenido (considerar 5 minutos para la sección de retrospectiva del grupo y 1 minuto por cada testimonio de miembro del equipo).   | Lorem Ipsum | Subir el video en YouTube con enlace privado. Incluir redacción de introducción a la sección, resumiendo el proceso de trabajo y los logros alcanzados por los miembros del equipo  |
| Expo TP1 | **Cantidad de videos:** 1 **Nomenclatura:** upc-pre-202610-1asi0787-15869-Heliosync\_Technologie-needfinding-TP1 **Formato:** .mp4 **Duración:** La duración máxima del video es de 20 minutos. | Lorem Ipsum | Subir el video en YouTube con enlace privado.  |


  

[image1]: <data:image/png;base64,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>