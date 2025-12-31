# Mditor

[English](README.md) | [简体中文](README-CN.md) | [繁體中文](README-TW.md) | [日本語](README-JA.md)

A powerful and elegant VS Code extension that transforms your Markdown editing experience with WYSIWYG capabilities and comprehensive file preview support.

## ✨ Highlights

Mditor brings professional-grade editing and preview capabilities to Visual Studio Code, featuring:

- 🎨 **Beautiful WYSIWYG Markdown Editor** - Real-time preview with rich formatting
- 📊 **Multi-format File Viewer** - Preview Office documents, PDFs, and more
- 🌓 **Multiple Theme Support** - Gorgeous light and dark themes for comfortable editing
- ⚡ **Lightning Fast** - Optimized performance for large documents
- 🎯 **Developer Friendly** - Rich keyboard shortcuts and intuitive interface

## 📸 Screenshots

### Light Theme
![Light Theme](images/light.png)

### Dark Theme
![Dark Theme](images/dark.png)

## 🚀 Features

### Markdown Editor Excellence

Powered by [Vditor](https://github.com/Vanessa219/vditor), our WYSIWYG editor provides:

- **Real-time Preview** - See your formatted content as you type
- **Rich Formatting** - Support for tables, code blocks, diagrams (Mermaid), math formulas (LaTeX)
- **Smart Paste** - Automatic image upload and path resolution
- **Export Anywhere** - Convert to PDF, DOCX, or HTML with one click
- **Theme Variety** - Multiple beautiful editor themes to match your style

#### Powerful Keyboard Shortcuts

Built on [Vditor shortcuts](shortcut.md) with enhanced productivity features:

- **Move list up**: `Ctrl+Alt+I` / `⌘+^+I`
- **Move list down**: `Ctrl+Alt+J` / `⌘+^+J`
- **Edit in VS Code**: `Ctrl+Alt+E` / `⌘+^+E`
- **Enhanced paste**: `Ctrl+V` / `Cmd+V` with automatic image handling

#### Smart Features

- Zoom editor with `Ctrl/Cmd + Mouse Wheel`
- Open hyperlinks with `Ctrl/Meta + Click` or double-click
- Drag & drop image insertion
- Automatic image path resolution
- Syntax highlighting with multiple theme options

### Comprehensive File Preview

Preview common file formats directly in VS Code:

- 📊 **Spreadsheets**: .xls, .xlsx, .csv (with edit & save capability)
- 📝 **Documents**: .docx
- 🖼️ **Graphics**: .svg
- 📄 **PDFs**: .pdf (powered by PDF.js)
- 🔤 **Fonts**: .ttf, .otf, .woff, .woff2
- 📋 **Markdown**: .md, .markdown
- 🌐 **HTTP**: .http, .rest (integrated HTTP client)
- ⚙️ **Registry**: .reg (Windows registry files)
- 📦 **Archives**: .zip, .jar, .vsix, .rar

### Additional Capabilities

- **Material Icons** - Beautiful file icons from Material Icon Theme
- **Live HTML Preview** - Press `Ctrl+Shift+V` for instant HTML preview
- **HTTP Client** - Send API requests directly from .http files
- **Registry Editor** - Syntax highlighting for Windows registry files

## 🔧 Configuration

Fine-tune Mditor through VS Code settings:

| Setting | Description |
|---------|-------------|
| `mditor.enabled` | Enable/disable the extension |
| `mditor.previewCode` | Enable code syntax highlighting in preview |
| `mditor.previewCodeStyle` | Default syntax highlighting style |
| `mditor.previewCodeHighlight.showLineNumber` | Show line numbers in code blocks |
| `mditor.editorLanguage` | Editor UI language |
| `mditor.workspacePathAsImageBasePath` | Use workspace path for image base path |
| `mditor.pasterImgPath` | Image paste path template |
| `mditor.chromiumPath` | Chromium path for PDF export |

### Switching to Native Markdown Editor

To use VS Code's default markdown editor, add to `settings.json`:

```json
{
    "workbench.editorAssociations": {
        "*.md": "default",
        "*.markdown": "default"
    }
}
```

## 📋 Requirements

- Visual Studio Code `^1.64.0`
- Internet connection (for some preview features)

## 📥 Installation

### From Marketplace
1. Open VS Code
2. Go to Extensions (`Ctrl+Shift+X`)
3. Search for "Mditor"
4. Click Install

### From VSIX
1. Download the latest .vsix file
2. Open VS Code
3. Extensions → `...` → Install from VSIX
4. Select the downloaded file

## 🎯 Quick Start

1. **Markdown Editing**: Open any `.md` file - the WYSIWYG editor launches automatically
2. **Office Preview**: Click on `.xlsx`, `.docx`, `.pdf` files to preview
3. **HTML Preview**: Open `.html` files and press `Ctrl+Shift+V`
4. **HTTP Requests**: Create `.http` files to test APIs
5. **Archive Viewing**: Open `.zip` or other archives to browse contents

## 🛠️ Development

```bash
# Install dependencies
npm install

# Build the extension
npm run build

# Development mode with hot reload
npm run dev

# Package for distribution
npm run package
```

## 💖 Support This Project

If you find Mditor helpful, consider supporting its development:

### International Donations
[![PayPal](https://img.shields.io/badge/PayPal-Donate-blue.svg?logo=paypal)](https://www.paypal.me/howpigcanfly)

**PayPal**: howpigcanfly@outlook.com

### China Mainland Donations
<p>
  <img src="images/alipay.jpg" alt="Alipay Donation" width="200" style="display:inline-block;margin-right:16px;" />
  <img src="images/wechatpay.jpg" alt="WeChat Pay Donation" width="200" style="display:inline-block;" />
</p>

**Alipay / WeChat Pay**: Scan the QR codes above

### Bank Transfer (China)
For bank transfer donations, please contact: dreamxwork@outlook.com

---

Your donations help maintain and improve this project. Thank you for your support!

## 🙏 Credits

This project is built on the shoulders of giants:

- **PDF Rendering**: [mozilla/pdf.js](https://github.com/mozilla/pdf.js/)
- **DOCX Rendering**: [VolodymyrBaydalka/docxjs](https://github.com/VolodymyrBaydalka/docxjs)
- **XLSX Processing**:
  - [SheetJS/sheetjs](https://github.com/SheetJS/sheetjs) - Excel parsing
  - [myliang/x-spreadsheet](https://github.com/myliang/x-spreadsheet) - Spreadsheet UI
- **HTTP Client**: [Rest Client](https://github.com/Huachao/vscode-restclient)
- **Markdown Engine**: [Vanessa219/vditor](https://github.com/Vanessa219/vditor)
- **Icon Theme**: [PKief/vscode-material-icon-theme](https://github.com/PKief/vscode-material-icon-theme)

## 📜 License

This project is licensed under the [LGPL-3.0-or-later License](LICENSE).

## 📞 Contact & Support

- **Repository**: [https://github.com/dreamxwork/mditor-vs](https://github.com/dreamxwork/mditor-vs)
- **Issues**: [GitHub Issues](https://github.com/dreamxwork/mditor-vs/issues)
- **Email**: dreamxwork@outlook.com

---

Made with ❤️ by the Mditor Team | *Last updated: 2026*
