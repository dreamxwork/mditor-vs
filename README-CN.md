# Mditor

## 介绍

English | [简体中文](README-CN.md) | [繁體中文](README-TW.md)

Mditor是一个功能强大的Visual Studio Code扩展，提供全面的文件预览功能和所见即所得的Markdown编辑器。此扩展支持在VS Code中预览各种常见的办公文件格式。

## 支持的文件格式

本扩展支持在VS Code中预览以下常见的富文件格式：

- **Excel**: .xls, .xlsx, .csv
- **Word**: .docx
- **SVG**: .svg
- **PDF**: .pdf
- **字体**: .ttf, .otf, .woff, .woff2
- **Markdown**: .md, .markdown
- **HTTP请求**: .http, .rest
- **Windows注册表**: .reg
- **压缩文件**: .zip, .jar, .vsix, .rar

## 功能特性

### Markdown编辑器

本扩展集成[Vditor](https://github.com/Vanessa219/vditor)实现对Markdown的所见即所得编辑。

如果你需要使用原生的VS Code Markdown编辑器，在你的`settings.json`中添加以下配置：

```json
{
    "workbench.editorAssociations": {
        "*.md": "default",
        "*.markdown": "default"
    }
}
```

#### 导出选项

在Markdown编辑器中右键可以将文件导出为PDF、DOCX或HTML格式。PDF导出依赖Chromium，可通过`mditor.chromiumPath`配置。

![导出选项](image/README-CN/1685418034035.png)

#### 快捷键

基于[Vditor快捷键](shortcut.md)以及更多功能：

- **将列表上移一行**: `Ctrl Alt I` / `⌘ ^ I`
- **将列表下移一行**: `Ctrl Alt J` / `⌘ ^ J`
- **在VS Code中编辑**: `Ctrl Alt E` / `⌘ ^ E`
- **粘贴增强内容**: `Ctrl V` / `Cmd V`（在Markdown文件中）

#### 使用提示

- 通过ctrl/cmd + 鼠标滚轮调整编辑器大小
- 超链接可以通过ctrl/meta + 点击或双击打开
- 图片粘贴和自动路径解析
- 多主题支持的语法高亮

### 其他功能

- **图标主题**: 内置Material Icon Theme图标
- **Excel预览**: 支持.xlsx和.csv文件的预览和保存功能（注意：.xlsx保存可能会丢失格式，.csv不支持GBK中文编码）
- **HTML实时预览**: 编辑HTML时按`Ctrl Shift V`打开实时预览
- **PDF预览**: 直接预览PDF文件
- **HTTP客户端**: 发送HTTP请求（由于REST Client本地请求有bug，进行了修改集成）
- **注册表编辑器**: 支持Windows注册表文件
- **压缩文件查看器**: 提取并查看各种压缩格式的内容

## 配置选项

扩展在VS Code设置中提供各种配置选项：

- `mditor.enabled`: 启用/禁用扩展
- `mditor.previewCode`: 在预览中启用代码语法高亮
- `mditor.previewCodeStyle`: 默认语法高亮样式
- `mditor.previewCodeHighlight.showLineNumber`: 在代码块中显示行号
- `mditor.editorLanguage`: 编辑器语言偏好
- `mditor.workspacePathAsImageBasePath`: 使用工作区路径作为Markdown图片基础路径
- `mditor.pasterImgPath`: 图片粘贴路径模板
- `mditor.chromiumPath`: PDF导出的Chromium浏览器路径

## 系统要求

- Visual Studio Code ^1.64.0
- 某些功能需要网络连接（PDF渲染，字体预览）

## 安装方法

1. 从VS Code市场安装：搜索"Mditor"
2. 或通过VSIX安装：下载并安装.vsix文件
3. 安装后重新加载VS Code

## 使用方法

1. **Markdown**: 打开任何.md文件开始使用所见即所得编辑器编辑
2. **办公文件**: 打开.xlsx、.docx、.pdf文件进行预览
3. **HTML**: 打开.html文件并按`Ctrl Shift V`进行实时预览
4. **HTTP请求**: 创建.http文件发送API请求
5. **注册表文件**: 打开.reg文件获得语法高亮和导航功能

## 开发

```bash
# 安装依赖
npm install

# 构建扩展
npm run build

# 开发模式运行
npm run dev

# 打包发布
npm run package
```

## 赞助支持

如果你愿意支持本项目的开发，可以通过下面的二维码进行捐助（支付宝 / 微信）：

<p>
  <img src="images/alipay.jpg" alt="Alipay 捐助" style="width:200px;display:inline-block;margin-right:16px;" />
  <img src="images/wechatpay.jpg" alt="WeChat Pay 捐助" style="width:200px;display:inline-block;" />
</p>

## 致谢

- **PDF渲染**: [mozilla/pdf.js/](https://github.com/mozilla/pdf.js/)
- **DOCX渲染**: [VolodymyrBaydalka/docxjs](https://github.com/VolodymyrBaydalka/docxjs)
- **XLSX渲染**:
  - [SheetJS/sheetjs](https://github.com/SheetJS/sheetjs): XLSX解析
  - [myliang/x-spreadsheet](https://github.com/myliang/x-spreadsheet): XLSX渲染
- **HTTP客户端**: [Rest Client](https://github.com/Huachao/vscode-restclient)
- **Markdown编辑器**: [Vanessa219/vditor](https://github.com/Vanessa219/vditor)
- **图标主题**: [PKief/vscode-material-icon-theme](https://github.com/PKief/vscode-material-icon-theme)

## 许可证

本项目采用[LGPL-3.0-or-later许可证](LICENSE)。

## 问题反馈和支持

- **错误报告**: [GitHub Issues](https://github.com/dreamxwork/mditor-vs/issues)
- **邮件支持**: dreamxwork@outlook.com
- **项目仓库**: [GitHub Repository](https://github.com/dreamxwork/mditor-vs.git)

---

*最后更新: 2024年*
