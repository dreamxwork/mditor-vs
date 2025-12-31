# Mditor

[English](README.md) | [简体中文](README-CN.md) | [繁體中文](README-TW.md) | [日本語](README-JA.md)

一款强大而优雅的 VS Code 扩展，通过所见即所得的编辑能力和全面的文件预览支持，彻底改变您的 Markdown 编辑体验。

## ✨ 特色亮点

Mditor 为 Visual Studio Code 带来专业级的编辑和预览功能：

- 🎨 **精美的所见即所得 Markdown 编辑器** - 实时预览，丰富格式
- 📊 **多格式文件查看器** - 预览 Office 文档、PDF 等
- 🌓 **多主题支持** - 华丽的明暗主题，舒适编辑
- ⚡ **闪电般快速** - 为大型文档优化的性能
- 🎯 **开发者友好** - 丰富的键盘快捷键和直观界面

## 📸 截图展示

### 浅色主题
![浅色主题](images/light.png)

### 深色主题
![深色主题](images/dark.png)

## 🚀 功能特性

### 卓越的 Markdown 编辑器

基于 [Vditor](https://github.com/Vanessa219/vditor) 构建，我们的所见即所得编辑器提供：

- **实时预览** - 输入即可看到格式化内容
- **丰富格式** - 支持表格、代码块、图表（Mermaid）、数学公式（LaTeX）
- **智能粘贴** - 自动图片上传和路径解析
- **随处导出** - 一键转换为 PDF、DOCX 或 HTML
- **主题多样** - 多种精美编辑器主题，匹配您的风格

#### 强大的快捷键

基于 [Vditor 快捷键](shortcut.md)，并增强了生产力功能：

- **列表上移**: `Ctrl+Alt+I` / `⌘+^+I`
- **列表下移**: `Ctrl+Alt+J` / `⌘+^+J`
- **在 VS Code 中编辑**: `Ctrl+Alt+E` / `⌘+^+E`
- **增强粘贴**: `Ctrl+V` / `Cmd+V` 自动处理图片

#### 智能功能

- 使用 `Ctrl/Cmd + 鼠标滚轮` 缩放编辑器
- 使用 `Ctrl/Meta + 点击` 或双击打开超链接
- 拖放插入图片
- 自动图片路径解析
- 多主题选项的语法高亮

### 全面的文件预览

直接在 VS Code 中预览常见文件格式：

- 📊 **电子表格**: .xls, .xlsx, .csv（支持编辑和保存）
- 📝 **文档**: .docx
- 🖼️ **图形**: .svg
- 📄 **PDF**: .pdf（由 PDF.js 驱动）
- 🔤 **字体**: .ttf, .otf, .woff, .woff2
- 📋 **Markdown**: .md, .markdown
- 🌐 **HTTP**: .http, .rest（集成 HTTP 客户端）
- ⚙️ **注册表**: .reg（Windows 注册表文件）
- 📦 **压缩包**: .zip, .jar, .vsix, .rar

### 其他功能

- **Material 图标** - 来自 Material Icon Theme 的精美文件图标
- **HTML 实时预览** - 按 `Ctrl+Shift+V` 即时预览 HTML
- **HTTP 客户端** - 直接从 .http 文件发送 API 请求
- **注册表编辑器** - Windows 注册表文件的语法高亮

## 🔧 配置选项

通过 VS Code 设置微调 Mditor：

| 设置项 | 说明 |
|--------|------|
| `mditor.enabled` | 启用/禁用扩展 |
| `mditor.previewCode` | 在预览中启用代码语法高亮 |
| `mditor.previewCodeStyle` | 默认语法高亮样式 |
| `mditor.previewCodeHighlight.showLineNumber` | 在代码块中显示行号 |
| `mditor.editorLanguage` | 编辑器界面语言 |
| `mditor.workspacePathAsImageBasePath` | 使用工作区路径作为图片基础路径 |
| `mditor.pasterImgPath` | 图片粘贴路径模板 |
| `mditor.chromiumPath` | PDF 导出的 Chromium 路径 |

### 切换到原生 Markdown 编辑器

要使用 VS Code 默认的 markdown 编辑器，在 `settings.json` 中添加：

```json
{
    "workbench.editorAssociations": {
        "*.md": "default",
        "*.markdown": "default"
    }
}
```

## 📋 系统要求

- Visual Studio Code `^1.64.0`
- 网络连接（某些预览功能需要）

## 📥 安装方法

### 从市场安装
1. 打开 VS Code
2. 进入扩展（`Ctrl+Shift+X`）
3. 搜索"Mditor"
4. 点击安装

### 从 VSIX 安装
1. 下载最新的 .vsix 文件
2. 打开 VS Code
3. 扩展 → `...` → 从 VSIX 安装
4. 选择下载的文件

## 🎯 快速开始

1. **Markdown 编辑**: 打开任何 `.md` 文件 - 所见即所得编辑器自动启动
2. **Office 预览**: 点击 `.xlsx`、`.docx`、`.pdf` 文件进行预览
3. **HTML 预览**: 打开 `.html` 文件并按 `Ctrl+Shift+V`
4. **HTTP 请求**: 创建 `.http` 文件测试 API
5. **压缩包查看**: 打开 `.zip` 或其他压缩包浏览内容

## 🛠️ 开发

```bash
# 安装依赖
npm install

# 构建扩展
npm run build

# 开发模式（热重载）
npm run dev

# 打包发布
npm run package
```

## 💖 支持本项目

如果您觉得 Mditor 有帮助，请考虑支持其开发：

### 国际捐赠
[![PayPal](https://img.shields.io/badge/PayPal-Donate-blue.svg?logo=paypal)](https://www.paypal.me/howpigcanfly)

**PayPal 账号**: howpigcanfly@outlook.com

### 中国大陆捐赠
<p>
  <img src="images/alipay.jpg" alt="支付宝捐赠" width="200" style="display:inline-block;margin-right:16px;" />
  <img src="images/wechatpay.jpg" alt="微信支付捐赠" width="200" style="display:inline-block;" />
</p>

**支付宝 / 微信支付**: 扫描上方二维码

### 银行转账
如需银行转账捐赠，请联系：dreamxwork@outlook.com

---

您的捐赠有助于维护和改进本项目。感谢您的支持！

## 🙏 致谢

本项目基于以下优秀开源项目构建：

- **PDF 渲染**: [mozilla/pdf.js](https://github.com/mozilla/pdf.js/)
- **DOCX 渲染**: [VolodymyrBaydalka/docxjs](https://github.com/VolodymyrBaydalka/docxjs)
- **XLSX 处理**:
  - [SheetJS/sheetjs](https://github.com/SheetJS/sheetjs) - Excel 解析
  - [myliang/x-spreadsheet](https://github.com/myliang/x-spreadsheet) - 电子表格界面
- **HTTP 客户端**: [Rest Client](https://github.com/Huachao/vscode-restclient)
- **Markdown 引擎**: [Vanessa219/vditor](https://github.com/Vanessa219/vditor)
- **图标主题**: [PKief/vscode-material-icon-theme](https://github.com/PKief/vscode-material-icon-theme)

## 📜 许可证

本项目采用 [LGPL-3.0-or-later 许可证](LICENSE)。

## 📞 联系与支持

- **项目仓库**: [https://github.com/dreamxwork/mditor-vs](https://github.com/dreamxwork/mditor-vs)
- **问题反馈**: [GitHub Issues](https://github.com/dreamxwork/mditor-vs/issues)
- **电子邮件**: dreamxwork@outlook.com

---

用 ❤️ 制作，来自 Mditor 团队 | *最后更新：2026 年*
