# Capítulo II: Requirements Elicitation & Analysis

## 2.1. Competidores
El ecosistema de soluciones tecnológicas aplicadas a la gestión de recursos hídricos a nivel global presenta un grado de maduración significativo. Sin embargo, una revisión crítica del mercado evidencia que la oferta de software e Internet de las Cosas (IoT) orientada a la economía circular hídrica en América Latina, particularmente en el Perú, se encuentra desatendida. Según el Banco Mundial (2025), el país requiere de una transformación infraestructural en sus métodos de saneamiento, destinando un programa de inversión de $200 millones para fomentar la transición hacia una economía circular que las soluciones actuales no son capaces  de consolidar.

 Las plataformas internacionales dominantes tienden a enfocarse en infraestructuras de países desarrollados, omitiendo las realidades logísticas, además de los marcos regulatorios locales estipulados por entidades como la Autoridad Nacional del Agua (ANA) junto con el Organismo de Evaluación y Fiscalización Ambiental (OEFA). Dicha desconexión tecnológica se traduce como una brecha de eficiencia crítica: según plantea la SUNASS (2025), el Perú necesita invertir una cantidad de 138,000 millones de soles en los próximos 30 años para cerrar la brecha de saneamiento, una cifra difícil de alcanzar empleando métodos tradicionales sin la adquisición y adopción de tecnologías de monitoreo de bajo costo y alta precisión.
Para una Empresa Prestadora de Servicios (EPS) o una operadora de residuos sólidos en el país, esta brecha significa que no existe un competidor directo, accesible, que cubra sus necesidades de extremo a extremo: desde la detección de anomalías químicas en tiempo real hasta la logística de redistribución para el reúso del agua. Por consiguiente, se han seleccionado para este análisis a tres competidores representativos (dos directos a nivel global sumados a uno indirecto corporativo), con el objetivo de demostrar cómo la arquitectura, combinada con el modelo de negocio de WebWarriors, ataca sus debilidades en el mercado peruano:

#### 1.	Kando (Competencia Directa en Capa Transaccional Analítica):
 ○	 **Perfil:** Empresa tecnológica global enfocada en la gestión de la calidad de aguas residuales mediante IoT, apoyada en el análisis de datos en la nube bajo el modelo Software as a Service (SaaS).

○	**Debilidad frente a nuestro nicho:** Es una solución de alto costo diseñada principalmente para "utility companies" norteamericanas al igual que europeas. Carece de un módulo logístico para la redistribución del agua recuperada, limitándose a la detección, sin lograr el cierre del ciclo de economía circular requerido en zonas de estrés hídrico.
#### 2.	SmartCover Systems (Competencia Directa en Capa de Infraestructura Física):
○	 **Perfil:** Proveedor especializado en el monitoreo remoto de sistemas de recolección de aguas residuales, enfocado en la prevención de desbordes (SSO) mediante sensores acústicos, así como satelitales.

○	**Debilidad frente a nuestro nicho:** Su enfoque es estrictamente volumétrico, orientado a la prevención de derrames. No realiza analítica química profunda (como variaciones críticas de pH) ni detección de gases tóxicos, variables fundamentales para habilitar el reúso del agua residual (ANA, 2026).
#### 3.	Veolia - Hubgrade (Competencia Indirecta en Capa Corporativa Integral):
○	**Perfil:** Gigante corporativo de servicios medioambientales que cuenta con "Hubgrade", una plataforma digital para el monitoreo, auditoría, además de optimización de recursos hídricos mediante gemelos digitales (digital twins).

○	**Debilidad frente a nuestro nicho:** Opera mediante proyectos multimillonarios "llave en mano". La barrera financiera, sumada a la rigidez burocrática de su implementación, resulta restrictiva e incluso prohibitiva para el grueso de municipalidades, al igual que operadoras medianas en el mercado peruano.


