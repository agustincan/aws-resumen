# Resumen de Servicios de AWS para el Examen Cloud Architect

**Fundamentos:**

* **Regiones y Zonas de Disponibilidad (AZs):** La infraestructura global de AWS. Las Regiones son áreas geográficas y las AZs son ubicaciones distintas dentro de una Región, diseñadas para la tolerancia a fallos.
* **VPC (Virtual Private Cloud):** Red virtual privada y aislada dentro de AWS, donde puedes lanzar tus recursos. Control total sobre el entorno de red.
* **IAM (Identity and Access Management):** Control de acceso y permisos para los recursos de AWS. Usuarios, grupos, roles y políticas para una seguridad granular.

**Computación:**

* **EC2 (Elastic Compute Cloud):** Servidores virtuales escalables en la nube. Ofrece varios tipos de instancias optimizadas para diferentes cargas de trabajo.
* **Lambda:** Servicio de computación sin servidor (serverless). Ejecuta código sin aprovisionar ni administrar servidores. Se paga por la computación consumida.
* **Elastic Beanstalk:** Plataforma como servicio (PaaS) para desplegar y administrar aplicaciones web. Abstrae la infraestructura subyacente.
* **ECS (Elastic Container Service) y EKS (Elastic Kubernetes Service):** Servicios para ejecutar y administrar contenedores Docker. ECS es la solución nativa de AWS, mientras que EKS es Kubernetes gestionado.
* **App Runner:** Servicio PaaS para desplegar aplicaciones web y APIs en contenedores directamente desde el código fuente o un contenedor.

**Almacenamiento:**

* **S3 (Simple Storage Service):** Almacenamiento de objetos altamente escalable y duradero. Ideal para copias de seguridad, archivos estáticos y data lakes.
* **EBS (Elastic Block Store):** Almacenamiento de bloques persistente para usar con instancias EC2. Similar a discos duros virtuales.
* **EFS (Elastic File System):** Almacenamiento de archivos escalable y compartido para instancias EC2. Compatible con el sistema de archivos Network File System (NFS).
* **S3 Glacier y S3 Glacier Deep Archive:** Almacenamiento de archivos de bajo costo para archivado a largo plazo. Diferentes opciones de recuperación con distintos tiempos y costos.
* **AWS Storage Gateway:** Servicio híbrido que conecta tu almacenamiento on-premise con la nube de AWS.

**Bases de Datos:**

* **RDS (Relational Database Service):** Servicio de bases de datos relacionales gestionado. Soporta MySQL, PostgreSQL, MariaDB, Oracle y SQL Server.
* **DynamoDB:** Base de datos NoSQL clave-valor altamente escalable y de baja latencia.
* **Aurora:** Base de datos relacional compatible con MySQL y PostgreSQL, optimizada para la nube de AWS con mejor rendimiento y disponibilidad.
* **Redshift:** Almacén de datos (data warehouse) rápido y escalable para análisis.
* **ElastiCache:** Servicios de caché en memoria compatibles con Redis y Memcached para mejorar el rendimiento de las aplicaciones.
* **Neptune:** Servicio de base de datos de grafos totalmente gestionado.
* **Timestream:** Base de datos de series temporales rápida y escalable para aplicaciones de IoT y análisis operacional.
* **QLDB (Quantum Ledger Database):** Base de datos de libro mayor inmutable y criptográficamente verificable.

**Redes y Distribución de Contenido:**

* **Route 53:** Servicio de DNS (Sistema de Nombres de Dominio) altamente disponible y escalable.
* **CloudFront:** Servicio de red de entrega de contenido (CDN) para distribuir contenido estático y dinámico a nivel global con baja latencia y alta velocidad de transferencia.
* **ELB (Elastic Load Balancing):** Distribuye el tráfico entrante entre múltiples instancias EC2 para mejorar la disponibilidad y la escalabilidad. Incluye Application Load Balancer (HTTP/HTTPS), Network Load Balancer (TCP/UDP) y Classic Load Balancer (legado).
* **API Gateway:** Servicio para crear, publicar, mantener, monitorizar y proteger APIs a cualquier escala.
* **Direct Connect:** Conexión de red dedicada desde tu entorno on-premise a AWS.
* **VPC Peering:** Conexión de red entre dos VPCs que permite el enrutamiento privado del tráfico entre ellas.
* **Transit Gateway:** Conecta múltiples VPCs y redes on-premise a través de un único punto centralizado.
* **PrivateLink:** Proporciona conectividad privada entre VPCs, servicios de AWS y tus servicios on-premise, sin exponer el tráfico a la internet pública.

**Seguridad, Identidad y Cumplimiento:**

