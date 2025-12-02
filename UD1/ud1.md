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

Al no tener sede física, la necesidad principal es crear una "Sede Digital" segura.

### Necesidades detectadas:

1. **Centralización y Seguridad (El Servidor):** Es vital sacar los datos del disco duro del portátil del jefe. Necesitan un servidor central (puede ser físico en casa del jefe o híbrido) que almacene todo con copias de seguridad automáticas (RAID + Backup externo).

2. **Acceso Remoto (VPN):** Los encargados de obra (como mi padre) necesitan poder conectarse desde sus casas o móviles para ver planos, partes de trabajo o facturas sin tener que ir a casa del jefe.

3. **Separación de Redes (VLAN):** En casa del jefe, es necesario separar el tráfico de la empresa del tráfico doméstico para evitar que un virus en la tablet de un familiar infecte la contabilidad de la empresa.

4. **Identidad Digital:** Profesionalizar el correo y la web para dar imagen de empresa seria.

### Propuesta de Proyecto:

Mi proyecto se titula **"Despliegue de Oficina Virtual Segura y Centralización de Datos (SOHO)"**. Consistirá en:

* **Instalación de Servidor Micro:** Configuración de un equipo servidor en el domicilio del gerente que actuará como Controlador de Dominio y Servidor de Archivos.

* **VPN Site-to-Site / Client-to-Site:** Configuración de una red privada virtual para que los empleados accedan al servidor de forma segura desde sus ubicaciones.

* **Directorio Activo:** Gestión de usuarios para controlar quién accede a qué (Jefe: Todo, Encargados: Obras, Administrativo: Facturas).
                
- [ ] **4. Oportunidades y viabilidad del proyecto**

Este proyecto es ideal porque resuelve un problema real de las PYMES actuales: la falta de oficina física.

* **Viabilidad Técnica:** Usaremos tecnologías estándar (Windows Server, OpenVPN/WireGuard) que funcionan perfectamente sobre conexiones de fibra domésticas. No hace falta obra civil.

* **Viabilidad Económica:** La inversión es mínima (un servidor de entrada o reutilizar un PC potente + licencias), pero el retorno es la **seguridad total** de que la empresa no perderá sus datos si se rompe un portátil.

* **Mejora Operativa:** Permitirá a mi padre y al resto del equipo trabajar de forma asíncrona y remota, modernizando la gestión de la empresa.
                
- [ ] **5. Obligaciones legales y normativas**

Al tratar datos de clientes en un domicilio particular, la normativa es estricta:

* **RGPD (Datos Personales):** Debemos garantizar que los datos de la empresa estén cifrados y separados de los datos personales de la familia. El servidor debe tener control de acceso estricto.

* **Teletrabajo:** El sistema debe cumplir con los estándares de seguridad para el trabajo remoto (conexiones cifradas VPN), evitando el uso de herramientas de control remoto inseguras (como TeamViewer gratuito sin contraseña).

* **LSSI:** Adecuación legal de la página web y correos electrónicos.
                
- [ ] **6. Guion inicial del proyecto**

El plan de trabajo para la "Informatización SOHO (Small Office Home Office)":

1. **Fase 1: Diseño de la Red Segura.**
   * Diseño de la segmentación de red en el domicilio del gerente (VLAN Empresa vs VLAN Casa).
   * Planificación del direccionamiento IP y túneles VPN.

2. **Fase 2: Instalación del Servidor Central.**
   * Puesta en marcha del hardware (Servidor).
   * Instalación de Windows Server y promoción a Controlador de Dominio.

3. **Fase 3: Gestión de Usuarios y Archivos.**
   * Creación de usuarios (Gerente, Encargados).
   * Configuración de carpetas compartidas y permisos NTFS.

4. **Fase 4: Acceso Remoto y Conectividad.**
   * Configuración del servidor VPN para acceso externo seguro.
   * Configuración de los clientes (portátiles de encargados) para conectar a la VPN.

5. **Fase 5: Servicios Web y Correo.**
   * Profesionalización del dominio y configuración de cuentas de correo.

6. **Fase 6: Seguridad y Documentación.**
   * Automatización de backups (3-2-1).
   * Manual de conexión remota para los empleados.
                
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

