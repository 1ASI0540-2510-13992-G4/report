<style>
  body {
    font-family: 'Times New Roman', sans-serif;
    text-align: justify;
    font-size: 12px;
    margin-left: 2em;
    margin-right: 2em;
    line-height: 2;
  }
  
  p {
    text-indent: 2em; /* Sangría en el primer renglón de cada párrafo */
  }

  h1 {
    margin-left: 0; /* No aplica sangría para el título principal */
  }

  h2 {
    margin-left: 0; /* No aplica sangría para subtítulos de nivel 2 */
  }

  h3 {
    margin-left: 2em; /* Aplica una sangría de 2em para subtítulos de nivel 3 */
  }

  h4 {
    margin-left: 4em; /* Aplica una sangría de 4em para subtítulos de nivel 4 */
  }
</style>

# UNIVERSIDAD PERUANA DE CIENCIAS APLICADAS

---

<p align="center">
  <img src="assets/upc_logo.svg"  style="width:500px; height:auto;" alt="">
</p>


# ANÁLISIS FORENSE DE SOFTWARE - 1ASI0540 - 13992

---

## INFORME DEL TRABAJO FINAL

### PROFESOR: Del Carpio Wong, Miguel Adolfo
### TEMA: Dark Web Forensics

## INTEGRANTES:

<table>
  <thead>
    <tr>
      <th style="background-color: #333; color: #fff;">Apellidos y Nombres</th>
      <th style="background-color: #333; color: #fff;">Código de Alumno</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Irigoyen Matos, Javier Sharvel</td>
      <td>u20221d156</td>
    </tr>
    <tr>
      <td>Jara Benites Quique, Vladimir</td>
      <td>u202022365</td>
    </tr>
    <tr>
      <td>León Vivas, Fabrizio Amir</td>
      <td>u20211b994</td>
    </tr>
    <tr>
      <td>Lizano Coll Cardenas, Fernando Jesus</td>
      <td>u202214522</td>
    </tr>
    <tr>
      <td>Lopez Acuña, Mario Joaquin</td>
      <td>u202116250</td>
    </tr>
    <tr>
      <td>Pescorán Angulo, Juan Fabritzzio</td>
      <td>u20221c936</td>
    </tr>
  </tbody>
</table>

--- 

2025 - 01

---

# Registro de Versiones del Informe

<table>
  <thead>
    <tr>
      <th style="background-color: #333; color: #fff;">Versión</th>
      <th style="background-color: #333; color: #fff;">Fecha</th>
      <th style="background-color: #333; color: #fff;">Autor</th>
      <th style="background-color: #333; color: #fff;">Descripción de modificación</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
  </tbody>
</table>

---

# Project Report Collaboration Insights
Para este proyecto hemos utilizado las herramientas GitHub para gestionar el progreso grupal.

Puede acceder al contenido del repositorio pulsando sobre el siguiente ícono:

<p align="center">
  <a href="https://github.com/1ASI0540-2510-13992-G4/report">
    <img src="assets/logos/teemo_solutions_logo.jpg" style="width:200px; height:auto;" alt="">
  </a>
</p>

aún falta colocar img xd

# Resumen

Este informe analiza el ataque de ransomware al oleoducto Colonial Pipeline en mayo de 2021, un incidente de alto impacto vinculado a la dark web, seleccionado como caso de estudio para el curso SI540. Atribuido al grupo DarkSide, el ataque paralizó el mayor sistema de distribución de combustible en EE. UU., provocando escasez de gasolina tras el cifrado de sistemas críticos y el robo de ~100 GB de datos sensibles. Los atacantes exigieron un rescate de US$4,4 millones mediante un portal en la red Tor. Posteriormente, las autoridades recuperaron parte del pago.

La intrusión se originó por credenciales de VPN comprometidas, disponibles en la dark web, lo que evidencia su papel en todo el ciclo del ataque: desde el acceso inicial hasta la extorsión. El informe detalla la cronología del incidente, las vulnerabilidades explotadas, la respuesta adoptada y los TTPs empleados, mapeados al marco MITRE ATT&CK. También se presentan cinco incidentes similares y se proponen estrategias de mitigación basadas en NIST, ISO/IEC y CIS Controls. El estudio resalta la necesidad de una ciberseguridad proactiva y en capas frente a amenazas relacionadas con la dark web.

