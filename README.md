# AWS MCP Role Configurations

> Configuraciones optimizadas de servidores AWS MCP organizadas por roles profesionales para maximizar la productividad en entornos cloud.

[![AWS](https://img.shields.io/badge/AWS-MCP%20Servers-orange?logo=amazon-aws)](https://awslabs.github.io/mcp/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)

## 📋 Tabla de Contenidos

- [Acerca del Proyecto](#-acerca-del-proyecto)
- [Roles Disponibles](#-roles-disponibles)
- [Estructura del Repositorio](#-estructura-del-repositorio)
- [Instalación y Uso](#-instalación-y-uso)
- [Configuraciones por Rol](#-configuraciones-por-rol)
- [Ejemplos de Uso](#-ejemplos-de-uso)
- [Contribuir](#-contribuir)
- [Recursos Adicionales](#-recursos-adicionales)

## 🎯 Acerca del Proyecto

Este repositorio contiene configuraciones JSON predefinidas para servidores AWS MCP (Model Context Protocol), organizadas específicamente para diferentes roles profesionales en entornos cloud. Cada configuración está diseñada para optimizar la productividad según las responsabilidades y casos de uso típicos de cada rol.

### ¿Qué son los AWS MCP Servers?

Los servidores AWS MCP son un conjunto de herramientas especializadas que mejoran las capacidades de los modelos de IA proporcionando:

- ✅ **Acceso a documentación actualizada** de AWS
- ✅ **Automatización de flujos de trabajo** comunes
- ✅ **Conocimiento especializado** del dominio cloud
- ✅ **Mejor calidad de respuestas** para tareas específicas de AWS

## 👥 Roles Disponibles

### 🏗️ Arquitecto de Infraestructura Cloud
**Enfoque:** Diseño de arquitecturas escalables, IaC, y optimización de costos
- Servidores de infraestructura y despliegue
- Herramientas de diagramado y documentación
- Estimación de costos pre-despliegue

### 📊 Analista CloudOps (Cloud Engineer)
**Enfoque:** Operaciones, monitoreo, y mantenimiento de infraestructura
- Herramientas de monitoreo y observabilidad
- Gestión de incidentes y soporte
- Análisis de costos operativos

### 🗄️ Analista DBA
**Enfoque:** Gestión de bases de datos, rendimiento, y análisis de datos
- Servidores de múltiples tipos de BD
- Herramientas de caching y optimización
- Monitoreo específico de bases de datos

## 📁 Estructura del Repositorio

```
aws-mcp-role-configs/
├── README.md
├── configs/
│   ├── arquitecto-infraestructura/
│   │   ├── minimal.json          # Configuración básica
│   │   ├── standard.json         # Configuración estándar
│   │   └── advanced.json         # Configuración completa
│   ├── cloudops-engineer/
│   │   ├── minimal.json
│   │   ├── standard.json
│   │   └── advanced.json
│   └── dba-analyst/
│       ├── minimal.json
│       ├── standard.json
│       └── advanced.json
├── examples/
│   ├── claude-desktop-setup.md   # Configuración para Claude Desktop
│   ├── cursor-setup.md          # Configuración para Cursor
│   └── vscode-setup.md          # Configuración para VS Code
├── docs/
│   ├── server-descriptions.md   # Descripción detallada de cada servidor
│   ├── troubleshooting.md      # Solución de problemas comunes
│   └── migration-guide.md      # Guía de migración entre configuraciones
└── LICENSE
```

## 🚀 Instalación y Uso

### Prerrequisitos

- Cliente MCP compatible (Claude Desktop, Cursor, VS Code con extensión MCP, etc.)
- Credenciales AWS configuradas
- Python 3.8+ (para algunos servidores locales)

### Uso Rápido

1. **Clona el repositorio:**
   ```bash
   git clone https://github.com/tu-usuario/aws-mcp-role-configs.git
   cd aws-mcp-role-configs
   ```

2. **Selecciona tu rol y nivel:**
   ```bash
   # Ejemplo para Arquitecto de Infraestructura - Nivel Estándar
   cp configs/arquitecto-infraestructura/standard.json ~/.config/claude-desktop/
   ```

3. **Configura tu cliente MCP:**
   - Para Claude Desktop: Edita `~/.config/claude-desktop/claude_desktop_config.json`
   - Para otros clientes: Ver `/examples/` para instrucciones específicas

4. **Reinicia tu cliente MCP** y ¡listo!

### Configuración Detallada

Ver la carpeta `/examples/` para instrucciones específicas de cada cliente MCP.

## ⚙️ Configuraciones por Rol

### Niveles de Configuración

| Nivel | Descripción | Servidores | Ideal para |
|-------|-------------|------------|------------|
| **Minimal** | Configuración básica esencial | 2-3 servidores | Principiantes, pruebas rápidas |
| **Standard** | Configuración equilibrada | 4-6 servidores | Uso diario profesional |
| **Advanced** | Configuración completa | 8+ servidores | Proyectos complejos, expertos |

### Resumen por Rol

#### 🏗️ Arquitecto de Infraestructura
- **Minimal:** AWS Knowledge + AWS API + CDK
- **Standard:** + Terraform + Pricing + Diagram
- **Advanced:** + CloudFormation + Support + Cost Explorer

#### 📊 CloudOps Engineer
- **Minimal:** AWS Knowledge + AWS API + CloudWatch
- **Standard:** + Cost Explorer + Support + Application Signals
- **Advanced:** + EKS/ECS + Step Functions + Monitoring tools

#### 🗄️ DBA Analyst
- **Minimal:** AWS Knowledge + AWS API + DynamoDB
- **Standard:** + Aurora (PostgreSQL/MySQL) + ElastiCache
- **Advanced:** + DocumentDB + Redshift + Neptune + múltiples BD

## 💡 Ejemplos de Uso

### Caso 1: Arquitecto creando nueva infraestructura
```bash
# Usar configuración standard para arquitecto
cp configs/arquitecto-infraestructura/standard.json mi-config.json
```
**Resultado:** Acceso a CDK, estimación de costos, y generación de diagramas automática.

### Caso 2: CloudOps monitoreando producción
```bash
# Usar configuración advanced para CloudOps
cp configs/cloudops-engineer/advanced.json mi-config.json
```
**Resultado:** Monitoreo completo, análisis de costos, y gestión de incidentes.

### Caso 3: DBA optimizando múltiples bases de datos
```bash
# Usar configuración advanced para DBA
cp configs/dba-analyst/advanced.json mi-config.json
```
**Resultado:** Acceso a múltiples tipos de BD, caching, y análisis de rendimiento.

## 🤝 Contribuir

¡Las contribuciones son bienvenidas! Por favor:

1. Fork el repositorio
2. Crea una rama para tu feature (`git checkout -b feature/nueva-configuracion`)
3. Commit tus cambios (`git commit -am 'Añadir nueva configuración'`)
4. Push a la rama (`git push origin feature/nueva-configuracion`)
5. Abre un Pull Request

### Pautas de Contribución

- Mantén las configuraciones organizadas por rol
- Incluye documentación para nuevos servidores
- Prueba las configuraciones antes de enviar PR
- Sigue las convenciones de naming existentes

## 📚 Recursos Adicionales

### Documentación Oficial
- [AWS MCP Servers](https://awslabs.github.io/mcp/) - Documentación oficial
- [Model Context Protocol](https://modelcontextprotocol.io/introduction) - Especificación MCP
- [Claude Desktop MCP](https://claude.ai/docs/mcp) - Configuración Claude Desktop

### Herramientas Relacionadas
- [AWS CLI](https://aws.amazon.com/cli/) - Interfaz de línea de comandos de AWS
- [AWS CDK](https://aws.amazon.com/cdk/) - Kit de desarrollo cloud
- [Terraform](https://www.terraform.io/) - Infrastructure as Code