### 2.1.1. Análisis competitivo
### 2.1.2. Estrategias y tacticas frente a competidores
Al momento de ingresar a un mercado caracterizado por infraestructuras heredadas junto a monopolios tecnológicos internacionales, la startup debe adoptarse a un pragmatismo estratégico. La viabilidad  del negocio no solo reside en competir en fuerza bruta de capital con corporaciones como Veolia, sino que se busca capturar un nicho crítico para resolver fricciones regulatorias, además de logísticas, que varios competidores globales ignoran.

A continuación, se detallan las estrategias operativas junto a las tácticas arquitectónicas que guiarán la construcción al igual que el despliegue del producto:

**1. Estrategia de Localización con Mitigación de Riesgos Normativos (Posicionamiento frente a Kando o Veolia)**
- 	**Objetivo Estratégico:** Diferenciarse radicalmente de las plataformas genéricas extranjeras, consolidando el software como una herramienta nativa de cumplimiento regulatorio, sirviendo como protección financiera para las empresas locales.

- **Táctica Ejecutable:** La arquitectura de la base de datos, operando en conjunto con el motor de alertas, se parametrizará rígidamente bajo los estándares exigidos por las autoridades nacionales. El sistema evaluará en tiempo real el pH junto a la emisión de gases tóxicos. Si los parámetros se acercan a los límites permisibles sancionables (los cuales pueden           desencadenar multas superiores a los S/ 128 millones, según el OEFA), el sistema generará bloqueos preventivos, emitiendo     reportes automatizados en el formato exacto requerido por los fiscalizadores (OEFA, 2024).

**2. Estrategia de Océano Azul: Cierre de la Cadena de Valor (Posicionamiento frente a SmartCover)**

- **Objetivo Estratégico:** Trascender la simple capa de telemetría e infraestructura de monitoreo, integrando la gestión comercial junto a la logística, habilitando la economía circular en el sector hídrico.

- **Táctica Ejecutable:** Mientras la competencia detecta un flujo de agua para luego emitir una alerta, la plataforma integrará un "Módulo de Logística de Redistribución". Al detectar que un volumen de agua residual cumple con los parámetros químicos para su reúso (conforme a los lineamientos de la ANA, 2026), el sistema no solo alertará a la planta, sino que orquestará la disponibilidad de este recurso en la plataforma, permitiendo su asignación junto a su transporte hacia sectores de alto déficit hídrico, transformando un desecho en un activo logístico.

**3. Estrategia Land and Expand mediante Reducción de Barreras CAPEX**

- **Objetivo Estratégico:** Vencer la resistencia financiera de las empresas estatales al igual que operadoras medianas que no pueden asumir los costos de implementación de licencias de competidores como Veolia.

- **Táctica Ejecutable:** El modelo de comercialización se ejecutará bajo un esquema de Software as a Service (SaaS), sustituyendo fuertes inversiones de capital (CAPEX) por gastos operativos manejables (OPEX). El ingreso inicial a la organización cliente se realizará a través de un piloto controlado en nodos críticos de la red de alcantarillado, demostrando empíricamente la reducción de los costos operativos (despliegue de cuadrillas de emergencia) como mecanismo de conversión hacia la adopción total del ecosistema de sensores.

**4. Estrategia de Cero Fricción en la Interfaz Operativa (UI/UX)**
  
- **Objetivo Estratégico:** Garantizar la adopción de la herramienta por parte del personal de campo al igual que operarios, mitigando el rechazo que generan los complejos tableros de control diseñados por la competencia exclusivamente para ingenieros de datos.

- **Táctica Ejecutable:** La interfaz de usuario (Front-end) se dividirá metodológicamente. El Back-Office web proveerá la densidad analítica requerida por la gerencia, mientras que el módulo para operadores de campo se construirá bajo principios de Mobile-First. Esta interfaz emitirá notificaciones Push asíncronas, directas, además de accionables, requiriendo un esfuerzo cognitivo mínimo para confirmar la atención de una obstrucción o riesgo biológico en tiempo real.


