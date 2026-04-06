# Mditor

[English](README.md) | [简体中文](README-CN.md) | [繁體中文](README-TW.md) | [日本語](README-JA.md) | [한국어](README-KO.md) | [Français](README-FR.md) | [Deutsch](README-DE.md) | [Español](README-ES.md) | [Русский](README-RU.md)

Eine leistungsstarke und elegante VS Code-Erweiterung, die Ihr Markdown-Bearbeitungserlebnis mit WYSIWYG-Funktionen und umfassender Dateivorschau-Unterstützung transformiert.

## ✨ Highlights

Mditor bringt professionelle Bearbeitungs- und Vorschaufunktionen zu Visual Studio Code:

- 🎨 **Wunderschöner WYSIWYG Markdown-Editor** - Echtzeit-Vorschau mit reichhaltiger Formatierung
- 📊 **Multi-Format-Dateibetrachter** - Vorschau von Office-Dokumenten, PDFs und mehr
- 🌓 **Mehrere Theme-Unterstützung** - Wunderschöne helle und dunkle Themes für komfortables Bearbeiten
- ⚡ **Blitzschnell** - Optimierte Leistung für große Dokumente
- 🎯 **Entwicklerfreundlich** - Umfangreiche Tastenkombinationen und intuitive Benutzeroberfläche

## 📸 Screenshots

### Helles Theme
![Helles Theme](images/light.png)

### Dunkles Theme
![Dunkles Theme](images/dark.png)

## 🚀 Funktionen

### Exzellenter Markdown-Editor

