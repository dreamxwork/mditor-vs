# Mditor

[English](README.md) | [简体中文](README-CN.md) | [繁體中文](README-TW.md) | [日本語](README-JA.md)

一款強大而優雅的 VS Code 擴充功能，透過所見即所得的編輯能力和全面的檔案預覽支援，徹底改變您的 Markdown 編輯體驗。

## ✨ 特色亮點

Mditor 為 Visual Studio Code 帶來專業級的編輯和預覽功能：

- 🎨 **精美的所見即所得 Markdown 編輯器** - 即時預覽，豐富格式
- 📊 **多格式檔案檢視器** - 預覽 Office 文件、PDF 等
- 🌓 **多主題支援** - 華麗的明暗主題，舒適編輯
- ⚡ **閃電般快速** - 為大型文件最佳化的效能
- 🎯 **開發者友善** - 豐富的鍵盤快速鍵和直覺介面

## 📸 截圖展示

### 淺色主題
![淺色主題](images/light.png)

### 深色主題
![深色主題](images/dark.png)

## 🚀 功能特性

### 卓越的 Markdown 編輯器

基於 [Vditor](https://github.com/Vanessa219/vditor) 建構，我們的所見即所得編輯器提供：

- **即時預覽** - 輸入即可看到格式化內容
- **豐富格式** - 支援表格、程式碼區塊、圖表（Mermaid）、數學公式（LaTeX）
- **智慧貼上** - 自動圖片上傳和路徑解析
- **隨處匯出** - 一鍵轉換為 PDF、DOCX 或 HTML
- **主題多樣** - 多種精美編輯器主題，符合您的風格

#### 強大的快速鍵

基於 [Vditor 快速鍵](shortcut.md)，並增強了生產力功能：

- **清單上移**: `Ctrl+Alt+I` / `⌘+^+I`
- **清單下移**: `Ctrl+Alt+J` / `⌘+^+J`
- **在 VS Code 中編輯**: `Ctrl+Alt+E` / `⌘+^+E`
- **增強貼上**: `Ctrl+V` / `Cmd+V` 自動處理圖片

#### 智慧功能

- 使用 `Ctrl/Cmd + 滑鼠滾輪` 縮放編輯器
- 使用 `Ctrl/Meta + 點擊` 或雙擊開啟超連結
- 拖放插入圖片
- 自動圖片路徑解析
- 多主題選項的語法醒目提示

### 全面的檔案預覽

直接在 VS Code 中預覽常見檔案格式：

- 📊 **試算表**: .xls, .xlsx, .csv（支援編輯和儲存）
- 📝 **文件**: .docx
- 🖼️ **圖形**: .svg
- 📄 **PDF**: .pdf（由 PDF.js 驅動）
- 🔤 **字型**: .ttf, .otf, .woff, .woff2
- 📋 **Markdown**: .md, .markdown
- 🌐 **HTTP**: .http, .rest（整合 HTTP 用戶端）
- ⚙️ **登錄檔**: .reg（Windows 登錄檔檔案）
- 📦 **壓縮檔**: .zip, .jar, .vsix, .rar

### 其他功能

- **Material 圖示** - 來自 Material Icon Theme 的精美檔案圖示
- **HTML 即時預覽** - 按 `Ctrl+Shift+V` 即時預覽 HTML
- **HTTP 用戶端** - 直接從 .http 檔案傳送 API 請求
- **登錄檔編輯器** - Windows 登錄檔檔案的語法醒目提示

## 🔧 設定選項

透過 VS Code 設定微調 Mditor：

| 設定項 | 說明 |
|--------|------|
| `mditor.enabled` | 啟用/停用擴充功能 |
| `mditor.previewCode` | 在預覽中啟用程式碼語法醒目提示 |
| `mditor.previewCodeStyle` | 預設語法醒目提示樣式 |
| `mditor.previewCodeHighlight.showLineNumber` | 在程式碼區塊中顯示行號 |
| `mditor.editorLanguage` | 編輯器介面語言 |
| `mditor.workspacePathAsImageBasePath` | 使用工作區路徑作為圖片基礎路徑 |
| `mditor.pasterImgPath` | 圖片貼上路徑範本 |
| `mditor.chromiumPath` | PDF 匯出的 Chromium 路徑 |

### 切換到原生 Markdown 編輯器

要使用 VS Code 預設的 markdown 編輯器，在 `settings.json` 中新增：

```json
{
    "workbench.editorAssociations": {
        "*.md": "default",
        "*.markdown": "default"
    }
}
```

## 📋 系統需求

- Visual Studio Code `^1.64.0`
- 網路連線（某些預覽功能需要）

## 📥 安裝方法

### 從市集安裝
1. 開啟 VS Code
2. 進入擴充功能（`Ctrl+Shift+X`）
3. 搜尋「Mditor」
4. 點擊安裝

### 從 VSIX 安裝
1. 下載最新的 .vsix 檔案
2. 開啟 VS Code
3. 擴充功能 → `...` → 從 VSIX 安裝
4. 選擇下載的檔案

## 🎯 快速開始

1. **Markdown 編輯**: 開啟任何 `.md` 檔案 - 所見即所得編輯器自動啟動
2. **Office 預覽**: 點擊 `.xlsx`、`.docx`、`.pdf` 檔案進行預覽
3. **HTML 預覽**: 開啟 `.html` 檔案並按 `Ctrl+Shift+V`
4. **HTTP 請求**: 建立 `.http` 檔案測試 API
5. **壓縮檔檢視**: 開啟 `.zip` 或其他壓縮檔瀏覽內容

## 🛠️ 開發

```bash
# 安裝相依套件
npm install

# 建置擴充功能
npm run build

# 開發模式（熱重載）
npm run dev

# 封裝發布
npm run package
```

## 💖 支援本專案

如果您覺得 Mditor 有幫助，請考慮支援其開發：

<p>
  <img src="images/alipay.jpg" alt="支付寶捐贈" width="200" style="display:inline-block;margin-right:16px;" />
  <img src="images/wechatpay.jpg" alt="微信支付捐贈" width="200" style="display:inline-block;" />
</p>

您的捐贈有助於維護和改進本專案。感謝您的支援！

## 🙏 致謝

本專案基於以下優秀開源專案建構：

- **PDF 渲染**: [mozilla/pdf.js](https://github.com/mozilla/pdf.js/)
- **DOCX 渲染**: [VolodymyrBaydalka/docxjs](https://github.com/VolodymyrBaydalka/docxjs)
- **XLSX 處理**:
  - [SheetJS/sheetjs](https://github.com/SheetJS/sheetjs) - Excel 解析
  - [myliang/x-spreadsheet](https://github.com/myliang/x-spreadsheet) - 試算表介面
- **HTTP 用戶端**: [Rest Client](https://github.com/Huachao/vscode-restclient)
- **Markdown 引擎**: [Vanessa219/vditor](https://github.com/Vanessa219/vditor)
- **圖示主題**: [PKief/vscode-material-icon-theme](https://github.com/PKief/vscode-material-icon-theme)

## 📜 授權條款

本專案採用 [LGPL-3.0-or-later 授權條款](LICENSE)。

## 📞 聯絡與支援

- **專案倉庫**: [https://github.com/dreamxwork/mditor-vs](https://github.com/dreamxwork/mditor-vs)
- **問題回饋**: [GitHub Issues](https://github.com/dreamxwork/mditor-vs/issues)
- **電子郵件**: dreamxwork@outlook.com

---

用 ❤️ 製作，來自 Mditor 團隊 | *最後更新：2026 年*
