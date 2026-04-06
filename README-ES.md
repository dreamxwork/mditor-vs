# Mditor

[English](README.md) | [简体中文](README-CN.md) | [繁體中文](README-TW.md) | [日本語](README-JA.md) | [한국어](README-KO.md) | [Français](README-FR.md) | [Deutsch](README-DE.md) | [Español](README-ES.md) | [Русский](README-RU.md)

Una extensión de VS Code potente y elegante que transforma tu experiencia de edición Markdown con capacidades WYSIWYG y soporte completo de vista previa de archivos.

## ✨ Características destacadas

Mditor aporta capacidades de edición y vista previa de nivel profesional a Visual Studio Code:

- 🎨 **Hermoso editor Markdown WYSIWYG** - Vista previa en tiempo real con formato enriquecido
- 📊 **Visor de archivos multiformato** - Vista previa de documentos Office, PDF y más
- 🌓 **Soporte de múltiples temas** - Hermosos temas claros y oscuros para una edición cómoda
- ⚡ **Ultrarrápido** - Rendimiento optimizado para documentos grandes
- 🎯 **Amigable para desarrolladores** - Atajos de teclado ricos e interfaz intuitiva

## 📸 Capturas de pantalla

### Tema claro
![Tema claro](images/light.png)

### Tema oscuro
![Tema oscuro](images/dark.png)

## 🚀 Características

### Excelencia del editor Markdown