!! ACÁ FALTA CITAR
 
# Indice
### [Registro de versiones del informe]()
### [Project Report Collaboration Insights]()
### [Indice]()
### [Resumen]()
### [Student Outcome]()

## [Capítulo 1: Incidentes]()
- [1.1. Listado de los últimos incidentes]()
- [1.2. Incidentes más graves]()

## [Capítulo 2: Incidente más grave (colocar el nombre)]()
- [2.1. Identificación del Incidente]()
  - [2.1.1. Descripción]()
  - [2.1.2. Consecuencias]()
    - [2.1.2.1. Activos Afectados]()
    - [2.1.2.2. Servicios Afectados]()
    - [2.1.2.3. Impacto]()
    - [2.1.2.4. Tiempo de indisponibilidad]()
  - [2.1.3. Proceso de Respuesta]()
  - [2.1.4. Solución del incidente]()
  - [2.1.5. Causa raíz del incidente]()
  - [2.1.6. Plan de acción seguido]()
  - [2.1.7. Clasificación del Incidente]()
- [2.2. Pérdidas]()
  - [2.2.1. Económicas]()
  - [2.2.2. Reputacionales]()
- [2.3. Tácticas, técnicas y procedimientos (TTPs) utilizados por el grupo]()
  - [2.3.1. Tácticas]()
  - [2.3.2. Técnicas]()
  - [2.3.3. Procedimientos]()
- [2.4. Vulnerabilidades asociadas al incidente]()
  - [2.4.1. CVE]()
  - [2.4.2. CVSS]()
  - [2.4.3. CWE]()

## [Capítulo 3: Estrategias de Ciberseguridad]()
- [3.1. Estrategias a Nivel Organizacional]()
- [3.2. Estrategias a Nivel de Infraestructura]()
- [3.3. Estrategias a Nivel de Desarrollo de Software]()
- [3.4. Estrategias a Nivel de Sistema de Información]()

## [Conclusiones]()
## [Recomendaciones]()
## [Bibliografía]()

<style>
  body {
    font-family: 'Times New Roman', sans-serif;
    text-align: justify;
    font-size: 12px;
    margin-left: 2em;
    margin-right: 2em;
    line-height: 2;
  }
  
  p {
    text-indent: 2em; /* Sangría en el primer renglón de cada párrafo */
  }

  h1 {
    margin-left: 0; /* No aplica sangría para el título principal */
  }

  h2 {
    margin-left: 0; /* No aplica sangría para subtítulos de nivel 2 */
  }

  h3 {
    margin-left: 2em; /* Aplica una sangría de 2em para subtítulos de nivel 3 */
  }

  h4 {
    margin-left: 4em; /* Aplica una sangría de 4em para subtítulos de nivel 4 */
  }
</style>

# **Capítulo 1: Incidentes**

## 1.1. Listado de últimos incidentes

A modo de contexto, a continuación, se enlistan brevemente cinco incidentes de ciberseguridad ocurridos en los últimos años (2020–2023) que presentan conexión directa y documentada con la dark web, ya sea por la filtración/venta de datos robados, extorsión mediante sitios ocultos de ransomware, uso de foros clandestinos para distribución de malware, o coordinación de actividades criminales en la darknet:

- 1. **Ataque de Ransomware a Colonial Pipeline (2021) Grupo DarkSide:** Cibercriminales comprometieron la mayor red de oleoductos de EE. UU. usando una contraseña filtrada en la dark web. Cifraron sistemas de TI y robaron ~100 GB de datos, exigiendo rescate de 75 BTC (US$4,4 M) a través de un portal Tor. Amenazaron con divulgar la información en su sitio de filtraciones en la darknet si no se pagaba. Es el caso que se analiza en detalle en este informe.


