# Mditor

[English](README.md) | [简体中文](README-CN.md) | [繁體中文](README-TW.md) | [日本語](README-JA.md) | [한국어](README-KO.md) | [Français](README-FR.md) | [Deutsch](README-DE.md) | [Español](README-ES.md) | [Русский](README-RU.md)

Une extension VS Code puissante et élégante qui transforme votre expérience d'édition Markdown avec des capacités WYSIWYG et un support complet de prévisualisation de fichiers.

## ✨ Points forts

Mditor apporte des capacités d'édition et de prévisualisation de qualité professionnelle à Visual Studio Code :

- 🎨 **Magnifique éditeur Markdown WYSIWYG** - Aperçu en temps réel avec formatage riche
- 📊 **Visionneuse de fichiers multi-formats** - Prévisualisez les documents Office, PDF et plus
- 🌓 **Support de thèmes multiples** - Magnifiques thèmes clairs et sombres pour une édition confortable
- ⚡ **Ultra rapide** - Performances optimisées pour les documents volumineux
- 🎯 **Convivial pour les développeurs** - Raccourcis clavier riches et interface intuitive

## 📸 Captures d'écran

### Thème clair
![Thème clair](images/light.png)

### Thème sombre
![Thème sombre](images/dark.png)

## 🚀 Fonctionnalités

### Excellence de l'éditeur Markdown

