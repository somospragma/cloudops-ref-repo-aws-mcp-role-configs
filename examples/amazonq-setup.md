# Configuración MCP para Amazon Q Developer

## 📋 Prerrequisitos
- Amazon Q Developer (VS Code, JetBrains, o CLI)
- Python 3.8+ y `uv` package manager
- AWS CLI configurado

## 🔧 Configuración

### 1. Ubicación del archivo
Amazon Q Developer busca la configuración en:
- **Global**: `~/.aws/amazonq/mcp.json`
- **Local**: `.amazonq/mcp.json` (en el directorio del proyecto)

### 2. Instalación Global (Recomendada)

```bash
# 1. Crear directorio
mkdir -p ~/.aws/amazonq/

# 2. Copiar configuración del rol deseado
cp configs/[rol]/mcp.json ~/.aws/amazonq/mcp.json

# 3. Reiniciar Amazon Q Developer
```

### 3. Instalación Local (Por Proyecto)

```bash
# En el directorio del proyecto
mkdir -p .amazonq/
cp configs/[rol]/mcp.json .amazonq/mcp.json
```

## 🎯 Ejemplos por Rol

### Arquitecto de Infraestructura
```bash
# Configuración completa para arquitectos
cp configs/arquitecto-infraestructura/mcp.json ~/.aws/amazonq/mcp.json
```

### CloudOps Engineer
```bash
# Configuración completa para CloudOps
cp configs/cloudops-engineer/mcp.json ~/.aws/amazonq/mcp.json
```

### DBA Analyst
```bash
# Configuración completa para DBAs
cp configs/dba-analyst/mcp.json ~/.aws/amazonq/mcp.json
```

## ✅ Verificación
1. Reiniciar Amazon Q Developer
2. Abrir Amazon Q Chat
3. Hacer clic en el ícono de herramientas
4. Verificar que los servidores MCP estén conectados

## 🔧 Configuración Manual (UI)
También puedes configurar desde la interfaz de Amazon Q:
1. Abrir Amazon Q Chat
2. Clic en ícono de herramientas
3. Agregar servidor MCP manualmente
4. Configurar según los archivos JSON
