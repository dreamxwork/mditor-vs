# Mditor

## 介紹

English | [简体中文](README-CN.md) | [繁體中文](README-TW.md)

Mditor是一個功能強大的Visual Studio Code擴展，提供全面的文件預覽功能和所見即所得的Markdown編輯器。此擴展支持在VS Code中預覽各種常見的辦公文件格式。

## 支援的文件格式

本擴展支援在VS Code中預覽以下常見的富文件格式：

- **Excel**: .xls, .xlsx, .csv
- **Word**: .docx
- **SVG**: .svg
- **PDF**: .pdf
- **字體**: .ttf, .otf, .woff, .woff2
- **Markdown**: .md, .markdown
- **HTTP請求**: .http, .rest
- **Windows登錄檔**: .reg
- **壓縮文件**: .zip, .jar, .vsix, .rar

## 功能特性

### Markdown編輯器

本擴展整合[Vditor](https://github.com/Vanessa219/vditor)實現對Markdown的所見即所得編輯。

如果你需要使用原生的VS Code Markdown編輯器，在你的`settings.json`中新增以下配置：

```json
{
    "workbench.editorAssociations": {
        "*.md": "default",
        "*.markdown": "default"
    }
}
```

#### 匯出選項

在Markdown編輯器中右鍵可以將文件匯出為PDF、DOCX或HTML格式。PDF匯出依賴Chromium，可透過`mditor.chromiumPath`配置。

![匯出選項](image/README-CN/1685418034035.png)

#### 快速鍵

基於[Vditor快速鍵](shortcut.md)以及更多功能：

- **將清單上移一行**: `Ctrl Alt I` / `⌘ ^ I`
- **將清單下移一行**: `Ctrl Alt J` / `⌘ ^ J`
- **在VS Code中編輯**: `Ctrl Alt E` / `⌘ ^ E`
- **貼上增強內容**: `Ctrl V` / `Cmd V`（在Markdown文件中）

#### 使用提示

- 透過ctrl/cmd + 滑鼠滾輪調整編輯器大小
- 超連結可以透過ctrl/meta + 點擊或雙擊開啟
- 圖片貼上和自動路徑解析
- 多主題支援的語法高亮

### 其他功能

- **圖示主題**: 內建Material Icon Theme圖示
- **Excel預覽**: 支援.xlsx和.csv文件的預覽和儲存功能（注意：.xlsx儲存可能會遺失格式，.csv不支援GBK中文編碼）
- **HTML即時預覽**: 編輯HTML時按`Ctrl Shift V`開啟即時預覽
- **PDF預覽**: 直接預覽PDF文件
- **HTTP客戶端**: 發送HTTP請求（由於REST Client本地請求有bug，進行了修改整合）
- **登錄檔編輯器**: 支援Windows登錄檔文件
- **壓縮文件檢視器**: 提取並檢視各種壓縮格式的內容

## 設定選項

擴展在VS Code設定中提供各種配置選項：

- `mditor.enabled`: 啟用/停用擴展
- `mditor.previewCode`: 在預覽中啟用程式碼語法高亮
- `mditor.previewCodeStyle`: 預設語法高亮樣式
- `mditor.previewCodeHighlight.showLineNumber`: 在程式碼區塊中顯示行號
- `mditor.editorLanguage`: 編輯器語言偏好
- `mditor.workspacePathAsImageBasePath`: 使用工作區路徑作為Markdown圖片基礎路徑
- `mditor.pasterImgPath`: 圖片貼上路徑範本
- `mditor.chromiumPath`: PDF匯出的Chromium瀏覽器路徑

## 系統需求

- Visual Studio Code ^1.64.0
- 某些功能需要網路連線（PDF渲染，字體預覽）

## 安裝方法

1. 從VS Code市集安裝：搜尋"Mditor"
2. 或透過VSIX安裝：下載並安裝.vsix文件
3. 安裝後重新載入VS Code

## 使用方法

1. **Markdown**: 開啟任何.md文件開始使用所見即所得編輯器編輯
2. **辦公文件**: 開啟.xlsx、.docx、.pdf文件進行預覽
3. **HTML**: 開啟.html文件並按`Ctrl Shift V`進行即時預覽
4. **HTTP請求**: 建立.http文件發送API請求
5. **登錄檔文件**: 開啟.reg文件獲得語法高亮和導航功能

## 開發

```bash
# 安裝依賴
npm install

# 建置擴展
npm run build

# 開發模式執行
npm run dev

# 封裝發布
npm run package
```

## 贊助支援

如果你願意支援本項目的開發，可以透過下面的二維碼進行捐助（支付寶 / 微信）：

<p>
  <img src="images/alipay.jpg" alt="Alipay 捐助" style="width:200px;display:inline-block;margin-right:16px;" />
  <img src="images/wechatpay.jpg" alt="WeChat Pay 捐助" style="width:200px;display:inline-block;" />
</p>

掃描任一二維碼即可完成捐助。若無法顯示，請確保倉庫中存在`images/alipay.jpg`和`images/wechatpay.jpg`文件。

## 致謝

- **PDF渲染**: [mozilla/pdf.js/](https://github.com/mozilla/pdf.js/)
- **DOCX渲染**: [VolodymyrBaydalka/docxjs](https://github.com/VolodymyrBaydalka/docxjs)
- **XLSX渲染**:
  - [SheetJS/sheetjs](https://github.com/SheetJS/sheetjs): XLSX解析
  - [myliang/x-spreadsheet](https://github.com/myliang/x-spreadsheet): XLSX渲染
- **HTTP客戶端**: [Rest Client](https://github.com/Huachao/vscode-restclient)
- **Markdown編輯器**: [Vanessa219/vditor](https://github.com/Vanessa219/vditor)
- **圖示主題**: [PKief/vscode-material-icon-theme](https://github.com/PKief/vscode-material-icon-theme)

## 授權條款

本專案採用[LGPL-3.0-or-later授權條款](LICENSE)。

## 問題回饋和支援

- **錯誤報告**: [GitHub Issues](https://github.com/dreamxwork/mditor-vs/issues)
- **郵件支援**: dreamxwork@outlook.com
- **專案倉庫**: [GitHub Repository](https://github.com/dreamxwork/mditor-vs.git)

---

*最後更新: 2024年*
