[Volver al índice general](../README.md)

# UD1 – Análisis del entorno y detección de necesidades tecnológicas

## Índice de apartados

- [ ] **1. Análisis del sector tecnológico**
                               
- [ ] **2. Selección de la empresa o contexto de trabajo**

- [ ] **3. Identificación de necesidades tecnológicas**
                          
- [ ] **4. Oportunidades y viabilidad del proyecto**

- [ ] **5. Obligaciones legales y normativas**

- [ ] **6. Guion inicial del proyecto**

# 1. Análisis del sector tecnológico

El sector TIC en Andalucía actúa como motor económico regional, destacando Sevilla y el PCT Cartuja con un crecimiento de facturación cercano al 14% anual. Este ecosistema fomenta la aparición de micro-consultoras tecnológicas que digitalizan a terceros, pero que paradójicamente suelen descuidar su propia infraestructura interna ("Shadow IT"), operando con sistemas domésticos y sin políticas de seguridad corporativa, lo que limita su escalabilidad y seguridad.

Ante este escenario, surge la necesidad crítica de profesionalizar la gestión interna de estas PYMES tecnológicas. Se requiere la intervención de perfiles técnicos superiores (ASIR) para implementar arquitecturas de "Confianza Cero" (Zero Trust), centralizar la identidad corporativa y segmentar redes, transformando infraestructuras precarias en entornos empresariales seguros y auditables que cumplan con los estándares del mercado.

# 2. Selección de la empresa o contexto de trabajo

La empresa seleccionada es **INFOSUR SOLUCIONES INFORMÁTICAS PARA LA GESTIÓN EMPRESARIAL S.L.**, ubicada en el Polígono Industrial Calonge de Sevilla (Calle D, Nave 2). Es una consultora técnica consolidada que ofrece servicios de mantenimiento integral, desarrollo web y soporte a empresas. Su estructura organizativa es ágil y distribuida: cuenta con una Dirección Técnica que supervisa proyectos, un equipo de desarrollo y sistemas que opera en modelo híbrido (presencial/remoto) y un área administrativa, adaptándose dinámicamente a las necesidades de sus clientes locales.

A pesar de su actividad tecnológica, la auditoría interna para este proyecto revela una infraestructura propia deficiente ("En casa del herrero, cuchillo de palo"). La empresa carece de un dominio interno (Active Directory) para gestionar a sus propios empleados, utiliza métodos inseguros para compartir credenciales de administración y no dispone de segmentación de red entre los entornos de pruebas y los corporativos. Esta situación simulada plantea riesgos de seguridad inaceptables y justifica la reingeniería completa de sus sistemas internos.

# 3. Identificación de necesidades tecnológicas

Se ha detectado una vulnerabilidad crítica en la gestión de identidades y accesos, ya que la falta de un servidor centralizado impide controlar qué empleado accede a qué recursos, poniendo en riesgo los datos de los clientes. Adicionalmente, la red plana actual mezcla tráfico de desarrollo potencialmente peligroso con datos administrativos, y la carencia de una VPN corporativa obliga a exponer servicios internos a internet de forma insegura para el teletrabajo.

Para solventar estas carencias, se propone el proyecto "Despliegue de Infraestructura Segura para Consultora TIC". La solución incluye la implementación de Windows Server como Controlador de Dominio (AD DS) para centralizar usuarios y equipos, el despliegue de una red segmentada con VLANs y Firewall perimetral, y la configuración de una VPN Site-to-Site. Se complementará con la migración de servicios web a una infraestructura LAMP propia y un sistema de backups automatizado.

# 4. Oportunidades y viabilidad del proyecto

La viabilidad técnica está asegurada al utilizar estándares de industria ampliamente soportados (Windows Server, Linux, OpenVPN) y hardware de servidor accesible o virtualización, aprovechando el conocimiento previo del personal técnico de la empresa. El proyecto permite transformar una debilidad interna en una fortaleza comercial, utilizando la nueva infraestructura segura como escaparate de buenas prácticas ante los clientes.

Desde la perspectiva económica y académica, la inversión es mínima en comparación con el riesgo mitigado de sanciones por RGPD o pérdida de reputación. Académicamente, el proyecto es idóneo para ASIR al integrar transversalmente la administración de sistemas operativos, la seguridad de redes, la gestión de bases de datos y la implantación de aplicaciones web en un escenario realista y profesional.

[Image of gráfico ROI retorno inversión seguridad]

# 5. Obligaciones legales y normativas

El proyecto garantiza el cumplimiento del RGPD y la LOPDGDD mediante medidas de seguridad técnicas como el cifrado de datos (BitLocker), listas de control de acceso (ACLs) y registros de auditoría obligatorios para empresas que tratan datos de terceros. También se asegura la adecuación a la LSSI-CE en los servicios web corporativos y comunicaciones electrónicas.

En materia laboral, se realizará una auditoría de licencias de software para asegurar la Propiedad Intelectual y se aplicará la normativa de Prevención de Riesgos Laborales (PRL) específica para teletrabajo y uso de Pantallas de Visualización de Datos (RD 488/1997), asegurando la ergonomía de los puestos técnicos remotos.

# 6. Guion inicial del proyecto

El cronograma se divide en cuatro fases: la Fase I (Redes y Seguridad) establecerá el perímetro seguro con Firewall, VLANs y VPN; la Fase II (Sistemas) desplegará el Controlador de Dominio, usuarios y políticas GPO.

La Fase III (Servicios) migrará la web e intranet a servidores LAMP propios y base de datos centralizada; finalmente, la Fase IV (Mantenimiento) activará los backups automatizados y la documentación final, asegurando una transición ordenada sin afectar la operatividad diaria.

[Image of diagrama de Gantt fases proyecto]

## Enlaces a recursos de la unidad

- [Documentos de la unidad](./documentos/)
- [Diagramas e imágenes](./img/)

  ## Bibliografía / Webgrafía 
- Sitio web oficial:

  - * **Sevilla TechPark (PCT Cartuja):** *Portal oficial del parque tecnológico y empresarial*.
    [https://www.pctcartuja.es/](https://www.pctcartuja.es/)

  - * **INCIBE (Instituto Nacional de Ciberseguridad):** *Portal para empresas y guías de seguridad*.
    [https://www.incibe.es/empresas](https://www.incibe.es/empresas)

  - * **BOE (Boletín Oficial del Estado):** *Legislación consolidada*.
    [https://www.boe.es/](https://www.boe.es/)

  - * **AEPD (Agencia Española de Protección de Datos):** *Guías y herramientas de cumplimiento*.
    [https://www.aepd.es/](https://www.aepd.es/)
      