- 2. **Cadena de Suministro - Ransomware a Kaseya VSA (2021) – Grupo REvil (Sodinokibi):** Un ataque sofisticado explotó vulnerabilidades zero-day (CVE-2021-30116 y otras) en el software de administración Kaseya VSA. Los atacantes distribuyeron ransomware masivamente a unas 1.500 empresas clientes en al menos 17 países. REvil exigió un rescate de 70 millones de dólares por un descifrador universal, publicando la demanda abiertamente en su sitio “Happy Blog” en la dark web. Aunque pidieron hasta $5M a algunas víctimas grandes, ofrecieron desbloqueo global por 70M en bitcoins. No hubo evidencia de filtración de datos en este caso debido al enfoque en cifrado masivo, pero el portal oculto fue central en la extorsión.


- 3. **Brecha de Datos en T-Mobile (2021):** En agosto de 2021, T-Mobile EE. UU. sufrió una grave brecha de seguridad que expuso los datos personales de aproximadamente 100 millones de clientes. El atacante, identificado como John E. Binns, accedió a la red de la compañía a través de un punto de entrada desprotegido. Entre la información robada se encontraban nombres completos, números de teléfono, números de Seguridad Social (SSN), licencias de conducir y códigos IMEI de dispositivos móviles. Posteriormente, el hacker ofreció a la venta una muestra de 30 millones de registros en un foro clandestino por 6 Bitcoins (aproximadamente 270 mil dólares estadounidenses en ese momento). La autenticidad de los datos fue verificada por medios especializados. T-Mobile confirmó públicamente el incidente el 17 de agosto de 2021. Más adelante, autoridades estadounidenses presentaron cargos formales contra Binns, quien había declarado que la seguridad de la empresa era “terriblemente débil”.


- 4. **Campaña de Ransomware Conti contra Costa Rica (2022):** A partir de abril de 2022, el gobierno de Costa Rica fue blanco de una serie de ataques de ransomware coordinados por el grupo criminal Conti, que afectaron a múltiples entidades estatales, incluidos los ministerios de Hacienda y Salud. Inicialmente, los atacantes exigieron un rescate de 10 millones de dólares a cambio de no divulgar información sensible. Ante la negativa del gobierno, Conti duplicó la demanda a 20 millones y exhortó a la población costarricense a presionar a sus autoridades para que pagaran. En mayo de 2022, la situación llevó al país a declarar un estado de emergencia nacional. Como represalia, el grupo filtró aproximadamente 672 GB de datos gubernamentales en su portal de la dark web. Poco después, Conti cesó sus operaciones bajo ese nombre, aunque sus miembros se habrían reagrupado en otras estructuras criminales. Este incidente evidenció la vulnerabilidad de las infraestructuras gubernamentales ante amenazas cibernéticas y el papel de la dark web como canal de extorsión y difusión de información confidencial.


- 5. **Brecha de Datos en Medibank (2022):** En octubre de 2022, Medibank, la mayor aseguradora de salud de Australia, fue víctima de un ciberataque que expuso información personal y médica de aproximadamente 9,7 millones de personas. Tras negarse a pagar el rescate exigido, la empresa enfrentó una filtración progresiva de los datos robados en un blog alojado en la dark web, llevada a cabo por actores vinculados a ransomware, presuntamente afiliados al grupo REvil. Los atacantes publicaron información extremadamente sensible, como diagnósticos de VIH y tratamientos por adicciones, clasificando a los pacientes como “buenos” o “malos” con el fin de ejercer mayor presión pública. El 1 de diciembre de 2022, los responsables del ataque declararon finalizada la operación (“case closed”) y liberaron en la dark web un archivo comprimido de 5 GB, que contenía los ~200 GB de datos robados. Este grave incidente generó una fuerte respuesta social y política en Australia, incluyendo una revisión de las normativas sobre notificación de brechas y la seguridad de los datos de salud.

Los casos anteriores representan solo una parte del conjunto de incidentes recientes con vínculos directos a la dark web. A continuación, se presenta un análisis detallado del caso seleccionado como principal: el ataque al oleoducto Colonial Pipeline. 
 
## 1.2. Incidentes más graves

# **Capítulo 2: Incidente más grave: Ataque Forense al Oleoducto Colonial Pipeline (2021)**

## 2.1. Identificación del Incidente

