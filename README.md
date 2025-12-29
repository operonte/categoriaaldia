# 🛒 Categoria al Día - Sistema de Gestión de Inventario Walmart Smart

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Platform](https://img.shields.io/badge/Platform-Walmart%20Smart-blue)](https://github.com)
[![Excel](https://img.shields.io/badge/Excel-Macro-orange)](https://github.com)
[![Status](https://img.shields.io/badge/Status-Active-success)](https://github.com)

> **Solución integral de automatización para la gestión de inventario en la plataforma Walmart Smart**, diseñada para optimizar el proceso de "Categoría al Día" mediante macros avanzadas que interactúan directamente con la interfaz del sistema.

---

## 📋 Descripción

**Categoria al Día** es una macro desarrollada específicamente para la plataforma Walmart Smart que automatiza y optimiza los procesos de gestión de inventario. Este sistema permite realizar operaciones complejas sobre más de **13,000 items**, facilitando tareas críticas como conteos físicos, gestión de códigos de barras, análisis de reportes y administración de existencias.

La macro está diseñada para trabajar exclusivamente dentro del ecosistema Walmart Smart y requiere acceso autorizado a la plataforma para su funcionamiento.

---

## ✨ Características Principales

### 🔧 Gestión de Inventario
- ✅ **Creación y gestión de códigos de barras** con estándar internacional (Code128, EAN8, EAN13)
- ✅ **Agregar o eliminar items en conteo** de forma masiva
- ✅ **Ampliación de información** para más de 13,000 items
- ✅ **Impresión directa** de códigos de barras o listas de conteo a impresora
- ✅ **Análisis avanzado de reportes** del sistema

### 📊 Administración de Existencias
- ✅ **Carga, eliminación y modificación** de existencias de items directamente en la maestra SMART
- ✅ **Creación de trabajos en el BIN** (sistema de almacenamiento)
- ✅ **Detección y reporte de items falsos** o con discrepancias
- ✅ **Rastreo de diferencias de inventario** en tiempo real
- ✅ **Seguimiento histórico** de items sin existencia por años

### 🔍 Análisis y Control
- ✅ **Creación de listas de conteo** personalizadas e importantes
- ✅ **Detección de fugas de inventario** mediante análisis de patrones
- ✅ **Integración con reportes del sistema** (mermas, rebajas, recibos, etc.)
- ✅ **Auditoría completa** de movimientos de inventario

### 🔐 Seguridad y Control de Acceso
- ✅ **Filtro de usuario automático**: La macro detecta automáticamente el usuario activo
- ✅ **Activación/desactivación automática**: Se habilita o deshabilita según el usuario (sin necesidad de contraseña)
- ✅ **Sistema recursivo**: Validación continua del usuario durante la ejecución
- ✅ **Control granular**: Permite gestionar qué usuarios tienen acceso a qué funcionalidades

---

## 🚀 Funcionalidades Detalladas

### 1. Generación de Códigos de Barras
Sistema HTML independiente que genera códigos de barras estándar internacional a partir de listas de UPC o códigos ITEM. Incluye:
- Soporte para múltiples estándares (Code128, EAN8, EAN13)
- Impresión directa a PDF
- Generación masiva desde listas

### 2. Gestión de Conteos
- Agregar items masivamente a conteos activos
- Eliminar items de conteos existentes
- Ampliar información detallada de items (precios, ubicaciones, descripciones)
- Validación automática de datos antes de aplicar cambios

### 3. Administración de Existencias
- Modificación directa en la maestra SMART del sistema
- Sincronización automática de cambios
- Historial de modificaciones
- Validación de integridad de datos

### 4. Análisis de Reportes
- Procesamiento de reportes de inventario (SPI2800R)
- Análisis de rebajas y markdowns por departamento
- Detección de mermas y discrepancias
- Generación de reportes consolidados

### 5. Trabajo con BIN
- Creación automática de trabajos en el sistema BIN
- Revisión de visibilidad de ubicaciones
- Rastreo de movimientos entre ubicaciones

### 6. Sistema de Filtro de Usuario
Sistema inteligente de control de acceso que garantiza seguridad sin complejidad:
- **Detección automática del usuario**: Identifica al usuario activo en el sistema Smart
- **Sin contraseñas**: El filtro funciona de forma transparente sin requerir credenciales adicionales
- **Activación/desactivación inteligente**: Se activa o desactiva automáticamente según las credenciales del usuario
- **Recursividad**: Verifica continuamente la identidad del usuario durante toda la ejecución
- **Control de acceso granular**: Permite configurar permisos específicos por usuario y funcionalidad
- **Seguridad proactiva**: Previene el uso no autorizado sin interrumpir el flujo de trabajo

---

## 📁 Estructura del Proyecto

```
Categoria_al_dia/
│
├── Categoria.xlsb                          # Macro principal (Excel con VBA)
├── generador codigos de barrahtml.html     # Generador independiente de códigos de barras
│
└── DATOS para nuevor proyectostxt/         # Carpeta de desarrollo y testing
    ├── reporte*.txt                        # Reportes de inventario procesados
    ├── lab*.txt                            # Archivos de pruebas y desarrollo
    ├── Items Top 50*.txt                   # Análisis de rebajas
    ├── reporte_merma*.txt                  # Reportes de mermas
    └── ...                                 # Otros archivos de soporte
```

---

## 🔑 Requisitos

### Sistema y Plataforma
- ⚠️ **Acceso autorizado a la plataforma Walmart Smart** (requisito obligatorio)
- Microsoft Excel con macros habilitadas (para Categoria.xlsb)
- Sistema operativo compatible con Excel y la plataforma Smart
- Permisos de administración en el sistema Walmart Smart
- **Usuario autorizado**: El sistema de filtro automático validará el acceso según el usuario activo

### Permisos Necesarios
- Acceso a la maestra de items
- Permisos de lectura/escritura en el sistema de inventario
- Acceso al módulo de conteos físicos
- Permisos para creación de trabajos BIN
- **Usuario configurado en el sistema de filtro**: El usuario debe estar autorizado en el sistema de filtro (configuración interna)

### Nota sobre el Filtro de Usuario
El sistema de filtro de usuario es completamente automático:
- 🔄 **No requiere intervención manual**: Se activa/desactiva automáticamente
- 🔄 **Sin contraseñas adicionales**: Utiliza las credenciales del sistema Smart
- 🔄 **Verificación continua**: Monitorea el usuario durante toda la sesión

---

## 📖 Uso Básico

### Generador de Códigos de Barras (HTML)
1. Abre `generador codigos de barrahtml.html` en tu navegador
2. Ingresa el departamento y título descriptivo cuando se solicite
3. Pega la lista de códigos ITEM o UPC (uno por línea)
4. Haz clic en "Generar código de barras"
5. Usa "Imprimir como PDF" para guardar o imprimir

### Macro Principal (Categoria.xlsb)
> ⚠️ **Importante**: La macro solo funciona dentro del entorno Walmart Smart con acceso autorizado.

1. Asegúrate de estar conectado a la plataforma Smart con tu usuario autorizado
2. Abre `Categoria.xlsb` en Excel
3. Habilita las macros si Excel lo solicita
4. **El sistema de filtro detectará automáticamente tu usuario** y habilitará/deshabilitará funcionalidades según corresponda
5. Ejecuta las funciones deseadas desde el menú de la macro
6. Sigue las instrucciones en pantalla para cada operación
7. El sistema validará continuamente tu identidad durante la ejecución (recursividad)

---

## 🛠️ Tecnologías Utilizadas

- **Excel VBA**: Para la macro principal y automatización
- **HTML/CSS/JavaScript**: Para el generador de códigos de barras
- **API de TEC-IT**: Para generación de códigos de barras estándar
- **Walmart Smart Platform**: Integración con el sistema de gestión

---

## ⚠️ Limitaciones y Consideraciones

- 🔒 **Requiere acceso autorizado**: La macro principal NO funciona fuera del entorno Walmart Smart
- 🔒 **Dependencia de plataforma**: Diseñada específicamente para la interfaz Smart de Walmart
- 🔒 **Uso interno**: Destinada exclusivamente para uso interno de la organización
- 🔒 **Versiones**: Compatibilidad depende de la versión activa de la plataforma Smart
- 🔒 **Filtro de usuario**: Solo los usuarios autorizados en el sistema de filtro podrán utilizar las funcionalidades completas
- 🔒 **Validación continua**: El sistema verifica el usuario durante toda la ejecución, por lo que cambios de sesión pueden afectar la funcionalidad

---

## 🎯 Casos de Uso

- ✅ **Auditorías de inventario**: Conteos físicos masivos optimizados
- ✅ **Gestión diaria de categorías**: Actualización rápida de información
- ✅ **Control de mermas**: Detección y reporte de discrepancias
- ✅ **Análisis de rebajas**: Procesamiento y análisis de markdowns
- ✅ **Rastreo histórico**: Seguimiento de items con problemas de inventario
- ✅ **Prevención de fugas**: Detección temprana de irregularidades

---

## 📝 Notas de Desarrollo

La carpeta `DATOS para nuevor proyectostxt/` contiene archivos de desarrollo, pruebas y referencias históricas. Estos archivos son utilizados para:
- Testing de nuevas funcionalidades
- Validación de reportes procesados
- Referencia histórica de operaciones
- Desarrollo iterativo de mejoras

---

## 🤝 Contribuciones

Este es un proyecto personal desarrollado para optimizar procesos internos. Las contribuciones están limitadas al contexto organizacional.

---

## 📄 Licencia

Este proyecto es de uso interno y está destinado exclusivamente para operaciones dentro del ecosistema Walmart Smart.

---

## 🔒 Política de Privacidad

Para información detallada sobre cómo manejamos la privacidad y seguridad de los datos, consulta nuestra [Política de Privacidad](PRIVACY_POLICY.md).

**Puntos clave:**
- No almacenamos contraseñas ni información sensible permanentemente
- Todo el procesamiento es local en la máquina del usuario
- Respetamos las políticas de privacidad de Walmart
- El sistema de filtro de usuario protege el acceso a funcionalidades

---

## 👤 Autor

Desarrollado para optimizar la gestión de inventario "Categoría al Día" en Walmart.

---

## 🙏 Agradecimientos

- Equipo de operaciones de inventario de Walmart
- Plataforma Smart por proporcionar las APIs y funcionalidades necesarias

---

## 📞 Soporte

Para soporte o consultas sobre el uso de esta herramienta, contacta al equipo de gestión de inventario autorizado.

---

<div align="center">

**⭐ Si este proyecto te resulta útil, considera darle una estrella en GitHub ⭐**

---

*Desarrollado con ❤️ para optimizar la gestión de inventario*

</div>

