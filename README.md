# IntroCybsercTools

Bienvenidos a la guía de introducción de herramientas de Ciberseguridad

Esta guía esta realizada gracias a los conceptos adquiridos mediante el programa de Google de Ciberseguridad:

https://www.coursera.org/professional-certificates/google-cybersecurity



Hemos de tener en cuenta que son los registros o logs y en que consiste el análisis de estos.

- **El análisis de registros** es una tarea crucial para que los analistas de seguridad identifiquen y mitiguen amenazas, riesgos y vulnerabilidades.

Tres tipos de logs:

1. **Los registros de firewall o firewall logs** registran los intentos de conexión o las conexiones establecidas para el tráfico entrante y saliente.
2. **Los registros de red o network logs** rastrean los dispositivos que entran y salen de la red, así como las conexiones entre dispositivos y servicios.
3. **Los registros del servidor o server logs** registran eventos relacionados con servicios como sitios web, correos electrónicos y recursos compartidos de archivos.



## SIEM Dashboards o Panel de control de Gestión de Información y Eventos de Seguridad

Recopilan y analizan datos de registros para monitorear actividades críticas, proporcionando visibilidad en tiempo real, monitoreo de eventos y alertas automatizadas.

Estas herramientas aumentan la eficiencia al minimizar la cantidad de registros que los profesionales de seguridad deben revisar manualmente.

Consisten en:

- **Los paneles de control SIEM presentan información de seguridad en un formato fácil de entender, similar a como las aplicaciones meteorológicas muestran datos meteorológicos.**
- **Los paneles de control ayudan a los analistas de seguridad a identificar rápidamente actividades sospechosas y tomar decisiones informadas.**
- **Los paneles de control se pueden personalizar para mostrar métricas y datos específicos que sean relevantes para diferentes partes interesadas en una organización.**Ejemplos de métricas: tiempo de respuesta, la disponibilidad y la tasa de fallos.

<img align="center" src="/img/1ºimagenn.PNG"  />

Tipos de herramientas SIEM:

- **Autohospedadas o selfhosted:** Las organizaciones instalan, operan y mantienen estas herramientas en su propia infraestructura. Ideal para organizaciones que necesitan control físico sobre datos confidenciales.
- **Alojadas en la nube o cloudhosted:** Los proveedores de SIEM mantienen y administran estas herramientas, accesibles a través de Internet. Ideal para organizaciones que no quieren invertir en infraestructura.
- **Híbridas o hybrid:** Combina soluciones autohospedadas y alojadas en la nube.

Herramientas SIEM populares:

- **Splunk Enterprise:** Herramienta autohospedada para analizar y buscar datos de registro para obtener información y alertas de seguridad.
- **Splunk Cloud:** Herramienta alojada en la nube para recopilar, buscar y monitorear datos de registro. Ideal para entornos híbridos o solo en la nube.
- **Chronicle:** Herramienta nativa de la nube para análisis de datos, monitoreo de registros y recopilación de datos. Diseñado para aprovechar las capacidades de la computación en la nube.

Vamos a profundizar en como son estas ultimas herramientas mencionadas y en sus paneles de control

**SPLUNK**

Paneles de control de Splunk

- **Panel de control de la postura de seguridad:** Supervisa los eventos y tendencias de seguridad en tiempo real, lo que permite a los analistas evaluar el rendimiento de la infraestructura y las políticas.
- **Panel de control de resumen ejecutivo:** Analiza el estado general de la seguridad a lo largo del tiempo, lo que ayuda a los equipos a mejorar las medidas de seguridad y reducir los riesgos.
- **Panel de control de revisión de incidentes:** Identifica patrones sospechosos durante los incidentes, destacando los elementos de alto riesgo para su revisión inmediata.
- **Panel de control de análisis de riesgos:** Ayuda a los analistas a identificar y priorizar los riesgos asociados con activos, usuarios o direcciones IP específicos.

**CHRONICLE**

Paneles de control de Chronicle

