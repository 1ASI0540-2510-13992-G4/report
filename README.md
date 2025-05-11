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

Colonial Pipeline adoptó un enfoque integral y coordinado para resolver el incidente de ransomware, combinando acciones técnicas, operativas y legales. Tras el análisis forense inicial, se utilizó el descifrador proporcionado por los atacantes luego del pago del rescate para intentar recuperar los sistemas cifrados. 

**Cuando el descifrador resultó ineficaz en algunos equipos, se recurrió a copias de seguridad verificadas para restaurar los servicios:**
- Se priorizó el restablecimiento seguro de los sistemas SCADA para reanudar la operación del oleoducto.
- Se implementaron controles de seguridad reforzados como MFA de emergencia y segmentación de red antes de restablecer la conectividad externa.
- La empresa colaboró con agencias gubernamentales y con la firma Mandiant para asegurar la limpieza completa de la red.
- Se compartieron indicadores de compromiso y lecciones aprendidas con el sector energético a través de CISA y el FBI.

### 2.1.5. Causa raíz del incidente

La causa raíz del incidente de Colonial Pipeline se puede atribuir a una serie de fallas en los controles de acceso y gestión de credenciales, lo que permitió la entrada de los atacantes de manera no detectada inicialmente.

  - **Uso de Credenciales Filtradas en la Dark Web**: La investigación reveló que los atacantes lograron acceso mediante una cuenta VPN comprometida. Esta cuenta pertenecía a Colonial Pipeline y su contraseña se encontraba en un lote de credenciales filtradas publicado en la dark web. Los atacantes compraron o escanearon bases de datos en la darknet que contenían credenciales válidas, y una de ellas correspondía a Colonial Pipeline, lo que permitió el acceso sin detección.
  - **Cuenta VPN Legada sin MFA**: La cuenta comprometida estaba asociada a un sistema de VPN antiguo, el cual no contaba con autenticación multifactor (MFA). Esto permitió a los atacantes ingresar a la red con solo la combinación de usuario y contraseña, lo que constituyó una vulnerabilidad crítica, al no existir una segunda capa de autenticación.
  - **Falta de Deshabilitación de Cuenta Inactiva**: La cuenta VPN comprometida aparentemente pertenecía a un ex-empleado o no se usaba regularmente, pero seguía activa. Esto reveló una deficiencia en la gestión del ciclo de vida de identidades, ya que la cuenta no fue deshabilitada o eliminada cuando se volvió obsoleta.
  - **Posible Escaneo de Puertos/Vulnerabilidades Públicas**: Aunque no hubo explotación de vulnerabilidades específicas, es probable que los atacantes realizaran un reconocimiento externo, buscando accesos VPN expuestos públicamente y verificando qué sistemas estaban disponibles. Esta información les permitió probar credenciales filtradas hasta obtener acceso sin utilizar malware, lo que dificultó la detección de la intrusión.

**Resumen**: La causa raíz del incidente se puede considerar un error humano y procedimental. La exposición de credenciales filtradas en la dark web, sumado a la falta de autenticación fuerte en una VPN expuesta a Internet, permitió que los atacantes ingresaran como usuarios legítimos. Una vez dentro, los atacantes explotaron la confianza implícita en la red interna para desplegar el ransomware. Este incidente destaca la importancia de monitorear filtraciones de datos y de implementar controles de autenticación robustos en sistemas expuestos.

### 2.1.6. Plan de acción seguido

- **Contención inmediata**:
   - Desde el momento del descubrimiento del ataque, Colonial Pipeline ejecutó un aislamiento inmediato de los sistemas afectados, desconectando partes críticas de la red.
   - Se apagó el oleoducto y se desconectaron los sistemas de control industrial (OT) para evitar la propagación del ransomware a los sistemas críticos de operaciones.
   - Esta medida evitó que el atacante tuviera acceso a las redes OT, protegiendo así los controladores de bombeo y otros componentes vitales.


- **Activación del Plan de Respuesta a Incidentes**:
  - Colonial Pipeline activó su plan de respuesta, notificando a las autoridades pertinentes, incluidas la CISA, el FBI y el Departamento de Energía.
  - La empresa convocó al equipo interno de TI y Seguridad, y contrató a la firma Mandiant (FireEye) para liderar la investigación forense y la contención técnica.
  - Mandiant ayudó a rastrear las acciones del atacante, identificar el vector de acceso (la cuenta VPN comprometida) y evaluar el alcance de la intrusión.