En esta sección se presenta un análisis forense completo del ataque de ransomware sufrido por Colonial Pipeline en mayo de 2021, un incidente emblemático tanto por su gravedad como por la participación de la dark web, que estuvo presente tanto en la intrusión como en la extorsión. El análisis se detalla cronológicamente, abarcando cada fase del ataque desde su inicio hasta su resolución.

### 2.1.1. Descripción

- **Cronología del Ataque**

  - **Abril 29, 2021:** Según la firma Mandiant, los atacantes ya estaban activos en la red de Colonial Pipeline desde al menos el 29 de abril. Sin embargo, en ese momento no se detectó actividad maliciosa evidente. Se cree que el acceso inicial fue posible mediante el uso de credenciales comprometidas de una VPN legada.
  - **7 de mayo, 2021 (Día 0):** Colonial Pipeline detecta una intrusión de ransomware en su entorno de TI. El ataque, iniciado en la madrugada, cifró archivos en los sistemas de administración del oleoducto. En respuesta al descubrimiento, la empresa decide detener proactivamente todas las operaciones del oleoducto para contener la propagación. Ese mismo día, los atacantes envían un mensaje de rescate a la empresa, indicando que el pago debía hacerse en Bitcoin a través de un portal oculto en la red Tor, propiedad del grupo DarkSide.
  - **8 de mayo, 2021:** Colonial Pipeline notifica el incidente a las autoridades federales de EE. UU. (FBI, CISA) y contrata expertos forenses externos (por ejemplo, Mandiant) para ayudar en la respuesta. Se comienzan a evaluar los sistemas comprometidos y verificar si se ha producido el robo de datos. Los atacantes afirman haber robado aproximadamente 100 GB de datos de los servidores de Colonial Pipeline antes de cifrarlos, amenazando con divulgar esta información si no se paga el rescate.
  - **9 de mayo, 2021:** Debido a la crítica situación (el oleoducto abastece alrededor del 45% del combustible de la costa este de EE. UU.) y la imposibilidad de restaurar rápidamente los sistemas, Colonial Pipeline decide pagar el rescate exigido para obtener la herramienta de descifrado. El pago fue de 75 Bitcoins (aproximadamente 4,4 millones de dólares), transferidos a la billetera indicada por DarkSide bajo la supervisión del FBI. Tras el pago, los atacantes proporcionan un decryptor o clave maestra. Mientras tanto, el Gobierno de EE. UU. emite una declaración regional de emergencia para facilitar el transporte alternativo de combustible por carretera en 17 estados.
  - **10–12 de mayo, 2021:** La herramienta de descifrado proporcionada resulta ser ineficaz y lenta. Como resultado, Colonial Pipeline recurre principalmente a restaurar sistemas desde sus respaldos internos para reanudar las operaciones. La empresa informa que su prioridad es garantizar la integridad de los sistemas antes de reiniciar el flujo de combustible. El 12 de mayo, después de casi 6 días de interrupción, Colonial Pipeline reinicia plenamente sus operaciones de bombeo de combustible, aunque algunos efectos operativos continuaron hasta el 15 de mayo, según reportes posteriores.
  - **19 de mayo, 2021:** Las investigaciones federales identifican varias direcciones de Bitcoin asociadas con el pago. El Departamento de Justicia logra rastrear y acceder a una de las carteras utilizadas por DarkSide. Para el 7 de junio, las autoridades anuncian la recuperación de 63,7 BTC (aproximadamente el 84% del rescate) mediante una clave privada en poder del FBI. Debido a la caída en el valor de Bitcoin, esos 63,7 BTC valían aproximadamente 2,3 millones de dólares, casi la mitad de los 4,4 millones de dólares iniciales. Este logro se considera uno de los primeros casos significativos de recuperación de un pago de ransomware.
  - **8–9 de junio, 2021:** El CEO de Colonial Pipeline, Joseph Blount, comparece ante el Senado de EE. UU. para dar explicaciones sobre el incidente. Revela que la brecha ocurrió debido a una única contraseña comprometida en una VPN sin autenticación multifactor. Explica que la cuenta VPN era legada, deshabilitada, pero aún accesible desde el punto de vista técnico y operativo, y que no contaba con MFA habilitado. También señala que no hubo evidencia de phishing, sugiriendo que los atacantes obtuvieron la contraseña de fuentes externas. Esta declaración valida la teoría de la reutilización de credenciales filtradas.
  - **Mayo – Julio 2021 (post-ataque):** DarkSide, el grupo criminal responsable del ataque, enfrenta presión internacional. A mediados de mayo, anuncian el cierre de sus operaciones y afirman haber donado parte de sus ganancias, probablemente como una estrategia para desviar la atención. Sin embargo, la inteligencia de seguridad indica que DarkSide se reconstituye bajo un nuevo nombre, “BlackMatter”, continuando ataques similares durante 2021. Colonial Pipeline colaboró con CISA y el FBI, compartiendo indicadores de compromiso (IoCs) del malware de DarkSide, que se publicaron en alertas de seguridad. Este incidente impulsó iniciativas gubernamentales para mejorar la ciberseguridad crítica, incluida la creación de un Joint Ransomware Task Force por CISA/FBI en 2022.