- **Panel de control de información empresarial:** Destaca las alertas recientes y los nombres de dominio sospechosos (IOC), indicando posibles amenazas y su gravedad.
- **Panel de control de ingestión y estado de los datos:** Supervisa la ingestión y el procesamiento de los datos de registro, garantizando la precisión e integridad de los datos para su análisis.
- **Panel de control de coincidencias de IOC:** Realiza un seguimiento de las principales amenazas, riesgos y vulnerabilidades a lo largo del tiempo, lo que permite a los profesionales de la seguridad centrarse en los problemas de alta prioridad.
- **Panel de control principal:** Proporciona una visión general de alto nivel de la ingestión de datos, las alertas y la actividad de los eventos a lo largo del tiempo, lo que ayuda a identificar las tendencias en las distintas fuentes.
- **Panel de control de detección de reglas:** Analiza los incidentes con mayor número de ocurrencias, gravedad y detecciones a lo largo del tiempo, lo que permite a los analistas gestionar los incidentes recurrentes y establecer tácticas de mitigación para reducir el nivel de riesgo de una organización.
- **Panel de control de resumen de inicio de sesión de usuario:** Supervisa el comportamiento de acceso de los usuarios en toda la organización, identificando la actividad inusual de los usuarios, como el inicio de sesión de un usuario desde varias ubicaciones al mismo tiempo. Esta información se utiliza para ayudar a mitigar las amenazas, los riesgos y las vulnerabilidades de las cuentas de usuario y las aplicaciones de la organización.

## Playbooks o Guías de acción

Son manuales que proporcionan detalles sobre las acciones operativas. Sirven para:

- Aclarar qué herramientas deben utilizarse en respuesta a un incidente de seguridad.
- Esenciales para mantener la seguridad de una organización.

Los diferentes tipos incluyen:

- Respuesta a incidentes
- Alertas de seguridad
-  Específicos de equipos 
-  Específicos de productos.

El mas común y usado es el de respuesta a incidentes:

Consiste en una guía con seis fases que se utilizan para mitigar y gestionar los incidentes de seguridad.

- **Preparación:** Las organizaciones deben prepararse para mitigar la probabilidad, el riesgo y el impacto de un incidente de seguridad documentando los procedimientos, estableciendo planes de personal y educando a los usuarios.

  *Ejemplo: Una organización crea un plan de respuesta a incidentes que describe los roles y responsabilidades de cada miembro del equipo de seguridad.*

- **Detección y análisis:** El objetivo de esta fase es detectar y analizar los eventos utilizando procesos y tecnología definidos.

  *Ejemplo: Un analista de seguridad usa una herramienta SIEM para detectar un pico repentino en el tráfico de la red, lo que podría indicar un ataque DDoS.*

- **Contención:** El objetivo de la contención es evitar daños mayores y reducir el impacto inmediato de un incidente de seguridad.

  *Ejemplo: Un analista aísla un sistema infectado con malware para evitar que se propague a otros sistemas.*

- **Erradicación y recuperación:** Esta fase implica la eliminación completa de los artefactos de un incidente para que una organización pueda volver a las operaciones normales.

  *Ejemplo: Un analista elimina el malware de un sistema infectado.*

- **Actividad posterior al incidente:** Esta fase incluye la documentación del incidente, la información a la dirección de la organización y la aplicación de las lecciones aprendidas para garantizar que la organización esté mejor preparada para gestionar futuros incidentes.

  *Ejemplo: Un equipo de seguridad lleva a cabo un análisis exhaustivo de un incidente de seguridad para determinar la causa raíz y evitar que vuelva a ocurrir.*

- **Coordinación:** Informar de los incidentes y compartir información a lo largo del proceso de respuesta a incidentes, basándose en las normas establecidas por la organización.

  *Ejemplo: Una organización comparte información sobre un incidente de seguridad con otras organizaciones de su sector.*



***En general, los manuales de estrategias y las herramientas SIEM son herramientas esenciales para mantener la seguridad de una organización y responder eficazmente a los incidentes de seguridad.***