* **IAM (revisitado):** Fundamental para la seguridad.
* **Security Hub:** Servicio para gestionar la postura de seguridad y realizar comprobaciones de seguridad.
* **GuardDuty:** Servicio de detección inteligente de amenazas que monitoriza la actividad maliciosa y el comportamiento inesperado.
* **Inspector:** Servicio automatizado de evaluación de seguridad para identificar vulnerabilidades en las instancias EC2 y contenedores.
* **WAF (Web Application Firewall):** Protege las aplicaciones web de ataques comunes como inyecciones SQL y scripting entre sitios (XSS).
* **Secrets Manager:** Almacena y gestiona de forma segura secretos como contraseñas, claves de API y otros datos confidenciales.
* **KMS (Key Management Service):** Servicio gestionado para crear y gestionar claves de cifrado.
* **CloudHSM (Hardware Security Module):** Módulos de seguridad de hardware dedicados para el almacenamiento de claves de cifrado con controles de cumplimiento normativo.
* **Certificate Manager (ACM):** Aprovisiona, gestiona y despliega certificados SSL/TLS para su uso con servicios de AWS.
* **Cognito:** Servicio para gestionar la identidad y el acceso de los usuarios a aplicaciones web y móviles.
* **Artifact:** Portal de acceso bajo demanda a los informes de cumplimiento de AWS (SOC, PCI, ISO, etc.).

**Herramientas de Gestión y Monitorización:**

* **CloudWatch:** Servicio de monitorización y observabilidad para recursos y aplicaciones de AWS. Recopila métricas, logs y eventos. Permite configurar alarmas y dashboards.
* **CloudTrail:** Registra la actividad de la API de AWS en tu cuenta, proporcionando un registro de auditoría de las acciones realizadas.
* **Config:** Realiza un seguimiento y evalúa las configuraciones de los recursos de AWS. Permite automatizar la evaluación del cumplimiento.
* **Systems Manager:** Proporciona una visión unificada para la gestión operativa y la automatización de tus recursos de AWS.
* **Trusted Advisor:** Ofrece recomendaciones para optimizar tu infraestructura de AWS en cuanto a costos, seguridad, tolerancia a fallos, rendimiento y límites de servicio.
* **Service Catalog:** Permite a las organizaciones crear y gestionar catálogos de servicios de TI aprobados para su uso en AWS.
* **CloudFormation:** Servicio de infraestructura como código (IaC) que te permite definir y desplegar la infraestructura de AWS como código.
* **Terraform:** Otra popular herramienta de IaC de terceros compatible con AWS.

**Análisis de Datos:**

* **S3 (revisitado):** A menudo utilizado como data lake.
* **Athena:** Servicio de consultas SQL interactivo sin servidor para analizar datos en S3.
* **Glue:** Servicio ETL (Extracción, Transformación y Carga) totalmente gestionado.
* **EMR (Elastic MapReduce):** Plataforma gestionada de Hadoop y Spark para procesar grandes volúmenes de datos.
* **Kinesis:** Plataforma para la transmisión de datos en tiempo real. Incluye Kinesis Data Streams, Kinesis Data Firehose y Kinesis Data Analytics.
* **QuickSight:** Servicio de inteligencia empresarial (BI) rápido y escalable para crear visualizaciones y dashboards.

**Integración de Aplicaciones:**

* **SQS (Simple Queue Service):** Servicio de colas de mensajes totalmente gestionado para desacoplar componentes de aplicaciones.
* **SNS (Simple Notification Service):** Servicio de mensajería de publicación/suscripción (pub/sub) para enviar notificaciones.
* **Step Functions:** Servicio de flujo de trabajo visual para coordinar aplicaciones distribuidas y microservicios.
* **EventBridge:** Bus de eventos sin servidor que permite conectar aplicaciones con datos de diversas fuentes.

**Inteligencia Artificial y Machine Learning:**

* **SageMaker:** Plataforma integral de machine learning para construir, entrenar y desplegar modelos de ML.
* **Rekognition:** Servicio de análisis de imágenes y videos.
* **Polly:** Servicio de texto a voz (TTS).
* **Lex:** Servicio para construir interfaces conversacionales (chatbots).
* **Translate:** Servicio de traducción automática de idiomas.
* **Comprehend:** Servicio de procesamiento de lenguaje natural (NLP) para extraer información de texto.

**Internet de las Cosas (IoT):**

* **IoT Core:** Plataforma gestionada para conectar, asegurar y gestionar dispositivos IoT.
* **IoT Greengrass:** Extiende las capacidades de la nube de AWS a los dispositivos locales.

**Consideraciones Clave para el Examen:**

* **Well-Architected Framework:** Comprende los cinco pilares: excelencia operativa, seguridad, fiabilidad, eficiencia de costos y sostenibilidad.
* **Escalabilidad y Elasticidad:** Cómo diseñar arquitecturas que puedan escalar automáticamente para manejar cargas variables.
* **Alta Disponibilidad y Tolerancia a Fallos:** Diseñar sistemas que sigan funcionando en caso de fallos.
* **Optimización de Costos:** Elegir los servicios y configuraciones más rentables.
* **Seguridad en la Nube:** Implementar las mejores prácticas de seguridad en todos los niveles.
* **Arquitecturas Híbridas:** Comprender cómo integrar entornos on-premise con AWS.
* **Serverless:** Conocer los casos de uso y beneficios de los servicios sin servidor.
* **Contenedores:** Entender cuándo y cómo utilizar ECS y EKS.