### 2.1.2. Consecuencias

El ataque a Colonial Pipeline no solo tuvo repercusiones inmediatas en los sistemas internos de la compañía, sino que también impactó gravemente la infraestructura crítica y la vida cotidiana de millones de personas. A continuación, se detallan los principales efectos del ataque en los activos, servicios y operaciones de la empresa.

#### 2.1.2.1. Activos Afectados

La investigación forense identificó los activos de TI específicos que resultaron comprometidos o afectados durante el incidente. Entre los principales se encuentran:

- **Red VPN Legada (Acceso Remoto):**

El ataque comenzó a través de un servidor de VPN de acceso remoto, el cual pertenecía a un sistema legado no adecuadamente desactivado. Este acceso, utilizado por empleados retirados o contratistas, carecía de autenticación multifactor, lo que permitía la conexión a la red interna mediante solo usuario y contraseña. La cuenta asociada, aunque inactiva, permaneció válida, funcionando como una puerta trasera inadvertida para los atacantes.


- **Servidores de Dominio y Directorio Activo:**

Tras obtener acceso a la red interna a través de la VPN, los atacantes probablemente lograron infiltrarse en los servidores de autenticación, tales como los controladores de dominio Active Directory. Esto les permitió escalar privilegios y moverse lateralmente en la red, comprometiendo múltiples sistemas Windows al obtener hashes de contraseñas y credenciales adicionales.


- **Sistemas de Facturación y Administración:**

La infección de ransomware afectó gravemente los sistemas administrativos de Colonial Pipeline, especialmente los encargados de la facturación y gestión de pedidos. Esta interrupción obligó a la empresa a cerrar temporalmente el oleoducto, ya que no podían procesar correctamente las facturas del combustible distribuido. Esto afectó la capacidad para monitorear y cobrar por los productos, pues servidores de bases de datos y aplicaciones financieras/logísticas fueron cifrados por el ransomware DarkSide.


- **Estaciones de Trabajo Corporativas:**

El ransomware también impactó una gran cantidad de estaciones de trabajo corporativas y servidores Windows en la red. El malware cifró archivos en todos los sistemas alcanzables, incluidos servidores de archivos, equipos de usuarios, y copias de seguridad en línea. Archivos ofimáticos, documentos internos, correos electrónicos almacenados localmente y otros datos en estaciones de trabajo fueron comprometidos, lo que generó una pérdida considerable de información.


- **Backups Conectados:**

Un aspecto crítico en la recuperación fue el análisis de las copias de seguridad. Aunque Colonial pudo utilizar backups offline para restaurar sus operaciones, es posible que algunas copias de seguridad que estuvieran accesibles desde la red en el momento del ataque también fueran cifradas. Sin embargo, la restauración exitosa de los sistemas sugiere que al menos algunos respaldos fueron seguros y no fueron afectados.


- **Datos Exfiltrados:**

Los atacantes también extrajeron aproximadamente 100 GB de datos sensibles, incluidos documentos de negocios, configuraciones de red, y datos personales de empleados y clientes. Estos datos fueron transferidos fuera de la red de Colonial Pipeline mediante su canal de comando y control (C2), probablemente utilizando Tor o cifrado para evitar su detección. Esto representó una grave amenaza a la privacidad y seguridad de la información confidencial de la empresa.

