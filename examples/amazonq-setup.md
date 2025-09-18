# Configuración MCP para Amazon Q CLI

## 📋 Prerrequisitos
- Amazon Q CLI (VS Code, JetBrains, o CLI)
- Python 3.8+ y `uv` package manager
- AWS CLI configurado

## 🔧 Configuración

### 1. Ubicación del archivo
Amazon Q busca la configuración en:
- **Global**: `~/.aws/amazonq/mcp.json`
- **Local**: `.amazonq/mcp.json` (en el directorio del proyecto)

### 2. Instalación Global (Recomendada)

```bash
# 1. Crear directorio
mkdir -p ~/.aws/amazonq/

# 2. Copiar configuración del rol deseado
cp configs/[rol]/mcp.json ~/.aws/amazonq/mcp.json

# 3. Reiniciar Amazon Q
```

### 3. Instalación Local (Por Proyecto)

```bash
# En el directorio del proyecto
mkdir -p .amazonq/
cp configs/[rol]/mcp.json .amazonq/mcp.json
```

## 🎯 Ejemplos por Rol

### Arquitecto CloudOps
```bash
# Configuración completa para arquitectos
cp configs/arquitecto-infraestructura/mcp.json ~/.aws/amazonq/mcp.json
```

### Analista CloudOps
```bash
# Configuración completa para CloudOps
cp configs/cloudops-engineer/mcp.json ~/.aws/amazonq/mcp.json
```

### Analista DBA
```bash
# Configuración completa para DBAs
cp configs/dba-analyst/mcp.json ~/.aws/amazonq/mcp.json
```

## ✅ Verificación
1. Reiniciar Amazon Q CLI
2. Abrir Amazon Q Chat
3. Ingresar `/tools`
4. Verificar que los servidores MCP estén conectados y disponibles

## 🔧 Configuración Manual (UI)
También puedes configurar desde la interfaz de Amazon Q:
1. Abrir Amazon Q Chat
2. Clic en ícono de herramientas
3. Agregar servidor MCP manualmente
4. Configurar según los archivos JSON
