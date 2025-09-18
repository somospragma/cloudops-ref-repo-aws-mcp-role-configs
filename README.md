# AWS MCP Role Configurations para Amazon Q

<div align="center">

![AWS](https://img.shields.io/badge/AWS-FF9900?style=for-the-badge&logo=amazon-aws&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-0066CC?style=for-the-badge&logo=protocol&logoColor=white)
![Amazon Q](https://img.shields.io/badge/Amazon%20Q-232F3E?style=for-the-badge&logo=amazon&logoColor=white)

**Configuraciones optimizadas de servidores MCP para diferentes roles en AWS CloudOps**

*Específicamente diseñadas para Amazon Q CLI*

</div>

---

## 📋 Tabla de Contenidos

- [🎯 Roles Disponibles](#-roles-disponibles)
- [🚀 Instalación Rápida](#-instalación-rápida)
- [📁 Estructura del Proyecto](#-estructura-del-proyecto)
- [⚙️ Configuraciones Detalladas](#️-configuraciones-detalladas)
- [📖 Documentación](#-documentación)
- [🔧 Prerrequisitos](#-prerrequisitos)

---

## 🎯 Roles Disponibles

### 🏗️ Arquitecto CloudOps
**Enfoque:** Diseño y despliegue de infraestructura  
**Servidores:** 8 MCP servers  
**Incluye:** AWS API, Knowledge, CDK, Terraform, CloudFormation, Pricing, Diagram, Support

**Casos de uso:**
- ✅ Diseñar arquitecturas escalables
- ✅ Crear plantillas de IaC (CDK, CloudFormation, Terraform)
- ✅ Estimar costos pre-despliegue
- ✅ Generar diagramas automáticos

### ⚙️ Analista CloudOps
**Enfoque:** Monitoreo y operación de infraestructura  
**Servidores:** 8 MCP servers  
**Incluye:** AWS API, Knowledge, CloudWatch, Cost Explorer, Support, AppSignals, EKS, ECS

**Casos de uso:**
- ✅ Monitorear infraestructura en producción
- ✅ Analizar logs y métricas
- ✅ Gestionar contenedores (EKS/ECS)
- ✅ Optimizar costos operativos

### 🗄️ Analista DBA
**Enfoque:** Administración de bases de datos  
**Servidores:** 10 MCP servers  
**Incluye:** AWS API, Knowledge, DynamoDB, Aurora (PostgreSQL/MySQL/DSQL), DocumentDB, ElastiCache, Redshift, Cost Explorer

**Casos de uso:**
- ✅ Administrar múltiples tipos de BD
- ✅ Optimizar consultas y rendimiento
- ✅ Gestionar backups y recuperación
- ✅ Monitorear costos de BD

---

## 🚀 Instalación Rápida

### Opción 1: Instalación directa
```bash
# Clonar repositorio
git clone https://github.com/tu-organizacion/aws-mcp-role-configs.git
cd aws-mcp-role-configs

# Instalar configuración para tu rol
cp configs/[rol]/mcp.json ~/.aws/amazonq/mcp.json

# Reiniciar Amazon Q
```

### Opción 2: Descarga específica
```bash
# Arquitecto CloudOps
cp configs/arquitecto-cloudops/mcp.json ~/.aws/amazonq/mcp.json

# Analista CloudOps
cp configs/analista-cloudops/mcp.json ~/.aws/amazonq/mcp.json

# Analista DBA
cp configs/analista-dba/mcp.json ~/.aws/amazonq/mcp.json
```

---

## 📁 Estructura del Proyecto

```
aws-mcp-role-configs/
├── README.md                    # 📖 Documentación principal
├── LICENSE                      # ⚖️ Licencia MIT
├── configs/                     # ⚙️ Configuraciones por rol
│   ├── arquitecto-cloudops/
│   │   └── mcp.json            # 🏗️ Configuración para arquitectos
│   ├── analista-cloudops/
│   │   └── mcp.json            # ⚙️ Configuración para CloudOps
│   └── analista-dba/
│       └── mcp.json            # 🗄️ Configuración para DBAs
├── examples/
│   └── amazonq-setup.md        # 📋 Guía de configuración
└── docs/                        # 📚 Documentación detallada
    ├── server-descriptions.md   # 🔍 Descripción de servidores
    └── troubleshooting.md       # 🛠️ Solución de problemas
```

---

## ⚙️ Configuraciones Detalladas

### 🏗️ Arquitecto CloudOps
| Servidor | Descripción | Casos de Uso |
|----------|-------------|--------------|
| AWS API | Gestión de recursos AWS | Crear, actualizar, eliminar recursos |
| AWS Knowledge | Documentación actualizada | Consultar mejores prácticas |
| AWS CDK | Desarrollo con CDK | Generar código de infraestructura |
| AWS Terraform | Flujos Terraform | Gestionar estado de infraestructura |
| AWS CloudFormation | Plantillas CF | Desplegar stacks |
| AWS Pricing | Estimación de costos | Calcular costos pre-despliegue |
| AWS Diagram | Diagramas automáticos | Visualizar arquitecturas |
| AWS Support | Casos de soporte | Gestionar incidentes |

### ⚙️ Analista CloudOps
| Servidor | Descripción | Casos de Uso |
|----------|-------------|--------------|
| AWS API | Gestión operativa | Monitorear recursos |
| AWS Knowledge | Documentación | Troubleshooting |
| CloudWatch | Métricas y logs | Análisis operacional |
| Cost Explorer | Análisis de costos | Optimización continua |
| AWS Support | Gestión de casos | Resolución de incidentes |
| CloudWatch AppSignals | Monitoreo de apps | Performance insights |
| Amazon EKS | Gestión Kubernetes | Orquestación de contenedores |
| Amazon ECS | Gestión Docker | Servicios containerizados |

### 🗄️ Analista DBA
| Servidor | Descripción | Casos de Uso |
|----------|-------------|--------------|
| AWS API | Gestión de BD | Administrar servicios de datos |
| AWS Knowledge | Documentación BD | Consultas específicas |
| DynamoDB | NoSQL operations | Gestión de tablas |
| Aurora PostgreSQL | PostgreSQL ops | Consultas relacionales |
| Aurora MySQL | MySQL ops | Administración MySQL |
| Aurora DSQL | SQL distribuido | Consultas escalables |
| DocumentDB | MongoDB-compatible | Operaciones de documentos |
| ElastiCache | Operaciones caché | Optimización rendimiento |
| Redshift | Data warehouse | Análisis de datos |
| Cost Explorer | Costos de BD | Optimización específica |

---

## 📖 Documentación

| Documento | Descripción |
|-----------|-------------|
| [📋 Configuración Amazon Q](examples/amazonq-setup.md) | Guía paso a paso para configurar Amazon Q |
| [🔍 Descripción de Servidores](docs/server-descriptions.md) | Detalles de cada servidor MCP |
| [🛠️ Solución de Problemas](docs/troubleshooting.md) | Troubleshooting y diagnóstico |

---

## 🔧 Prerrequisitos

### Software Requerido
- ✅ **Amazon Q Developer** (VS Code, JetBrains, o CLI)
- ✅ **Python 3.8+** y `uv` package manager
- ✅ **AWS CLI** configurado con credenciales

### Instalación de Prerrequisitos
```bash
# Instalar uv package manager
pip install uv

# Verificar instalación
uv --version

# Configurar AWS CLI (si no está configurado)
aws configure
```

### Verificación
```bash
# Verificar Python
python3 --version

# Verificar AWS CLI
aws sts get-caller-identity

# Verificar uv
uv --version
```

</div>