---
En resumen, los activos afectados fueron principalmente sistemas clave de TI corporativos, como la red VPN, servidores Windows y aplicaciones de negocio. Sin embargo, y de manera crítica, los sistemas operativos tecnológicos (OT) de control del oleoducto no fueron comprometidos directamente. No obstante, la interconexión entre los sistemas TI y OT provocó que la infección en los primeros obligara a la detención preventiva de los segundos, como medida de seguridad. Este incidente subraya la importancia vital de una adecuada segmentación entre ambas redes para prevenir que vulnerabilidades en TI puedan impactar sistemas críticos de infraestructura operativa.

#### 2.1.2.2. Servicios Afectados

El ataque a Colonial Pipeline tuvo un impacto significativo en varios servicios clave, afectando tanto a la operación interna como a los servicios externos relacionados con el suministro de combustible y la infraestructura crítica. A continuación, se detallan los principales servicios afectados:

1. **Operación de Oleoducto y Distribución de Combustible**:  
La interrupción del flujo de combustible a través del oleoducto Colonial Pipeline fue el servicio más directamente afectado. Como medida de precaución, Colonial Pipeline decidió detener todas las operaciones del oleoducto para evitar una propagación del ataque. Esto paralizó la distribución de gasolina, diésel y combustible de aviación en la costa Este de los Estados Unidos durante casi 6 días, lo que generó escasez de combustible en varios estados.


2. **Sistemas de Facturación y Gestión de Pedidos**:  
   Los sistemas de facturación y administración que controlan el seguimiento y pago de la distribución de productos se vieron gravemente comprometidos. El cifrado de estos sistemas impidió a Colonial Pipeline realizar las funciones de facturación necesarias para gestionar el flujo de combustible, lo que contribuyó a la decisión de cerrar el oleoducto. La incapacidad de realizar tareas administrativas vitales afectó la gestión logística y financiera del servicio.


3. **Sistemas de Seguridad y Monitoreo**:  
   Aunque no se comprometieron directamente los sistemas de control de la infraestructura OT, los sistemas de monitoreo y seguridad asociados con la red de TI fueron afectados. La incapacidad de monitorear los sistemas de control del oleoducto durante el ataque obligó a Colonial Pipeline a tomar medidas preventivas, como la detención del servicio para garantizar la seguridad operativa y la integridad de la infraestructura crítica.


4. **Acceso a Información y Comunicación Interna**:  
   El ataque afectó a las estaciones de trabajo corporativas y los servidores de la empresa, lo que interrumpió las comunicaciones internas y la accesibilidad de información vital para los empleados. Esto impidió la correcta coordinación de la respuesta al incidente y afectó el acceso a los recursos necesarios para la recuperación.


5. **Servicios de Backup y Recuperación de Datos**:  
   Los servicios de respaldo, aunque parcialmente comprometidos, permitieron a la empresa restaurar sus sistemas. La restauración de operaciones dependió en gran medida de los backups offline, lo que subraya la importancia de contar con copias de seguridad externas y no accesibles directamente desde la red principal para evitar que se vean comprometidas en ataques como este.


En general, el ataque afectó a múltiples servicios críticos dentro de Colonial Pipeline, creando una cadena de interrupciones que impactaron tanto en las operaciones internas como en el suministro de combustible, afectando a consumidores y sectores dependientes de esta infraestructura esencial.

#### 2.1.2.3. Impacto

El ataque a Colonial Pipeline tuvo un impacto significativo a varios niveles: técnico, económico, social y regulatorio.

En primer lugar, la interrupción operativa del oleoducto generó un desabastecimiento masivo de combustibles en la costa este de Estados Unidos, afectando directamente a millones de personas. Esto se tradujo en largas filas en gasolineras, compras de pánico y alteraciones en la logística de transporte, tanto terrestre como aéreo. Aeropuertos clave, como el de Atlanta, se vieron forzados a buscar fuentes alternativas de suministro o reprogramar vuelos debido a la escasez de combustible para aeronaves.