Angetrieben von [Vditor](https://github.com/Vanessa219/vditor), bietet unser WYSIWYG-Editor:

- **Echtzeit-Vorschau** - Sehen Sie Ihren formatierten Inhalt während der Eingabe
- **Reichhaltige Formatierung** - Unterstützung für Tabellen, Codeblöcke, Diagramme (Mermaid), mathematische Formeln (LaTeX)
- **Intelligentes Einfügen** - Automatischer Bild-Upload und Pfadauflösung
- **Überall exportieren** - Mit einem Klick in PDF, DOCX oder HTML konvertieren
- **Theme-Vielfalt** - Mehrere schöne Editor-Themes passend zu Ihrem Stil

#### Leistungsstarke Tastenkombinationen

Basierend auf [Vditor-Shortcuts](shortcut.md) mit erweiterten Produktivitätsfunktionen:

- **Liste nach oben verschieben**: `Ctrl+Alt+I` / `⌘+^+I`
- **Liste nach unten verschieben**: `Ctrl+Alt+J` / `⌘+^+J`
- **In VS Code bearbeiten**: `Ctrl+Alt+E` / `⌘+^+E`
- **Erweitertes Einfügen**: `Ctrl+V` / `Cmd+V` mit automatischer Bildverarbeitung

#### Intelligente Funktionen

- Editor mit `Ctrl/Cmd + Mausrad` zoomen
- Hyperlinks mit `Ctrl/Meta + Klick` oder Doppelklick öffnen
- Bilder per Drag & Drop einfügen
- Automatische Bildpfadauflösung
- Syntax-Hervorhebung mit mehreren Theme-Optionen

### Umfassende Dateivorschau

Vorschau gängiger Dateiformate direkt in VS Code:

- 📊 **Tabellenkalkulationen**: .xls, .xlsx, .csv (mit Bearbeitungs- und Speicherfunktion)
- 📝 **Dokumente**: .docx
- 🖼️ **Grafiken**: .svg
- 📄 **PDFs**: .pdf (angetrieben von PDF.js)
- 🔤 **Schriftarten**: .ttf, .otf, .woff, .woff2
- 📋 **Markdown**: .md, .markdown
- 🌐 **HTTP**: .http, .rest (integrierter HTTP-Client)
- ⚙️ **Registry**: .reg (Windows-Registry-Dateien)
- 📦 **Archive**: .zip, .jar, .vsix, .rar

### Zusätzliche Funktionen

- **Material-Icons** - Schöne Datei-Icons vom Material Icon Theme
- **Live-HTML-Vorschau** - Drücken Sie `Ctrl+Shift+V` für sofortige HTML-Vorschau
- **HTTP-Client** - API-Anfragen direkt aus .http-Dateien senden
- **Registry-Editor** - Syntax-Hervorhebung für Windows-Registry-Dateien

## 🔧 Konfiguration

Mditor über VS Code-Einstellungen feinabstimmen:

| Einstellung | Beschreibung |
|-------------|--------------|
| `mditor.enabled` | Erweiterung aktivieren/deaktivieren |
| `mditor.previewCode` | Code-Syntax-Hervorhebung in der Vorschau aktivieren |
| `mditor.previewCodeStyle` | Standard-Syntax-Hervorhebungsstil |
| `mditor.previewCodeHighlight.showLineNumber` | Zeilennummern in Codeblöcken anzeigen |
| `mditor.editorLanguage` | Editor-UI-Sprache |
| `mditor.workspacePathAsImageBasePath` | Workspace-Pfad als Bild-Basispfad verwenden |
| `mditor.pasterImgPath` | Bild-Einfügen-Pfadvorlage |
| `mditor.chromiumPath` | Chromium-Pfad für PDF-Export |

### Zum nativen Markdown-Editor wechseln

Um den Standard-Markdown-Editor von VS Code zu verwenden, fügen Sie zu `settings.json` hinzu:

```json
{
    "workbench.editorAssociations": {
        "*.md": "default",
        "*.markdown": "default"
    }
}
```

## 📋 Anforderungen

- Visual Studio Code `^1.64.0`
- Internetverbindung (für einige Vorschaufunktionen)

## 📥 Installation

### Vom Marketplace
1. VS Code öffnen
2. Zu Erweiterungen gehen (`Ctrl+Shift+X`)
3. Nach "Mditor" suchen
4. Auf Installieren klicken

### Von VSIX
1. Neueste .vsix-Datei herunterladen
2. VS Code öffnen
3. Erweiterungen → `...` → Von VSIX installieren
4. Heruntergeladene Datei auswählen

## 🎯 Schnellstart

1. **Markdown-Bearbeitung**: Beliebige `.md`-Datei öffnen - der WYSIWYG-Editor startet automatisch
2. **Office-Vorschau**: Auf `.xlsx`-, `.docx`-, `.pdf`-Dateien klicken, um Vorschau anzuzeigen
3. **HTML-Vorschau**: `.html`-Dateien öffnen und `Ctrl+Shift+V` drücken
4. **HTTP-Anfragen**: `.http`-Dateien erstellen, um APIs zu testen
5. **Archiv-Anzeige**: `.zip` oder andere Archive öffnen, um Inhalte zu durchsuchen

## 📖 Markdown-Beispiele

Möchten Sie sehen, was Mditor kann? Schauen Sie sich unsere umfassende Markdown-Beispieldatei an, die alle unterstützten Funktionen zeigt:

**[markdown-examples.md herunterladen](https://raw.githubusercontent.com/dreamxwork/mditor-vs/main/markdown-examples.md)**

Diese Beispieldatei enthält:
- Grundlegende Textformatierung (Überschriften, Fett, Kursiv, Listen)
- Codeblöcke mit Syntax-Hervorhebung (C++, Java, Python, Shell, CMake, Log-Dateien)
- Mermaid-Diagramme (Flussdiagramme, Sequenzdiagramme, Klassendiagramme, Gantt-Diagramme, Git-Branch-Graphen)
- Mathematische Formeln (LaTeX)
- Tabellen und Datenvisualisierung
- Musiknotation (ABC-Notation)
- Graphviz-Diagramme
- ECharts-Datenvisualisierung
- Und vieles mehr!

## 🛠️ Entwicklung

```bash
# Abhängigkeiten installieren
npm install

# Erweiterung erstellen
npm run build

# Entwicklungsmodus mit Hot Reload
npm run dev

# Für Verteilung paketieren
npm run package
```

## 💖 Dieses Projekt unterstützen

Wenn Sie Mditor hilfreich finden, erwägen Sie, seine Entwicklung zu unterstützen:

### Internationale Spenden
[![PayPal](https://img.shields.io/badge/PayPal-Donate-blue.svg?logo=paypal)](https://www.paypal.me/howpigcanfly)

**PayPal-Konto**: howpigcanfly@outlook.com

### Krypto-Spenden
**Bitcoin (BTC)**: `13KGRMK3AGMNxQqdC5yyNRi7cpmD3mQhAM`

### Spenden aus Festlandchina
<p>
  <img src="images/alipay.jpg" alt="Alipay-Spende" width="200" style="display:inline-block;margin-right:16px;" />
  <img src="images/wechatpay.jpg" alt="WeChat Pay-Spende" width="200" style="display:inline-block;" />
</p>

**Alipay / WeChat Pay**: QR-Codes oben scannen

### Banküberweisung
Für Spenden per Banküberweisung kontaktieren Sie bitte: dreamxwork@outlook.com

---

Ihre Spenden helfen, dieses Projekt zu pflegen und zu verbessern. Vielen Dank für Ihre Unterstützung!

## 🙏 Danksagungen

Dieses Projekt steht auf den Schultern von Giganten:

- **PDF-Rendering**: [mozilla/pdf.js](https://github.com/mozilla/pdf.js/)
- **DOCX-Rendering**: [VolodymyrBaydalka/docxjs](https://github.com/VolodymyrBaydalka/docxjs)
- **XLSX-Verarbeitung**:
  - [SheetJS/sheetjs](https://github.com/SheetJS/sheetjs) - Excel-Parsing
  - [myliang/x-spreadsheet](https://github.com/myliang/x-spreadsheet) - Tabellenkalkulations-UI
- **HTTP-Client**: [Rest Client](https://github.com/Huachao/vscode-restclient)
- **Markdown-Engine**: [Vanessa219/vditor](https://github.com/Vanessa219/vditor)
- **Icon-Theme**: [PKief/vscode-material-icon-theme](https://github.com/PKief/vscode-material-icon-theme)

## 📜 Lizenz

Dieses Projekt ist unter der [LGPL-3.0-or-later-Lizenz](LICENSE) lizenziert.

## 📞 Kontakt & Support

- **Repository**: [https://github.com/dreamxwork/mditor-vs](https://github.com/dreamxwork/mditor-vs)
- **Issues**: [GitHub Issues](https://github.com/dreamxwork/mditor-vs/issues)
- **E-Mail**: dreamxwork@outlook.com

---

Mit ❤️ erstellt vom Mditor-Team | *Zuletzt aktualisiert: 2026*