- **Comunicación con autoridades y público**:
  - Colonial Pipeline mantuvo una comunicación constante con las autoridades relevantes y emitió comunicados de prensa informando sobre el ataque.
  - Primero se informó de "problemas técnicos" y luego se confirmó el ciberataque y el apagón del oleoducto.
  - Se coordinó con agencias gubernamentales para asegurar que la información se manejara adecuadamente y se mantuviera al público informado.


- **Pago controlado del rescate**:
  - Colonial Pipeline, en consulta con el FBI y sus aseguradoras, optó por negociar con los atacantes.
  - A través de un portal seguro en la dark web proporcionado por los atacantes, se coordinó el pago de 75 BTC como parte del rescate.
  - Este pago fue monitoreado por el FBI, lo que permitió la recopilación de información valiosa sobre las comunicaciones y las direcciones de criptomonedas, facilitando la posterior recuperación de fondos.


- **Análisis forense post-incidente**:
  - Mandiant realizó un análisis detallado de la intrusión, recolectando información de sistemas comprometidos, incluyendo volcados de memoria, copias forenses de discos y registros.
  - Se identificaron las credenciales comprometidas utilizadas por los atacantes y se procedió a deshabilitar las cuentas afectadas.
  - Además, se buscaron indicadores de compromiso (IoCs) relacionados con el malware DarkSide para garantizar que no quedaran restos de la intrusión en la red.


- **Restauración y mejora**:
  - Una vez descifrado el sistema (o restaurado desde backups en caso de fallos con el descifrador), se procedió con la restauración progresiva de los servicios críticos, comenzando con las operaciones del oleoducto.
  - Se implementaron medidas de seguridad como la autenticación multifactor (MFA) en los accesos remotos y se cerraron puertos VPN antiguos.
  - En días posteriores, se colaboró con consultores para mejorar la segmentación de red, la monitorización continua 24/7 y la auditoría de sistemas en busca de otras vulnerabilidades.


- **Colaboración con autoridades y el sector**:
  - Colonial Pipeline compartió detalles técnicos del ataque con la CISA y el sector energético, alimentando alertas conjuntas y ayudando a prevenir futuros ataques en otras organizaciones.
  - Esta cooperación fue clave para prevenir un ataque similar en otras empresas del sector energético.


### 2.1.7. Clasificación del Incidente (Taxonomía)

<p>El incidente que afectó a Colonial Pipeline se clasifica como un <strong>ciberataque de tipo ransomware</strong>. El grupo responsable fue DarkSide, un actor de amenazas conocido por llevar a cabo ataques de ransomware. Este grupo cifró los sistemas de Colonial Pipeline y exigió un rescate para restaurar el acceso a los datos y sistemas comprometidos. La técnica empleada para este ataque es común en las campañas de ransomware, donde los atacantes buscan bloquear el acceso a los sistemas críticos de las organizaciones y extorsionarlas a cambio de una recompensa.</p>

<p>En cuanto al <strong>vector de ataque</strong>, los atacantes utilizaron <strong>credenciales filtradas</strong> para obtener acceso inicial a la red. Estas credenciales pertenecían a una cuenta de VPN de Colonial Pipeline que había sido comprometida y publicada en la dark web. A través de la circulación de estas credenciales en foros clandestinos, los atacantes pudieron acceder a la red sin ser detectados inicialmente, lo que les permitió llevar a cabo su ataque sin utilizar técnicas más complejas, como el phishing o explotación de vulnerabilidades de software.</p>

<p>Las <strong>técnicas utilizadas</strong> en este incidente incluyen principalmente el <strong>uso de credenciales válidas</strong> para ingresar a la red corporativa, seguido por la <strong>ejecución de ransomware</strong> en los sistemas afectados. Tras acceder a la red mediante la cuenta de VPN, los atacantes aprovecharon la falta de autenticación multifactor (MFA) en los servicios de acceso remoto para ganar acceso a sistemas críticos. Posteriormente, se movieron lateralmente dentro de la infraestructura utilizando herramientas comunes de movimiento lateral como <strong>Cobalt Strike</strong>, lo que les permitió escalar privilegios y extender el impacto del ataque.</p>

