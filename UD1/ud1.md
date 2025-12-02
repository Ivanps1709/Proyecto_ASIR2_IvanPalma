[Volver al índice general](../README.md)

# UD1 – Análisis del entorno y detección de necesidades tecnológicas

## Índice de apartados

- [ ] **1. Análisis del sector tecnológico**

Para empezar con el Proyecto Intermodular, he estado investigando cómo está el mercado laboral y tecnológico en mi entorno cercano, concretamente en **Sevilla y Andalucía**.

La conclusión principal es que el sector está en un momento muy bueno. No es solo una impresión mía; los datos de 2024 y 2025 muestran que Sevilla se está consolidando como un punto clave para la tecnología en el sur de Europa.

### Situación actual en Sevilla (2024-2025)

Lo que más destaca es el crecimiento del **Sevilla TechPark** (lo que siempre hemos llamado la Cartuja). Según las últimas noticias, el parque ha crecido un **13,7%** en actividad económica este último año. Esto significa que hay más empresas, más dinero moviéndose y, sobre todo, más necesidad de gente que sepa gestionar sistemas informáticos.

Pero no todo son grandes multinacionales. El tejido empresarial de nuestra zona sigue dependiendo mucho de las **PYMES (Pequeñas y Medianas Empresas)**. He notado que hay dos velocidades:

1. **Las empresas tecnológicas puras:** Que van a tope con la nube, IA y ciberseguridad avanzada.

2. **Las empresas "de toda la vida" (construcción, gestorías, logística):** Que se están viendo obligadas a digitalizarse a la fuerza porque si no, se quedan atrás o sufren ataques informáticos.

### Ámbitos de interés para un técnico ASIR

Mirando ofertas de trabajo y leyendo sobre las necesidades de las empresas locales, he visto que lo que más falta hace y donde nosotros podemos entrar es:

* **Oficina Virtual y Teletrabajo:** Muchas PYMES ya no tienen oficina física, pero necesitan trabajar como si la tuvieran. Configurar accesos remotos seguros (VPN) es clave.

* **Gestión de servidores y Nube:** No basta con tener un portátil en casa, necesitan centralizar la información para no depender de un solo dispositivo.

* **Ciberseguridad básica:** Al trabajar desde redes domésticas (WiFi de casa), los datos de la empresa corren peligro. Separar lo personal de lo profesional es una necesidad urgente.

En resumen, hay hueco de sobra para proponer proyectos de mejora de infraestructura, porque aunque el sector crece, la seguridad y la profesionalización de los sistemas básicos en las empresas medianas todavía tiene mucho margen de mejora.
                               
- [ ] **2. Selección de la empresa o contexto de trabajo**

Para este proyecto he seleccionado una empresa real de mi entorno, donde trabaja un familiar directo, lo que me permite conocer de primera mano sus carencias tecnológicas.

* **Nombre de la empresa:** *Carvajal Construcciones y Reformas*.

* **Ubicación:** Coria del Río (Sevilla).

* **Actividad:** Empresa con más de 25 años de experiencia en construcción y reformas integrales.

* **Estructura:** No disponen de oficina física fija ("oficina virtual"). El gerente gestiona la empresa desde su domicilio particular y los encargados (como mi padre) coordinan las obras in-situ.

* **Infraestructura actual (El problema):** La situación es crítica a nivel de seguridad y operatividad:
  * **Dependencia total de un portátil:** Toda la facturación y gestión está en el portátil personal del jefe, conectado al WiFi doméstico de su casa.
  * **Red Insegura:** Los datos de la empresa conviven en la misma red que los dispositivos personales de la familia (móviles, consolas, TV), sin segmentación ni firewall profesional.
  * **Falta de Colaboración:** Si mi padre o los otros encargados necesitan consultar un presupuesto o un plano, no pueden acceder al sistema. Tienen que llamar por teléfono o esperar a verse en persona.
  * **Web y Correo:** Web básica en WordPress y uso de correos gratuitos no corporativos.
                               
- [ ] **3. Identificación de necesidades tecnológicas**

Al no tener sede física, la necesidad principal es crear una "Sede Digital" segura, integrando servicios de red, administración de sistemas, bases de datos y seguridad.

### Necesidades detectadas:

1. **Centralización y Seguridad (Módulos ASO y SEG):** Es vital sacar los datos del portátil del jefe. Necesitan un servidor central con control de acceso estricto y copias de seguridad.

2. **Acceso Remoto y Redes (Módulo SRED):** Los encargados necesitan conectarse vía VPN desde las obras. Además, es urgente segmentar la red en casa del jefe para separar lo doméstico de lo empresarial.

