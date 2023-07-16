# Proyecto_Individual_2 - Henry-DSPT01

Este es el segundo proyecto Individual de Henry DS PT 01 - Adriana Gabriela López Guerra

<img src="../imagenes/dis1.png" alt="Logo">


# Análisis de Datos - Proyecto Individual

Este proyecto tiene como objetivo realizar un análisis exhaustivo de los datos sobre el acceso a Internet en la República Argentina utilizando los conjuntos de datos disponibles en el sitio web del ENACOM. El objetivo principal es proponer una serie de indicadores clave de rendimiento (KPI) de interés para una empresa consultora (prestadora de servicios de telecomunicaciones) que busca instalarse en el territorio argentino. Para lograr esto, se seguirán una serie de pasos que incluyen el proceso de Extracción, Transformación y Carga (ETL) para limpiar los conjuntos de datos seleccionados, así como un análisis exploratorio de datos (EDA) para identificar relaciones, detectar valores atípicos y datos anómalos. Estos pasos nos ayudarán a obtener una visión más clara de la situación actual del acceso a Internet en el país y a generar recomendaciones informadas para mejorar la conectividad de los hogares.

## Contexto del proyecto

Las telecomunicaciones desempeñan un papel fundamental en nuestra sociedad, ya que permiten la transmisión de información a través de diversos medios electrónicos como la telefonía, la televisión, la radio y el internet. En particular, el internet ha revolucionado la forma en que nos comunicamos, trabajamos, aprendemos y nos entretenemos al proporcionar una red global de computadoras interconectadas.

En un mundo cada vez más conectado, las telecomunicaciones son esenciales para mantenernos informados y en contacto, incluso en situaciones de pandemia como la que enfrentamos actualmente. El intercambio de datos y la comunicación se realizan principalmente a través de internet, líneas telefónicas fijas y telefonía móvil, brindando acceso a la información y la posibilidad de conectarse con personas de todo el mundo.

En este contexto, Argentina se destaca en el desarrollo de las telecomunicaciones, con un total de 62,12 millones de conexiones para el año 2020. Esta cifra demuestra el alcance y la importancia de las comunicaciones en el país, permitiendo que sus habitantes estén conectados y accedan a los beneficios de la era digital.

A medida que avanzamos hacia un futuro cada vez más digitalizado, las telecomunicaciones seguirán desempeñando un papel fundamental en nuestra sociedad, impulsando la innovación, la colaboración y el crecimiento en todos los ámbitos. Es importante continuar fomentando el desarrollo de estas tecnologías para garantizar una conectividad sólida y accesible para todos los ciudadanos argentinos.

## Fuente de datos

La información utilizada en este análisis se obtuvo de los conjuntos de datos disponibles en el sitio oficial del ENACOM (Ente Nacional de Comunicaciones).

