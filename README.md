# Mditor

## Introduction

English | [简体中文](README-CN.md) | [繁體中文](README-TW.md)

Mditor is a powerful Visual Studio Code extension that provides comprehensive file preview capabilities and WYSIWYG markdown editing. This extension supports previewing various common office file formats in VS Code.

## Supported File Formats

This extension supports previewing these common rich file formats in VS Code:

- **Excel**: .xls, .xlsx, .csv
- **Word**: .docx
- **SVG**: .svg
- **PDF**: .pdf
- **Fonts**: .ttf, .otf, .woff, .woff2
- **Markdown**: .md, .markdown
- **HTTP Requests**: .http, .rest
- **Windows Registry**: .reg
- **Compressed Files**: .zip, .jar, .vsix, .rar

## Features

### Markdown Editor

This extension integrates [Vditor](https://github.com/Vanessa219/vditor) to provide WYSIWYG markdown editing. **Please note that this editor is no longer actively maintained.**

If you want to use the original VS Code markdown editor, add this to your `settings.json`:

```json
{
    "workbench.editorAssociations": {
        "*.md": "default",
        "*.markdown": "default"
    }
}
```

#### Export Options

Right-click in the markdown editor to export files to PDF, DOCX, or HTML formats. PDF export depends on Chromium, which can be configured via `mditor.chromiumPath`.

![Export Options](image/README-CN/1685418034035.png)

#### Keyboard Shortcuts

Based on [Vditor shortcuts](shortcut.md) with additional features:

- **Move list up**: `Ctrl Alt I` / `⌘ ^ I`
- **Move list down**: `Ctrl Alt J` / `⌘ ^ J`
- **Edit in VS Code**: `Ctrl Alt E` / `⌘ ^ E`
- **Paste enhanced content**: `Ctrl V` / `Cmd V` (in markdown files)

#### Tips

- Resize editor via ctrl/cmd + mouse scroll
- Hyperlinks can be opened by ctrl/meta + click or double-click
- Image paste and automatic path resolution
- Syntax highlighting with multiple themes support

### Additional Features

- **Icon Theme**: Built-in Material Icon Theme icons
- **Excel Preview**: Support for .xlsx and .csv files with save functionality (note: .xlsx save may lose formatting, .csv doesn't support GBK Chinese encoding)
- **HTML Live Preview**: Press `Ctrl Shift V` to open live preview while editing HTML
- **PDF Preview**: Direct PDF file viewing
- **HTTP Client**: Send HTTP requests (modified integration due to REST Client local request bugs)
- **Registry Editor**: Support for Windows registry files
- **Compressed File Viewer**: Extract and view contents of various archive formats

## Configuration

The extension provides various configuration options in VS Code settings:

- `mditor.enabled`: Enable/disable the extension
- `mditor.previewCode`: Enable code syntax highlighting in preview
- `mditor.previewCodeStyle`: Default syntax highlight style
- `mditor.previewCodeHighlight.showLineNumber`: Show line numbers in code blocks
- `mditor.editorLanguage`: Editor language preference
- `mditor.workspacePathAsImageBasePath`: Use workspace path as markdown image base path
- `mditor.pasterImgPath`: Image paste path template
- `mditor.chromiumPath`: Chromium browser path for PDF export

## Requirements

- Visual Studio Code ^1.64.0
- Internet connection for some features (PDF rendering, font preview)

## Installation

1. Install from VS Code marketplace: Search for "Mditor"
2. Or install via VSIX: Download and install the .vsix file
3. Reload VS Code after installation

## Usage

1. **Markdown**: Open any .md file to start editing with the WYSIWYG editor
2. **Office Files**: Open .xlsx, .docx, .pdf files to preview them
3. **HTML**: Open .html files and press `Ctrl Shift V` for live preview
4. **HTTP Requests**: Create .http files to send API requests
5. **Registry Files**: Open .reg files with syntax highlighting and navigation

## Development

```bash
# Install dependencies
npm install

# Build the extension
npm run build

# Run in development mode
npm run dev

# Package for distribution
npm run package
```

## Sponsor

If you'd like to support the development of this project, you can make a donation via the QR codes below (Alipay / WeChat Pay):

<p>
  <img src="images/alipay.jpg" alt="Alipay Donation" style="width:200px;display:inline-block;margin-right:16px;" />
  <img src="images/wechatpay.jpg" alt="WeChat Pay Donation" style="width:200px;display:inline-block;" />
</p>

## Credits

- **PDF Rendering**: [mozilla/pdf.js/](https://github.com/mozilla/pdf.js/)
- **DOCX Rendering**: [VolodymyrBaydalka/docxjs](https://github.com/VolodymyrBaydalka/docxjs)
- **XLSX Rendering**:
  - [SheetJS/sheetjs](https://github.com/SheetJS/sheetjs): XLSX parsing
  - [myliang/x-spreadsheet](https://github.com/myliang/x-spreadsheet): XLSX rendering
- **HTTP Client**: [Rest Client](https://github.com/Huachao/vscode-restclient)
- **Markdown Editor**: [Vanessa219/vditor](https://github.com/Vanessa219/vditor)
- **Material Icon Theme**: [PKief/vscode-material-icon-theme](https://github.com/PKief/vscode-material-icon-theme)

## License

This project is licensed under the [LGPL-3.0-or-later License](LICENSE).

## Issues and Support

- **Bug Reports**: [GitHub Issues](https://github.com/dreamxwork/mditor-vs/issues)
- **Email Support**: dreamxwork@outlook.com
- **Repository**: [GitHub Repository](https://github.com/dreamxwork/mditor-vs.git)

---

*Last updated: 2024*