3. **Web y Datos (Módulos IAW y ABD):** La web actual es precaria. Necesitan migrar el WordPress a un hosting profesional, lo que implica gestionar el servidor web y la **base de datos** subyacente de forma segura.

### Propuesta de Proyecto:

Mi proyecto se titula **"Despliegue de Oficina Virtual SOHO con Servicios Integrados"**. Consistirá en:

* **Infraestructura Híbrida (ASO/SRED):** Servidor local actuando como Controlador de Dominio y Servidor de Archivos, con servicios DHCP y DNS configurados.

* **Seguridad Perimetral (SEG):** Implementación de Firewall y VPN para cifrar las conexiones de los trabajadores remotos.

* **Servicios Web y Base de Datos (IAW/ABD):** Migración del WordPress corporativo, gestionando la base de datos SQL de clientes/proyectos y configurando el servicio de correo.
                          
- [ ] **4. Oportunidades y viabilidad del proyecto**

Este proyecto es ideal porque resuelve un problema real y permite aplicar todas las competencias del ciclo ASIR:

* **Viabilidad Técnica:** Usaremos tecnologías estándar (Windows Server, MySQL, Apache/Nginx, OpenVPN) que funcionan perfectamente sobre conexiones domésticas modernas.

* **Viabilidad Económica:** La inversión es mínima (reutilización de hardware + licencias), pero el retorno en **seguridad** es incalculable para la empresa.

* **Cobertura Curricular:** El proyecto permite demostrar conocimientos en Administración de Sistemas (ASO), Redes (SRED), Seguridad (SEG), Aplicaciones Web (IAW) y Bases de Datos (ABD).
                             
- [ ] **5. Obligaciones legales y normativas**

Al tratar datos de clientes en un domicilio particular, la normativa es estricta:

* **RGPD (Datos Personales):** Debemos garantizar que los datos de la empresa estén cifrados y separados de los datos personales de la familia. El servidor debe tener control de acceso estricto.

* **Teletrabajo:** El sistema debe cumplir con los estándares de seguridad para el trabajo remoto (conexiones cifradas VPN), evitando el uso de herramientas de control remoto inseguras.

* **LSSI:** Adecuación legal de la página web y correos electrónicos.
                                
- [ ] **6. Guion inicial del proyecto**

El plan de trabajo integra todas las áreas del ciclo formativo:

1. **Fase 1: Redes y Seguridad (SRED/SEG).**
   * Diseño de VLANs para aislar la red de empresa en el domicilio.
   * Planificación de direccionamiento IP y túneles VPN.

2. **Fase 2: Sistemas Operativos (ASO).**
   * Instalación de Windows Server y promoción a Controlador de Dominio (AD).
   * Gestión de usuarios (Gerente, Encargados) y permisos NTFS.

3. **Fase 3: Servicios de Red (SRED).**
   * Configuración de servicios DHCP y DNS internos.
   * Configuración del acceso remoto seguro (VPN).

4. **Fase 4: Web y Bases de Datos (IAW/ABD).**
   * Migración del WordPress a hosting propio.
   * Gestión y aseguramiento de la **Base de Datos** de clientes.

5. **Fase 5: Mantenimiento y Seguridad (SEG).**
   * Automatización de backups 3-2-1 (Datos + Base de Datos).
   * Implementación de Firewall perimetral.
                                
## Enlaces a recursos de la unidad

- [Documentos de la unidad](./documentos/)
- [Diagramas e imágenes](./img/)

  ## Bibliografía / Webgrafía 
- Autor1, Título del libro o artículo, Editorial/Año.
- Sitio web oficial:
  
  - **eCitySevilla:** *"Sevilla TechPark crece un 13,7% en 2024 y factura ya 5.513 millones de euros"*. [Enlace](https://ecitysevilla.com/sevilla-techpark-crece-un-137-en-2024-y-factura-ya-5-513-millones-de-euros/)
  - **Al Andalus Innovation Venture:** *"Andalucía afianza su posición en el ecosistema tech español con 714 empresas y más de 747 millones de euros en facturación"*. [Enlace](https://alandalusinnovation.com/andalucia-afianza-su-posicion-en-el-ecosistema-tech-espanol-con-714-empresas-y-mas-de-747-millones-de-euros-en-facturacion/)
  - **Carvajal Construcciones:** Sitio web corporativo de la empresa analizada. [Enlace](https://carvajalconstrucciones.com/)
  - **Sevilla TechPark:** Actualidad y noticias del parque tecnológico. [Enlace](https://sevillatechpark.es/actualidad/)
  - **InfoJobs:** Análisis de la demanda de perfiles técnicos en Sevilla. [Enlace](https://www.infojobs.net/)
             
- Tutoriales y guías recomendadas: [Enlace](https://www.ejemplo2.com)

