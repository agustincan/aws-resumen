# 🚀 Resumen de Servicios AWS - Guía para Examen Cloud Architect

*Actualizado: Abril 2025*  
*Fuente: AWS Documentation + Examen SAA-C03*  

---

## 🔹 **Categorías Principales**

### 1. **Computación (Compute)**
- **EC2** → Máquinas virtuales escalables (On-Demand, Spot, Reserved Instances).
- **Lambda** → Serverless (ejecución por eventos, pago por milisegundo).
- **ECS/EKS** → Contenedores Docker (ECS = AWS, EKS = Kubernetes).
- **Fargate** → Serverless para contenedores (sin gestionar servidores).
- **Batch** → Procesamiento por lotes (batch jobs).

### 2. **Almacenamiento (Storage)**
- **S3** → Objetos escalable (99.999999999% durabilidad).
  - *Clases*: Standard, Intelligent-Tiering, Glacier (archivo).
- **EBS** → Discos para EC2 (SSD/HDD, snapshots).
- **EFS** → Sistema de archivos compartido (NFS).
- **FSx** → Para Windows (SMB) o Lustre (HPC).

### 3. **Bases de Datos (Database)**
- **RDS** → Bases relacionales (MySQL, PostgreSQL, Aurora).
- **DynamoDB** → NoSQL clave-valor (autoescalable).
- **Redshift** → Data Warehouse (análisis de grandes volúmenes).
- **ElastiCache** → Caché en memoria (Redis/Memcached).

### 4. **Redes (Networking)**
- **VPC** → Red privada virtual (subnets, route tables).
- **CloudFront** → CDN (baja latencia, DDoS protection).
- **Route 53** → DNS escalable + registro de dominios.
- **API Gateway** → Publicar APIs REST/WebSocket.

### 5. **Seguridad (Security)**
- **IAM** → Gestión de usuarios/permisos (políticas JSON).
- **KMS** → Cifrado de datos (claves maestras).
- **WAF** → Firewall para aplicaciones web (protege de SQLi, XSS).
- **Shield** → Protección contra DDoS.

### 6. **Monitorización (Monitoring)**
- **CloudWatch** → Métricas y logs (alarmas).
- **CloudTrail** → Auditoría de llamadas API.
- **X-Ray** → Traza solicitudes en microservicios.

### 7. **Integración (Application Integration)**
- **SQS** → Colas de mensajes (desacopla aplicaciones).
- **SNS** → Notificaciones push (SMS, email, HTTP).
- **EventBridge** → Bus de eventos (react a cambios).

### 8. **Migración (Migration)**
- **DMS** → Migración de bases de datos.
- **Snowball** → Transferencia física de datos (petabytes).

### 9. **Machine Learning**
- **SageMaker** → Entrenar/desplegar modelos ML.
- **Rekognition** → Análisis de imágenes/video.

---

## 🔥 **Servicios Clave para el Examen**
| Servicio | Caso de Uso | Importancia |
|----------|------------|------------|
| **S3**   | Almacenamiento estático, hosting web | ⭐⭐⭐⭐⭐ |
| **EC2**  | Aplicaciones generales (Linux/Windows) | ⭐⭐⭐⭐⭐ |
| **IAM**  | Seguridad y permisos | ⭐⭐⭐⭐⭐ |
| **Lambda** | Eventos puntuales (ej: procesar uploads a S3) | ⭐⭐⭐⭐ |
| **RDS**  | Bases de datos SQL gestionadas | ⭐⭐⭐⭐ |

---

## 📌 **Tips para el Examen**
1. **Patrones comunes**:  
   - Escalado horizontal → Auto Scaling + ELB.  
   - Alta disponibilidad → Multi-AZ (RDS), S3 Cross-Region Replication.  
2. **Preguntas frecuentes**:  
   - Diferencias entre **S3 Standard vs Glacier**.  
   - Cuándo usar **DynamoDB vs RDS**.  
   - Cómo proteger datos en tránsito/reposo (**KMS + TLS**).  

---

> 💡 **Descarga este resumen como archivo .md** [aquí](#) (simulado) o cópialo manualmente.  
> ✨ *Revisa siempre la [documentación oficial de AWS](https://aws.amazon.com/es/documentation/).*