Impulsado por [Vditor](https://github.com/Vanessa219/vditor), nuestro editor WYSIWYG proporciona:

- **Vista previa en tiempo real** - Ve tu contenido formateado mientras escribes
- **Formato enriquecido** - Soporte para tablas, bloques de código, diagramas (Mermaid), fórmulas matemáticas (LaTeX)
- **Pegado inteligente** - Carga automática de imágenes y resolución de rutas
- **Exportar en cualquier lugar** - Convierte a PDF, DOCX o HTML con un clic
- **Variedad de temas** - Múltiples temas de editor hermosos para combinar con tu estilo

#### Atajos de teclado potentes

Basado en [atajos de Vditor](shortcut.md) con características de productividad mejoradas:

- **Mover lista arriba**: `Ctrl+Alt+I` / `⌘+^+I`
- **Mover lista abajo**: `Ctrl+Alt+J` / `⌘+^+J`
- **Editar en VS Code**: `Ctrl+Alt+E` / `⌘+^+E`
- **Pegado mejorado**: `Ctrl+V` / `Cmd+V` con manejo automático de imágenes

#### Características inteligentes

- Hacer zoom en el editor con `Ctrl/Cmd + Rueda del ratón`
- Abrir hipervínculos con `Ctrl/Meta + Clic` o doble clic
- Inserción de imágenes arrastrando y soltando
- Resolución automática de rutas de imagen
- Resaltado de sintaxis con múltiples opciones de tema

### Vista previa completa de archivos

Vista previa de formatos de archivo comunes directamente en VS Code:

- 📊 **Hojas de cálculo**: .xls, .xlsx, .csv (con capacidad de edición y guardado)
- 📝 **Documentos**: .docx
- 🖼️ **Gráficos**: .svg
- 📄 **PDF**: .pdf (impulsado por PDF.js)
- 🔤 **Fuentes**: .ttf, .otf, .woff, .woff2
- 📋 **Markdown**: .md, .markdown
- 🌐 **HTTP**: .http, .rest (cliente HTTP integrado)
- ⚙️ **Registro**: .reg (archivos de registro de Windows)
- 📦 **Archivos**: .zip, .jar, .vsix, .rar

### Capacidades adicionales

- **Iconos Material** - Hermosos iconos de archivo del Material Icon Theme
- **Vista previa HTML en vivo** - Presiona `Ctrl+Shift+V` para vista previa HTML instantánea
- **Cliente HTTP** - Envía solicitudes API directamente desde archivos .http
- **Editor de registro** - Resaltado de sintaxis para archivos de registro de Windows

## 🔧 Configuración

Ajusta finamente Mditor a través de la configuración de VS Code:

| Configuración | Descripción |
|---------------|-------------|
| `mditor.enabled` | Habilitar/deshabilitar la extensión |
| `mditor.previewCode` | Habilitar resaltado de sintaxis de código en vista previa |
| `mditor.previewCodeStyle` | Estilo de resaltado de sintaxis predeterminado |
| `mditor.previewCodeHighlight.showLineNumber` | Mostrar números de línea en bloques de código |
| `mditor.editorLanguage` | Idioma de la interfaz del editor |
| `mditor.workspacePathAsImageBasePath` | Usar ruta del espacio de trabajo como ruta base de imagen |
| `mditor.pasterImgPath` | Plantilla de ruta de pegado de imagen |
| `mditor.chromiumPath` | Ruta de Chromium para exportación PDF |

### Cambiar al editor Markdown nativo

Para usar el editor markdown predeterminado de VS Code, agrega a `settings.json`:

```json
{
    "workbench.editorAssociations": {
        "*.md": "default",
        "*.markdown": "default"
    }
}
```

## 📋 Requisitos

- Visual Studio Code `^1.64.0`
- Conexión a Internet (para algunas características de vista previa)

## 📥 Instalación

### Desde el Marketplace
1. Abrir VS Code
2. Ir a Extensiones (`Ctrl+Shift+X`)
3. Buscar "Mditor"
4. Hacer clic en Instalar

### Desde VSIX
1. Descargar el último archivo .vsix
2. Abrir VS Code
3. Extensiones → `...` → Instalar desde VSIX
4. Seleccionar el archivo descargado

## 🎯 Inicio rápido

1. **Edición Markdown**: Abrir cualquier archivo `.md` - el editor WYSIWYG se inicia automáticamente
2. **Vista previa Office**: Hacer clic en archivos `.xlsx`, `.docx`, `.pdf` para vista previa
3. **Vista previa HTML**: Abrir archivos `.html` y presionar `Ctrl+Shift+V`
4. **Solicitudes HTTP**: Crear archivos `.http` para probar APIs
5. **Visualización de archivos**: Abrir `.zip` u otros archivos para explorar contenido

## 📖 Ejemplos de Markdown

¿Quieres ver qué puede hacer Mditor? Consulta nuestro archivo de ejemplos de Markdown completo que muestra todas las características compatibles:

**[Descargar markdown-examples.md](https://raw.githubusercontent.com/dreamxwork/mditor-vs/main/markdown-examples.md)**

Este archivo de ejemplos incluye:
- Formato de texto básico (encabezados, negrita, cursiva, listas)
- Bloques de código con resaltado de sintaxis (C++, Java, Python, Shell, CMake, archivos de registro)
- Diagramas Mermaid (diagramas de flujo, diagramas de secuencia, diagramas de clases, diagramas de Gantt, gráficos de ramas Git)
- Fórmulas matemáticas (LaTeX)
- Tablas y visualización de datos
- Notación musical (notación ABC)
- Diagramas Graphviz
- Visualización de datos ECharts
- ¡Y mucho más!

## 🛠️ Desarrollo

```bash
# Instalar dependencias
npm install

# Construir la extensión
npm run build

# Modo de desarrollo con recarga en caliente
npm run dev

# Empaquetar para distribución
npm run package
```

## 💖 Apoyar este proyecto

Si encuentras útil Mditor, considera apoyar su desarrollo:

### Donaciones internacionales
[![PayPal](https://img.shields.io/badge/PayPal-Donate-blue.svg?logo=paypal)](https://www.paypal.me/howpigcanfly)

**Cuenta PayPal**: howpigcanfly@outlook.com

### Donaciones en criptomonedas
**Bitcoin (BTC)**: `13KGRMK3AGMNxQqdC5yyNRi7cpmD3mQhAM`

### Donaciones en China continental
<p>
  <img src="images/alipay.jpg" alt="Donación Alipay" width="200" style="display:inline-block;margin-right:16px;" />
  <img src="images/wechatpay.jpg" alt="Donación WeChat Pay" width="200" style="display:inline-block;" />
</p>

**Alipay / WeChat Pay**: Escanea los códigos QR anteriores

### Transferencia bancaria
Para donaciones por transferencia bancaria, contacta: dreamxwork@outlook.com

---

Tus donaciones ayudan a mantener y mejorar este proyecto. ¡Gracias por tu apoyo!

## 🙏 Créditos

Este proyecto está construido sobre los hombros de gigantes:

- **Renderizado PDF**: [mozilla/pdf.js](https://github.com/mozilla/pdf.js/)
- **Renderizado DOCX**: [VolodymyrBaydalka/docxjs](https://github.com/VolodymyrBaydalka/docxjs)
- **Procesamiento XLSX**:
  - [SheetJS/sheetjs](https://github.com/SheetJS/sheetjs) - Análisis de Excel
  - [myliang/x-spreadsheet](https://github.com/myliang/x-spreadsheet) - Interfaz de hoja de cálculo
- **Cliente HTTP**: [Rest Client](https://github.com/Huachao/vscode-restclient)
- **Motor Markdown**: [Vanessa219/vditor](https://github.com/Vanessa219/vditor)
- **Tema de iconos**: [PKief/vscode-material-icon-theme](https://github.com/PKief/vscode-material-icon-theme)

## 📜 Licencia

Este proyecto está licenciado bajo la [Licencia LGPL-3.0-or-later](LICENSE).

## 📞 Contacto y soporte

- **Repositorio**: [https://github.com/dreamxwork/mditor-vs](https://github.com/dreamxwork/mditor-vs)
- **Problemas**: [GitHub Issues](https://github.com/dreamxwork/mditor-vs/issues)
- **Correo electrónico**: dreamxwork@outlook.com

---

Hecho con ❤️ por el equipo Mditor | *Última actualización: 2026*