En segundo lugar, el ataque expuso debilidades críticas en la ciberseguridad de infraestructuras esenciales. Aunque el malware no alcanzó directamente los sistemas OT (tecnología operativa) que controlan el flujo físico del oleoducto, la afectación de los sistemas TI en especial los sistemas de facturación y monitoreo obligó a detener las operaciones por razones de seguridad y trazabilidad.

Desde el punto de vista económico, el rescate pagado ascendió a US$4,4 millones, además de las pérdidas asociadas a la interrupción del servicio, los costos de recuperación tecnológica, investigaciones, asesorías legales y posibles sanciones regulatorias. Si bien una parte del rescate fue recuperada por el Departamento de Justicia, el daño económico fue considerable.

Finalmente, el incidente provocó un daño reputacional severo para Colonial Pipeline, que fue ampliamente criticada por su falta de preparación y medidas preventivas mínimas como la autenticación multifactor. Esto, a su vez, derivó en una respuesta gubernamental más estricta, incluyendo la imposición de nuevas regulaciones obligatorias en ciberseguridad para operadores de infraestructura crítica.

En conjunto, el impacto del incidente fue una advertencia clara de cómo los ciberataques pueden trascender lo digital para desestabilizar aspectos clave del funcionamiento social y económico de un país.

#### 2.1.2.4. Tiempo de Indisponibilidad

El tiempo de indisponibilidad operativa de Colonial Pipeline fue de aproximadamente seis días. El ataque ocurrió el 7 de mayo de 2021, y el oleoducto comenzó a reanudar operaciones el 12 de mayo del mismo año, con un restablecimiento completo reportado el 15 de mayo.

Durante este período, las operaciones de distribución de combustible se vieron completamente detenidas en gran parte del sistema, lo que provocó una escasez significativa de gasolina, diésel y combustible para aviación en múltiples estados de la costa este de EE.UU.

A nivel de sistemas internos de TI, algunos servidores y estaciones de trabajo tardaron más en ser restaurados. La prioridad se centró en recuperar la infraestructura crítica para facturación y logística. Gracias a la disponibilidad de copias de seguridad ilesas, Colonial pudo iniciar el proceso de recuperación poco después del ataque, aunque la restauración completa de todos los servicios tomó semanas.

Este tiempo de inactividad evidenció la alta dependencia entre los sistemas TI y las operaciones OT, así como la necesidad de contar con planes de respuesta y recuperación más robustos para minimizar el impacto en la continuidad del negocio.

#### Tabla 

<table>
  <thead>
    <tr>
      <th>Categoría</th>
      <th>Detalle</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Activos Afectados</strong></td>
      <td>
        - Red VPN Legada comprometida por falta de MFA y cuenta inactiva activa.<br>
        - Servidores Windows y Active Directory: movimiento lateral y escalada de privilegios.<br>
        - Sistemas de facturación y administración: cifrados, imposibilitando la operación.<br>
        - Estaciones de trabajo corporativas afectadas por ransomware.<br>
        - Backups conectados parcialmente cifrados; backups offline permitieron recuperación.<br>
        - Exfiltración de 100 GB de datos sensibles mediante canales cifrados.
      </td>
    </tr>
    <tr>
      <td><strong>Servicios Afectados</strong></td>
      <td>
        - Operación del oleoducto detenida por precaución.<br>
        - Sistemas de facturación y pedidos inhabilitados.<br>
        - Sistemas de monitoreo y seguridad de TI impactados.<br>
        - Comunicación interna y acceso a información corporativa interrumpidos.<br>
        - Servicios de backup parcial comprometidos; recuperación posible gracias a backups offline.
      </td>
    </tr>
    <tr>
      <td><strong>Impacto</strong></td>
      <td>
        - Desabastecimiento de combustible y pánico social en la costa este de EE.UU.<br>
        - Vulnerabilidad crítica expuesta en infraestructura esencial.<br>
        - Pérdidas económicas, incluyendo el pago de US$4.4 millones en rescate.<br>
        - Daño reputacional y presión regulatoria significativa.<br>
        - Respuesta gubernamental con nuevas regulaciones de ciberseguridad.
      </td>
    </tr>
    <tr>
      <td><strong>Tiempo de Indisponibilidad</strong></td>
      <td>
        - Aproximadamente 6 días sin operación (7–12 de mayo de 2021).<br>
        - Restablecimiento completo reportado el 15 de mayo.<br>
        - Recuperación de TI tomó semanas; prioridad fue facturación y logística.<br>
        - Evidenció la dependencia entre TI y OT, y la necesidad de planes de contingencia.
      </td>
    </tr>
  </tbody>