[Enlace](https://datosabiertos.enacom.gob.ar/dashboards/20000/acceso-a-internet/ " Enacom")


# ETL - Extracción, Transformación y carga de los datasets

En esta etapa del proyecto, se llevó a cabo el proceso de Extracción, Transformación y Carga (ETL) de los datasets seleccionados. El objetivo principal fue analizar la cantidad de datos y realizar una unión adecuada para mejorar el procesamiento de la información. Como resultado, se generaron cuatro datasets principales: `df_combinado`, `df_nacional`, `df_partidos` y `df_indicadores`. 

Durante la etapa de transformación, se aplicaron diversas técnicas para garantizar la calidad y relevancia de los datos. Se llevaron a cabo acciones como la limpieza de registros duplicados, la normalización de variables y la eliminación de aquellos datos considerados redundantes o irrelevantes para los objetivos del proyecto.

El dataset df_combinado se creó como una combinación de varios datasets, permitiendo un análisis integral de los datos de acceso a internet en Argentina. Por otro lado, df_nacional contiene información específica a nivel nacional, mientras que df_partidos se enfoca en los datos a nivel de partidos y localidades. Por último, df_indicadores incluye indicadores socioeconómicos relevantes.

Es importante destacar que la selección y descarte de datasets se realizó de manera cuidadosa, teniendo en cuenta la calidad y pertinencia de la información para este proyecto en particular.

Con la finalización de la etapa de ETL, los datasets resultantes están listos para ser utilizados en el siguiente paso del análisis, donde se buscarán relaciones, patrones y se generarán insights significativos.

# EDA - Análisis Exploratorio de los datos

En este proyecto de análisis de datos, se exploran y analizan cuatro dataframes diferentes: `df_combinado`, `df_nacional`, `df_partidos` y `df_indicadores`. Cada uno de ellos proporciona información relevante sobre distintos aspectos relacionados con las conexiones de internet, indicadores económicos y datos demográficos en Argentina.

## Conceptos relevantes para el análisis de los datos
- **ADSL**: ADSL (Asymmetric Digital Subscriber Line) es una tecnología de conexión a Internet de banda ancha que utiliza líneas telefónicas para transmitir datos. Proporciona una velocidad de descarga más rápida en comparación con la velocidad de carga. Es ampliamente utilizado en hogares y pequeñas empresas.

- **Cablemodem**: El cablemodem es un dispositivo que permite la conexión a Internet a través de las redes de cable de televisión. Utiliza la infraestructura de televisión por cable para transmitir datos de alta velocidad. Es una opción popular para conexiones de Internet de alta velocidad en hogares y negocios.

- **Fibra óptica**: La fibra óptica es una tecnología de transmisión de datos que utiliza hilos delgados de vidrio o plástico para transmitir señales de luz. Proporciona velocidades de conexión extremadamente rápidas y mayor capacidad de ancho de banda en comparación con otras tecnologías. La fibra óptica es conocida por su alta velocidad y estabilidad, y es utilizada en conexiones de Internet de alta velocidad y redes de telecomunicaciones.

- **Wireless**: Wireless, también conocido como conexión inalámbrica, se refiere a la tecnología que permite la transmisión de datos sin cables físicos. Utiliza ondas de radio o señales de infrarrojos para enviar y recibir datos. Las conexiones inalámbricas son ampliamente utilizadas en dispositivos móviles, como teléfonos inteligentes, tabletas y computadoras portátiles, así como en redes Wi-Fi para acceder a Internet.

--

- **Banda ancha fija**: La banda ancha fija se refiere a una conexión de Internet de alta velocidad y constante que utiliza cables físicos, como cables coaxiales o fibra óptica, para transmitir datos. Proporciona una velocidad de conexión más rápida y estable en comparación con las conexiones de acceso telefónico, lo que permite una transferencia eficiente de datos y un acceso rápido a Internet. Ejemplos: ADSL, Cablemodem, Fibra óptica.

- **Dial up**: Dial up es una forma de conexión a Internet que utiliza una línea telefónica y un módem para establecer una conexión temporal. Requiere marcar un número telefónico y establecer una conexión punto a punto con un proveedor de servicios de Internet (ISP). Sin embargo, las conexiones de acceso telefónico son más lentas en comparación con las tecnologías modernas, como la banda ancha, y están siendo reemplazadas por opciones de conexión más rápidas. Ejemplos: ISDN (Integrated Services Digital Network) y modem de acceso telefónico.

--

- **Mbps (Media de bajada)**: Mbps (Megabits por segundo) es una unidad de medida utilizada para expresar la velocidad de transferencia de datos en una conexión a Internet. Representa la cantidad de megabits que pueden ser transferidos por segundo. La velocidad de bajada se refiere a la velocidad a la cual los datos pueden ser descargados desde Internet hacia el dispositivo del usuario. Cuanto mayor sea el valor de Mbps, más rápido será el proceso de descarga de datos.


A continuación, se presenta una descripción detallada de cada dataframe y los principales hallazgos encontrados en el análisis.

## df_combinado

El dataframe `df_combinado` contiene datos relacionados con los tipos de conexiones de internet, tanto en términos de cantidad como de velocidades. A continuación se enumeran algunas de las columnas importantes en este dataframe:

- ADSL, Cablemodem, Fibra óptica, Wireless, Otros: Cantidad de conexiones de cada tipo.
- Accesos por cada 100 hogares: Número de accesos a internet por cada 100 hogares.
- Total_conexion: Total de conexiones de internet registradas.

## df_nacional

El dataframe `df_nacional` proporciona información a nivel nacional sobre las conexiones de internet y algunos indicadores económicos. A continuación se destacan algunas columnas clave:

- Banda ancha fija, Dial up, Mbps (Media de bajada): Cantidad de conexiones según el tipo.
- Ingresos (miles de pesos): Ingresos económicos registrados.
- ADSL, Cablemodem, Fibra óptica, Wireless, Otras conexiones, Total de conexiones de cada tipo.

## df_partidos

El dataframe `df_partidos` contiene datos específicos sobre los diferentes partidos y localidades de Argentina. Algunas columnas relevantes son:

- Provincia, Partido, Localidad: Información geográfica de los datos.
- ADSL, CableModem, Fibra Optica, Otras conexiones: Cantidad de conexiones según el tipo.
- Poblacion: Número de habitantes registrados.
- Telefonia Fija, Latitud, Longitud: Datos adicionales sobre telecomunicaciones y ubicación geográfica.

## df_indicadores

El dataframe `df_indicadores` proporciona indicadores económicos clave. Algunas columnas destacadas son:

- IPC US, IPC AR: Índice de Precios al Consumidor en Estados Unidos y Argentina respectivamente.
- USDARS oficial, USDARS blue: Tasas de cambio del dólar estadounidense en Argentina (oficial y paralelo).
- PBI millones: Producto Bruto Interno registrado.


## Principales hallazgos

Durante el análisis de estos dataframes, se han identificado algunos hallazgos y patrones interesantes. A continuación se presentan algunos de ellos:

- Existe una tendencia a nivel nacional de aumentar las conexiones de cablemodem y fibra óptica, mientras que las conexiones de ADSL se mantuvieron estables hasta cierto punto y luego disminuyeron.
- Se observa una correlación positiva entre algunas velocidades de conexión, lo que puede indicar que los usuarios tienden a migrar a conexiones más rápidas y estables.
- A nivel provincial, se destaca la prevalencia de la telefonía fija en la mayoría de las localidades registradas.
- Los indicadores económicos muestran un aumento anual en el IPC tanto en Estados Unidos como en Argentina, así como una devaluación del peso argentino frente al dólar estadounidense. También se observa un crecimiento del Producto Bruto Interno a lo largo de los años.

Estos hallazgos proporcionan información valiosa para comprender el panorama de las conexiones de internet y los indicadores económicos en Argentina. Este análisis puede ser utilizado para tomar decisiones informadas y desarrollar estrategias efectivas en el ámbito de las telecomunicaciones y el desarrollo socioeconómico del país.

# Power Bi - Presentación de resultados

El análisis del sector de las telecomunicaciones ha proporcionado información valiosa sobre su comportamiento. Los KPI calculados y las métricas analizadas permiten evaluar la penetración de banda ancha, el crecimiento, los accesos por cada 100 hogares, los ingresos por conexión y el porcentaje de conexiones de fibra óptica. Además, el análisis del contexto socioeconómico y los reclamos del mercado han ayudado a comprender los factores externos que influyen en el sector.

Estos resultados y conclusiones son fundamentales para la toma de decisiones estratégicas en el sector de las telecomunicaciones. Los hallazgos proporcionarán información valiosa para mejorar la calidad de los servicios, identificar oportunidades de crecimiento y adaptarse a las demandas del mercado.



