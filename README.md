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

### 2.1.2. Consecuencias

#### 2.1.2.1. Activos Afectados
#### 2.1.2.2. Servicios Afectados
#### 2.1.2.3. Impacto
#### 2.1.2.4. Tiempo de indisponibilidad

### 2.1.3. Proceso de Respuesta

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

