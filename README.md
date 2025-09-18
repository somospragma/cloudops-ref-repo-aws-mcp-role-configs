# AWS MCP Role Configurations para Amazon Q Developer

Configuraciones optimizadas de servidores MCP para diferentes roles en AWS CloudOps, específicamente diseñadas para Amazon Q Developer.

## 🎯 Roles Disponibles

### 🏗️ Arquitecto CloudOps
Servidores incluidos: AWS API, Knowledge, CDK, Terraform, CloudFormation, Pricing, Diagram, Support

### ⚙️ Analista CloudOps
Servidores incluidos: AWS API, Knowledge, CloudWatch, Cost Explorer, Support, AppSignals, EKS, ECS

### 🗄️ Analista DBA
Servidores incluidos: AWS API, Knowledge, DynamoDB, Aurora (PostgreSQL/MySQL/DSQL), DocumentDB, ElastiCache, Redshift, Cost Explorer

## 🚀 Instalación Rápida

```bash
# Copiar configuración del rol deseado
cp configs/[rol]/mcp.json ~/.aws/amazonq/mcp.json

# Reiniciar Amazon Q Developer
```

## 📁 Estructura

- `configs/` - Configuraciones por rol (un archivo mcp.json por rol)
- `examples/` - Guía de configuración para Amazon Q Developer
- `docs/` - Documentación detallada

## 📖 Documentación

- [Configuración Amazon Q Developer](examples/amazonq-setup.md)
- [Descripción de Servidores](docs/server-descriptions.md)
- [Solución de Problemas](docs/troubleshooting.md)
- [Guía de Migración](docs/migration-guide.md)