<p>El <strong>impacto</strong> del ataque fue significativo tanto en términos operativos como financieros. La interrupción operativa fue grave, ya que obligó a Colonial Pipeline a desconectar partes críticas de su infraestructura, incluido el oleoducto, lo que afectó el suministro de combustible en varias regiones de Estados Unidos. Además de la interrupción de los servicios, la empresa sufrió pérdidas financieras relacionadas con el pago del rescate y los costos derivados de la investigación, la recuperación y la mejora de sus sistemas de seguridad post-incidente. La reputación de la empresa también se vio gravemente afectada, ya que la exposición pública del ataque y las vulnerabilidades de seguridad evidenciaron deficiencias importantes en los controles de acceso de la organización.</p>

<p>Desde la perspectiva de la taxonomía del marco MITRE ATT&CK, este incidente puede clasificarse en las siguientes fases:</p>

<ul>
    <li><strong>Initial Access</strong>: Los atacantes lograron acceder a la red utilizando <strong>credenciales válidas</strong> obtenidas a través de filtraciones previas en la dark web.</li>
    <li><strong>Execution</strong>: El ataque culminó con la <strong>ejecución de ransomware</strong>, que cifró los sistemas comprometidos.</li>
    <li><strong>Persistence</strong>: Los atacantes utilizaron herramientas como <strong>Cobalt Strike</strong> para mantener su acceso a la red y moverse lateralmente dentro de la infraestructura.</li>
    <li><strong>Privilege Escalation</strong>: A medida que los atacantes se movían dentro de la red, escalaron privilegios para obtener acceso a sistemas más sensibles.</li>
    <li><strong>Impact</strong>: La interrupción de operaciones, así como las pérdidas económicas y reputacionales, fueron las consecuencias principales del ataque.</li>
</ul>

<p>Finalmente, según el marco de respuesta a incidentes, las fases de <strong>contención</strong>, <strong>erradicación</strong> y <strong>recuperación</strong> se implementaron en la respuesta de Colonial Pipeline. Se aislaron los sistemas comprometidos, se deshabilitaron las cuentas de acceso y se restauraron los servicios mediante descifradores y backups. A pesar de la interrupción, la acción rápida permitió a la empresa comenzar su proceso de recuperación y restauración de operaciones en un plazo relativamente corto.</p>

## 2.2. Pérdidas

<p>El ataque a Colonial Pipeline tuvo un impacto considerable en diversas áreas, tanto tangibles como intangibles. Las pérdidas no solo incluyeron costos directos como el pago del rescate, sino también gastos derivados de la interrupción operativa, la respuesta y la remediación, así como el daño a la reputación de la empresa. Estas consecuencias resaltan la importancia de una infraestructura de ciberseguridad robusta para prevenir incidentes de esta magnitud.</p>

### 2.2.1. Económicas

<p>Las pérdidas económicas derivadas del ataque a Colonial Pipeline son significativas y se pueden categorizar en varias áreas clave. La pérdida directa más evidente fue el <strong>pago de rescate</strong> de 75 BTC (aproximadamente 4,4 millones de dólares), aunque una parte de esos fondos (63,7 BTC) fue recuperada por el gobierno un mes después. Sin embargo, Colonial Pipeline no logró recuperar aproximadamente 2,1 millones de dólares debido a la fluctuación del valor de Bitcoin. A pesar de que muchas pólizas de ciberseguro cubren estos rescates, generalmente resultan en primas más altas para la empresa en el futuro.</p>

<p>En términos de <strong>pérdidas operativas</strong>, el impacto fue considerable debido a la interrupción de las operaciones. Colonial Pipeline dejó de transportar y vender combustible durante varios días, lo que resultó en la pérdida de ingresos por la venta de 2,5 millones de barriles de petróleo diarios. A pesar de los márgenes pequeños por barril, las pérdidas de ingresos en esos cinco días suman varios millones de dólares. Además, la empresa tuvo que reembolsar o no cobrar penalidades contractuales a proveedores por la falta de entrega, lo que también representó un costo importante.</p>

<p>Los <strong>costos de respuesta y remediación</strong> fueron otro factor económico relevante. Estos incluyen los gastos derivados de la contratación de firmas externas de respuesta como Mandiant, la asesoría legal, y los costos asociados con la adquisición de nuevos sistemas de hardware y software para reemplazar los comprometidos. Además, Colonial Pipeline anunció inversiones significativas para mejorar su ciberseguridad a largo plazo, lo que implica un aumento en su presupuesto de TI para implementar soluciones de autenticación multifactor (MFA), segmentación de red, y herramientas de detección y respuesta ante incidentes.</p>