Propulsé par [Vditor](https://github.com/Vanessa219/vditor), notre éditeur WYSIWYG fournit :

- **Aperçu en temps réel** - Voyez votre contenu formaté pendant que vous tapez
- **Formatage riche** - Support des tableaux, blocs de code, diagrammes (Mermaid), formules mathématiques (LaTeX)
- **Collage intelligent** - Téléchargement automatique d'images et résolution de chemin
- **Exportation partout** - Convertissez en PDF, DOCX ou HTML en un clic
- **Variété de thèmes** - Plusieurs beaux thèmes d'éditeur pour correspondre à votre style

#### Raccourcis clavier puissants

Basé sur les [raccourcis Vditor](shortcut.md) avec des fonctionnalités de productivité améliorées :

- **Déplacer la liste vers le haut** : `Ctrl+Alt+I` / `⌘+^+I`
- **Déplacer la liste vers le bas** : `Ctrl+Alt+J` / `⌘+^+J`
- **Éditer dans VS Code** : `Ctrl+Alt+E` / `⌘+^+E`
- **Collage amélioré** : `Ctrl+V` / `Cmd+V` avec gestion automatique des images

#### Fonctionnalités intelligentes

- Zoomer l'éditeur avec `Ctrl/Cmd + Molette de la souris`
- Ouvrir les hyperliens avec `Ctrl/Meta + Clic` ou double-clic
- Insertion d'images par glisser-déposer
- Résolution automatique du chemin d'image
- Coloration syntaxique avec plusieurs options de thème

### Prévisualisation complète de fichiers

Prévisualisez les formats de fichiers courants directement dans VS Code :

- 📊 **Feuilles de calcul** : .xls, .xlsx, .csv (avec capacité d'édition et de sauvegarde)
- 📝 **Documents** : .docx
- 🖼️ **Graphiques** : .svg
- 📄 **PDF** : .pdf (propulsé par PDF.js)
- 🔤 **Polices** : .ttf, .otf, .woff, .woff2
- 📋 **Markdown** : .md, .markdown
- 🌐 **HTTP** : .http, .rest (client HTTP intégré)
- ⚙️ **Registre** : .reg (fichiers de registre Windows)
- 📦 **Archives** : .zip, .jar, .vsix, .rar

### Capacités supplémentaires

- **Icônes Material** - Belles icônes de fichiers du Material Icon Theme
- **Aperçu HTML en direct** - Appuyez sur `Ctrl+Shift+V` pour un aperçu HTML instantané
- **Client HTTP** - Envoyez des requêtes API directement depuis les fichiers .http
- **Éditeur de registre** - Coloration syntaxique pour les fichiers de registre Windows

## 🔧 Configuration

Ajustez finement Mditor via les paramètres VS Code :

| Paramètre | Description |
|-----------|-------------|
| `mditor.enabled` | Activer/désactiver l'extension |
| `mditor.previewCode` | Activer la coloration syntaxique du code dans l'aperçu |
| `mditor.previewCodeStyle` | Style de coloration syntaxique par défaut |
| `mditor.previewCodeHighlight.showLineNumber` | Afficher les numéros de ligne dans les blocs de code |
| `mditor.editorLanguage` | Langue de l'interface de l'éditeur |
| `mditor.workspacePathAsImageBasePath` | Utiliser le chemin de l'espace de travail comme chemin de base d'image |
| `mditor.pasterImgPath` | Modèle de chemin de collage d'image |
| `mditor.chromiumPath` | Chemin Chromium pour l'exportation PDF |

### Basculer vers l'éditeur Markdown natif

Pour utiliser l'éditeur markdown par défaut de VS Code, ajoutez à `settings.json` :

```json
{
    "workbench.editorAssociations": {
        "*.md": "default",
        "*.markdown": "default"
    }
}
```

## 📋 Exigences

- Visual Studio Code `^1.64.0`
- Connexion Internet (pour certaines fonctionnalités d'aperçu)

## 📥 Installation

### Depuis le Marketplace
1. Ouvrir VS Code
2. Aller dans Extensions (`Ctrl+Shift+X`)
3. Rechercher "Mditor"
4. Cliquer sur Installer

### Depuis VSIX
1. Télécharger le dernier fichier .vsix
2. Ouvrir VS Code
3. Extensions → `...` → Installer depuis VSIX
4. Sélectionner le fichier téléchargé

## 🎯 Démarrage rapide

1. **Édition Markdown** : Ouvrir n'importe quel fichier `.md` - l'éditeur WYSIWYG se lance automatiquement
2. **Aperçu Office** : Cliquer sur les fichiers `.xlsx`, `.docx`, `.pdf` pour prévisualiser
3. **Aperçu HTML** : Ouvrir les fichiers `.html` et appuyer sur `Ctrl+Shift+V`
4. **Requêtes HTTP** : Créer des fichiers `.http` pour tester les API
5. **Visualisation d'archives** : Ouvrir `.zip` ou autres archives pour parcourir le contenu

## 📖 Exemples Markdown

Vous voulez voir ce que Mditor peut faire ? Consultez notre fichier d'exemples Markdown complet qui présente toutes les fonctionnalités prises en charge :

**[Télécharger markdown-examples.md](https://raw.githubusercontent.com/dreamxwork/mditor-vs/main/markdown-examples.md)**

Ce fichier d'exemples comprend :
- Formatage de texte de base (titres, gras, italique, listes)
- Blocs de code avec coloration syntaxique (C++, Java, Python, Shell, CMake, fichiers journaux)
- Diagrammes Mermaid (organigrammes, diagrammes de séquence, diagrammes de classes, diagrammes de Gantt, graphiques de branches Git)
- Formules mathématiques (LaTeX)
- Tableaux et visualisation de données
- Notation musicale (notation ABC)
- Diagrammes Graphviz
- Visualisation de données ECharts
- Et bien plus encore !

## 🛠️ Développement

```bash
# Installer les dépendances
npm install

# Construire l'extension
npm run build

# Mode développement avec rechargement à chaud
npm run dev

# Empaqueter pour la distribution
npm run package
```

## 💖 Soutenir ce projet

Si vous trouvez Mditor utile, envisagez de soutenir son développement :

### Dons internationaux
[![PayPal](https://img.shields.io/badge/PayPal-Donate-blue.svg?logo=paypal)](https://www.paypal.me/howpigcanfly)

**Compte PayPal** : howpigcanfly@outlook.com

### Dons en cryptomonnaies
**Bitcoin (BTC)** : `13KGRMK3AGMNxQqdC5yyNRi7cpmD3mQhAM`

### Dons en Chine continentale
<p>
  <img src="images/alipay.jpg" alt="Don Alipay" width="200" style="display:inline-block;margin-right:16px;" />
  <img src="images/wechatpay.jpg" alt="Don WeChat Pay" width="200" style="display:inline-block;" />
</p>

**Alipay / WeChat Pay** : Scannez les codes QR ci-dessus

### Virement bancaire
Pour les dons par virement bancaire, veuillez contacter : dreamxwork@outlook.com

---

Vos dons aident à maintenir et améliorer ce projet. Merci pour votre soutien !

## 🙏 Crédits

Ce projet est construit sur les épaules de géants :

- **Rendu PDF** : [mozilla/pdf.js](https://github.com/mozilla/pdf.js/)
- **Rendu DOCX** : [VolodymyrBaydalka/docxjs](https://github.com/VolodymyrBaydalka/docxjs)
- **Traitement XLSX** :
  - [SheetJS/sheetjs](https://github.com/SheetJS/sheetjs) - Analyse Excel
  - [myliang/x-spreadsheet](https://github.com/myliang/x-spreadsheet) - Interface de feuille de calcul
- **Client HTTP** : [Rest Client](https://github.com/Huachao/vscode-restclient)
- **Moteur Markdown** : [Vanessa219/vditor](https://github.com/Vanessa219/vditor)
- **Thème d'icônes** : [PKief/vscode-material-icon-theme](https://github.com/PKief/vscode-material-icon-theme)

## 📜 Licence

Ce projet est sous licence [LGPL-3.0-or-later](LICENSE).

## 📞 Contact et support

- **Dépôt** : [https://github.com/dreamxwork/mditor-vs](https://github.com/dreamxwork/mditor-vs)
- **Problèmes** : [GitHub Issues](https://github.com/dreamxwork/mditor-vs/issues)
- **Email** : dreamxwork@outlook.com

---

Fait avec ❤️ par l'équipe Mditor | *Dernière mise à jour : 2026*