</table>


### 2.1.3. Proceso de Respuesta

Colonial Pipeline contaba con un Plan de Respuesta a Incidentes (PRI) y ejecutó un proceso estructurado de respuesta al ataque, alineado en gran medida con buenas prácticas del sector y marcos reconocidos como NIST 800-61r2 (Computer Security Incident Handling Guide). A continuación se describe cómo su actuación refleja un proceso basado en un framework maduro:

**1. Preparación (Preparation):**

- Existencia de un PRI y Ciberseguro: Colonial tenía un plan de respuesta vigente y cobertura de ciberseguro, lo cual facilitó la activación rápida de mecanismos formales y contactos clave.
- Alianzas preestablecidas: Contaban con acceso a expertos externos (Mandiant), lo que indica preparación anticipada para incidentes de gran escala.

**2. Detección y Análisis (Detection & Analysis):**

- Detección el 7 de mayo: El ransomware fue detectado temprano en la mañana.
- Análisis forense: Se contrató inmediatamente a Mandiant, que realizó análisis detallados de memoria, discos y logs.
- Identificación del vector de ataque: Se determinó que el ingreso fue mediante una cuenta VPN inactiva sin MFA.
- Uso de IoCs y herramientas como Cobalt Strike identificadas: Indicadores de compromiso fueron compartidos con CISA y otras entidades.

**3. Contención, Erradicación y Recuperación:**

- **Contención inmediata:**
  - Aislamiento de sistemas afectados.
  - Desconexión de los sistemas OT como medida preventiva.
  - Apagado del oleoducto para prevenir movimiento lateral.


- **Erradicación:**
  - Cierre de accesos vulnerables (VPN legadas).
  - Deshabilitación de cuentas comprometidas.
  - Escaneo y limpieza de la red con apoyo de Mandiant.


- **Recuperación:**
  - Uso del descifrador recibido tras el pago.
  - Restauración desde backups cuando el descifrador falló.
  - Reimplementación progresiva de sistemas críticos: primeras operaciones (SCADA), luego facturación.
  - Aplicación de MFA de emergencia antes de restablecer accesos remotos.

**4. Comunicación y Coordinación:**
   
- Notificación rápida a autoridades: FBI, CISA y Departamento de Energía fueron informados desde el inicio.
- Comunicaciones públicas claras: Colonial fue progresivamente transparente sobre la naturaleza del incidente y sus efectos.
- Colaboración activa: Participaron en alertas conjuntas con CISA/FBI para prevenir ataques similares en otras infraestructuras.

**5. Mejora Continua (Post-Incident Activities):**

- Auditoría y refuerzo de controles:
  - Segmentación de red. 
  - MFA universal. 
  - Cierre de puertos y servicios obsoletos. 
  - Implementación de monitoreo continuo.


- Lecciones compartidas:
  - Distribución de IoCs y tácticas de DarkSide al sector energético. 
  - Participación en análisis de inteligencia sectorial.

### 2.1.4. Solución del incidente

### 2.1.5. Causa raíz del incidente

### 2.1.6. Plan de acción seguido

### 2.1.7. Clasificación del Incidente

## 2.2. Pérdidas

### 2.2.1. Económicas
### 2.2.2. Reputacionales

## 2.3. Tácticas, técnicas y procedimientos (TTPs) utilizados por el grupo

### 2.3.1. Tácticas
### 2.3.2. Técnicas
### 2.3.3. Procedimientos

## 2.4. Vulnerabilidades asociadas al incidente

### 2.4.1. CVE
### 2.4.2. CVSS
### 2.4.3. CWE


# **Capítulo 3: Estrategias de Ciberseguridad**

## 3.1. Estrategias a Nivel Organizacional

## 3.2. Estrategias a Nivel de Infraestructura

## 3.3. Estrategias a Nivel de Desarrollo de Software

## 3.4. Estrategias a Nivel de Sistema de Información

