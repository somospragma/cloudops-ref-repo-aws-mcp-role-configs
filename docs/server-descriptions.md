# Descripción de Servidores MCP

## 🔧 Servidores Básicos

### aws-api
**Paquete**: `awslabs.aws-api-mcp-server`
**Descripción**: Interacción directa con servicios AWS via AWS CLI
**Casos de uso**: 
- Gestión de recursos AWS
- Consultas de estado de servicios
- Operaciones CRUD en recursos

### aws-knowledge  
**Paquete**: `awslabs.aws-knowledge-mcp-server`
**Descripción**: Acceso a documentación actualizada de AWS
**Casos de uso**:
- Consulta de mejores prácticas
- Referencias de API
- Guías de implementación

## 🏗️ Infraestructura como Código

### aws-cdk
**Paquete**: `awslabs.cdk-mcp-server`
**Descripción**: Desarrollo con AWS CDK y cumplimiento de seguridad
**Casos de uso**:
- Generación de código CDK
- Validación de seguridad
- Patrones de arquitectura

### aws-terraform
**Paquete**: `awslabs.terraform-mcp-server`
**Descripción**: Flujos de trabajo Terraform con escaneo de seguridad
**Casos de uso**:
- Gestión de infraestructura Terraform
- Escaneo de vulnerabilidades
- Documentación de recursos

### aws-cloudformation
**Paquete**: `awslabs.cfn-mcp-server`
**Descripción**: Gestión directa de recursos CloudFormation
**Casos de uso**:
- Despliegue de stacks
- Gestión de recursos via Cloud Control API
- Plantillas CloudFormation

## 💰 Costos y Pricing

### aws-pricing
**Paquete**: `awslabs.aws-pricing-mcp-server`
**Descripción**: Estimación de costos y análisis de pricing
**Casos de uso**:
- Cálculo de costos pre-despliegue
- Comparación de opciones
- Optimización de costos

### cost-explorer
**Paquete**: `awslabs.cost-explorer-mcp-server`
**Descripción**: Análisis detallado de costos históricos
**Casos de uso**:
- Reportes de costos
- Análisis de tendencias
- Identificación de ahorros

## 📊 Monitoreo y Observabilidad

### cloudwatch
**Paquete**: `awslabs.cloudwatch-mcp-server`
**Descripción**: Métricas, alarmas y logs de CloudWatch
**Casos de uso**:
- Monitoreo de infraestructura
- Análisis de logs
- Configuración de alarmas

### cloudwatch-appsignals
**Paquete**: `awslabs.cloudwatch-appsignals-mcp-server`
**Descripción**: Monitoreo de aplicaciones e insights de rendimiento
**Casos de uso**:
- APM (Application Performance Monitoring)
- Trazabilidad de requests
- Métricas de aplicación

## 🗄️ Bases de Datos

### dynamodb
**Paquete**: `awslabs.dynamodb-mcp-server`
**Descripción**: Operaciones completas DynamoDB
**Casos de uso**:
- Gestión de tablas
- Consultas y operaciones CRUD
- Configuración de índices

### aurora-postgresql
**Paquete**: `awslabs.postgres-mcp-server`
**Descripción**: Operaciones PostgreSQL via RDS Data API
**Casos de uso**:
- Consultas SQL
- Gestión de bases de datos
- Análisis de rendimiento

### aurora-mysql
**Paquete**: `awslabs.mysql-mcp-server`
**Descripción**: Operaciones MySQL via RDS Data API
**Casos de uso**:
- Consultas SQL
- Administración de BD
- Optimización de queries

### aurora-dsql
**Paquete**: `awslabs.aurora-dsql-mcp-server`
**Descripción**: SQL distribuido con compatibilidad PostgreSQL
**Casos de uso**:
- Consultas distribuidas
- Escalabilidad horizontal
- Análisis de datos

### documentdb
**Paquete**: `awslabs.documentdb-mcp-server`
**Descripción**: Base de datos compatible con MongoDB
**Casos de uso**:
- Operaciones NoSQL
- Gestión de documentos
- Consultas complejas

### elasticache
**Paquete**: `awslabs.elasticache-mcp-server`
**Descripción**: Operaciones completas de ElastiCache
**Casos de uso**:
- Gestión de caché
- Optimización de rendimiento
- Configuración de clusters

### redshift
**Paquete**: `awslabs.redshift-mcp-server`
**Descripción**: Data warehouse y análisis
**Casos de uso**:
- Consultas analíticas
- Gestión de clusters
- ETL y procesamiento

## 🐳 Contenedores y Orquestación

### eks
**Paquete**: `awslabs.eks-mcp-server`
**Descripción**: Gestión de clusters Kubernetes
**Casos de uso**:
- Administración de clusters EKS
- Despliegue de aplicaciones
- Gestión de nodos

### ecs
**Paquete**: `awslabs.ecs-mcp-server`
**Descripción**: Orquestación de contenedores
**Casos de uso**:
- Gestión de servicios ECS
- Configuración de tasks
- Escalado automático

## 🎨 Herramientas Adicionales

### aws-diagram
**Paquete**: `awslabs.aws-diagram-mcp-server`
**Descripción**: Generación de diagramas de arquitectura
**Casos de uso**:
- Diagramas automáticos
- Documentación visual
- Presentaciones técnicas

### aws-support
**Paquete**: `awslabs.aws-support-mcp-server`
**Descripción**: Gestión de casos de soporte AWS
**Casos de uso**:
- Creación de tickets
- Seguimiento de casos
- Escalación de problemas
