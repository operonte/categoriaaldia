# Categoría al Día

Macro de Excel para gestión de inventario Walmart Smart. Automatiza conteos, códigos de barras, análisis de reportes y gestión de más de 13.000 ítems con filtro de usuario automático.

## 📋 Características

- **Gestión de inventario** para Walmart Smart
- **Automatización de conteos** y códigos de barras
- **Análisis de reportes** integrado
- **Base de datos** de más de 13.000 ítems
- **Filtro de usuario automático** para acceso personalizado

## 📁 Contenido del Proyecto

| Archivo | Descripción |
|---------|-------------|
| `Categoria.xlsb` | Workbook de Excel con las macros de gestión de inventario |
| `generador codigos de barrahtml.html` | Generador de códigos de barras en HTML (abre en navegador para imprimir etiquetas) |

## 🚀 Requisitos

- **Microsoft Excel** (con macros habilitadas)
- Windows (recomendado para mejor compatibilidad con VBA)

## 📦 Instalación y Uso

1. **Descarga** el repositorio o clona con:
   ```bash
   git clone https://github.com/operonte/categoriaaldia.git
   ```

2. **Habilita las macros** en Excel:
   - Abre `Categoria.xlsb`
   - Si Excel bloquea las macros, ve a *Archivo → Opciones → Centro de confianza* y permite el contenido de este libro

3. **Generador de códigos de barras**:
   - Abre `generador codigos de barrahtml.html` en tu navegador
   - Ingresa la lista de ítems o UPC (uno por línea)
   - Genera e imprime como PDF para etiquetas

## ⚠️ Nota de Seguridad

- No incluir datos sensibles del negocio en el repositorio
- Los archivos `*.txt` y la carpeta `DATOS para nuevor proyectostxt/` están excluidos por seguridad (ver `.gitignore`)

## 👨‍💻 Desarrollador

**Cristian Bravo Droguett**  
📧 cristian.bravo.droguett@gmail.com

## 📄 Licencia

Este proyecto está bajo la licencia MIT. Ver el archivo [LICENSE](LICENSE) para más detalles.