<p>Finalmente, el incidente también provocó <strong>penalizaciones legales y regulatorias</strong>. Si bien Colonial Pipeline no fue multada de inmediato, el ataque dio lugar a nuevas normativas y directivas de seguridad impuestas por la Transportation Security Administration (TSA). El incumplimiento de estas directivas puede resultar en sanciones económicas adicionales. Además, las posibles demandas colectivas de partes afectadas, como clientes o proveedores, podrían generar más costos legales para la empresa.</p>

<table>
  <thead>
    <tr>
      <th><strong>Categoría</strong></th>
      <th><strong>Descripción</strong></th>
      <th><strong>Valor Estimado</strong></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Pago de Rescate</strong></td>
      <td>El pago inicial de 75 BTC (aproximadamente 4,4 millones de dólares) a los atacantes. A pesar de la recuperación parcial de 63,7 BTC, Colonial no recuperó 2,1 millones debido a la fluctuación del valor de Bitcoin.</td>
      <td>≈ $4,4 millones (75 BTC), con $2,1 millones no recuperados.</td>
    </tr>
    <tr>
      <td><strong>Pérdidas Operativas</strong></td>
      <td>La interrupción de las operaciones resultó en la pérdida de ingresos por la venta de 2,5 millones de barriles diarios. También hubo reembolsos o penalidades no cobradas a proveedores debido a la falta de entrega.</td>
      <td>Varias millones de dólares por ingresos perdidos.</td>
    </tr>
    <tr>
      <td><strong>Costos de Respuesta y Remediación</strong></td>
      <td>Contratación de firmas externas (Mandiant), asesoría legal, adquisición de hardware/software para reemplazar sistemas comprometidos, y gastos para mejorar la ciberseguridad.</td>
      <td>Haciendo inversiones adicionales por varios millones de dólares.</td>
    </tr>
    <tr>
      <td><strong>Penalizaciones Legales/Regulatorias</strong></td>
      <td>Posibles multas por incumplir las directivas de seguridad de la TSA, así como posibles demandas colectivas de clientes o proveedores afectados.</td>
      <td>Costos no estimados, pero potencialmente significativos por demandas legales y sanciones.</td>
    </tr>
  </tbody>
</table>

### 2.2.2. Reputacionales

<p>El ataque a Colonial Pipeline tuvo un impacto significativo en su reputación, tanto a nivel comercial como público. Las consecuencias no solo se limitan a los aspectos financieros, sino que también se reflejan en la percepción que los socios, clientes y el público en general tienen sobre la seguridad y confiabilidad de la empresa. A continuación se detallan los principales impactos reputacionales derivados del incidente:</p>

<ul>
  <li><strong>Desconfianza de los Socios Comerciales:</strong> El incidente expuso vulnerabilidades significativas en la infraestructura de seguridad de Colonial Pipeline. Esto pudo haber generado desconfianza en sus socios comerciales, quienes podrían reconsiderar futuras colaboraciones o compromisos con la empresa debido a la exposición de información sensible y la interrupción de servicios críticos.</li>

  <li><strong>Impacto en la Confianza del Público:</strong> Al ser un caso de alto perfil, Colonial Pipeline pasó a ser asociado con un ataque de ransomware que afectó un sistema crítico de infraestructura. Esto podría haber erosionado la confianza del público, especialmente en lo que respecta a la seguridad y fiabilidad del suministro de combustible.</li>

  <li><strong>Relaciones Públicas y Gestión de Crisis:</strong> Colonial Pipeline tuvo que desplegar esfuerzos significativos en relaciones públicas para reparar su imagen. La empresa invirtió recursos en campañas para demostrar su compromiso con la ciberseguridad y la mejora de sus sistemas de protección para evitar futuros ataques.</li>

  <li><strong>Posibles Restricciones Regulatorias:</strong> La pérdida de confianza generada por el ataque podría haber tenido implicaciones regulatorias, ya que los reguladores podrían imponer restricciones adicionales o exigencias más estrictas sobre la seguridad cibernética en el sector de la energía, lo que afecta indirectamente a Colonial Pipeline.</li>
</ul>

<p>En resumen, las consecuencias reputacionales del ataque son de largo alcance y podrían afectar la capacidad de Colonial Pipeline para operar de manera eficiente en el futuro, además de generar un costo indirecto asociado con la reconstrucción de su imagen pública y la restauración de la confianza entre sus socios y clientes.</p>

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

