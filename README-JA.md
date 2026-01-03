# Mditor

[English](README.md) | [简体中文](README-CN.md) | [繁體中文](README-TW.md) | [日本語](README-JA.md) | [한국어](README-KO.md) | [Français](README-FR.md) | [Deutsch](README-DE.md) | [Español](README-ES.md) | [Русский](README-RU.md)

WYSIWYG 機能と包括的なファイルプレビューサポートにより、Markdown 編集体験を変革する強力でエレガントな VS Code 拡張機能です。

## ✨ ハイライト

Mditor は Visual Studio Code にプロフェッショナルグレードの編集とプレビュー機能を提供します：

- 🎨 **美しい WYSIWYG Markdown エディター** - リアルタイムプレビューとリッチフォーマット
- 📊 **マルチフォーマットファイルビューアー** - Office ドキュメント、PDF などのプレビュー
- 🌓 **複数のテーマサポート** - 快適な編集のための豪華なライト/ダークテーマ
- ⚡ **超高速** - 大きなドキュメント向けに最適化されたパフォーマンス
- 🎯 **開発者フレンドリー** - 豊富なキーボードショートカットと直感的なインターフェース

## 📸 スクリーンショット

### ライトテーマ
![ライトテーマ](images/light.png)

### ダークテーマ
![ダークテーマ](images/dark.png)

## 🚀 機能

### 優れた Markdown エディター

[Vditor](https://github.com/Vanessa219/vditor) をベースに構築された WYSIWYG エディターは以下を提供します：

- **リアルタイムプレビュー** - 入力するとフォーマットされたコンテンツが表示されます
- **リッチフォーマット** - テーブル、コードブロック、図表（Mermaid）、数式（LaTeX）をサポート
- **スマート貼り付け** - 自動画像アップロードとパス解決
- **どこでもエクスポート** - ワンクリックで PDF、DOCX、HTML に変換
- **豊富なテーマ** - スタイルに合わせた美しいエディターテーマ

#### 強力なキーボードショートカット

[Vditor ショートカット](shortcut.md)をベースに、生産性機能を強化：

- **リストを上に移動**: `Ctrl+Alt+I` / `⌘+^+I`
- **リストを下に移動**: `Ctrl+Alt+J` / `⌘+^+J`
- **VS Code で編集**: `Ctrl+Alt+E` / `⌘+^+E`
- **拡張貼り付け**: `Ctrl+V` / `Cmd+V` 自動画像処理付き

#### スマート機能

- `Ctrl/Cmd + マウスホイール` でエディターをズーム
- `Ctrl/Meta + クリック` またはダブルクリックでハイパーリンクを開く
- ドラッグ＆ドロップで画像挿入
- 自動画像パス解決
- 複数のテーマオプションによるシンタックスハイライト

### 包括的なファイルプレビュー

VS Code で一般的なファイル形式を直接プレビュー：

- 📊 **スプレッドシート**: .xls, .xlsx, .csv（編集と保存が可能）
- 📝 **ドキュメント**: .docx
- 🖼️ **グラフィックス**: .svg
- 📄 **PDF**: .pdf（PDF.js で動作）
- 🔤 **フォント**: .ttf, .otf, .woff, .woff2
- 📋 **Markdown**: .md, .markdown
- 🌐 **HTTP**: .http, .rest（統合 HTTP クライアント）
- ⚙️ **レジストリ**: .reg（Windows レジストリファイル）
- 📦 **アーカイブ**: .zip, .jar, .vsix, .rar

### 追加機能

- **Material アイコン** - Material Icon Theme の美しいファイルアイコン
- **HTML ライブプレビュー** - `Ctrl+Shift+V` で HTML を即座にプレビュー
- **HTTP クライアント** - .http ファイルから直接 API リクエストを送信
- **レジストリエディター** - Windows レジストリファイルのシンタックスハイライト

## 🔧 設定

VS Code の設定で Mditor を微調整：

| 設定 | 説明 |
|------|------|
| `mditor.enabled` | 拡張機能を有効/無効にする |
| `mditor.previewCode` | プレビューでコードのシンタックスハイライトを有効にする |
| `mditor.previewCodeStyle` | デフォルトのシンタックスハイライトスタイル |
| `mditor.previewCodeHighlight.showLineNumber` | コードブロックに行番号を表示 |
| `mditor.editorLanguage` | エディター UI 言語 |
| `mditor.workspacePathAsImageBasePath` | ワークスペースパスを画像ベースパスとして使用 |
| `mditor.pasterImgPath` | 画像貼り付けパステンプレート |
| `mditor.chromiumPath` | PDF エクスポート用の Chromium パス |

### ネイティブ Markdown エディターへの切り替え

VS Code のデフォルト markdown エディターを使用するには、`settings.json` に追加：

```json
{
    "workbench.editorAssociations": {
        "*.md": "default",
        "*.markdown": "default"
    }
}
```

## 📋 必要条件

- Visual Studio Code `^1.64.0`
- インターネット接続（一部のプレビュー機能に必要）

## 📥 インストール

### マーケットプレイスからインストール
1. VS Code を開く
2. 拡張機能に移動（`Ctrl+Shift+X`）
3. "Mditor" を検索
4. インストールをクリック

### VSIX からインストール
1. 最新の .vsix ファイルをダウンロード
2. VS Code を開く
3. 拡張機能 → `...` → VSIX からインストール
4. ダウンロードしたファイルを選択

## 🎯 クイックスタート

1. **Markdown 編集**: 任意の `.md` ファイルを開く - WYSIWYG エディターが自動起動
2. **Office プレビュー**: `.xlsx`、`.docx`、`.pdf` ファイルをクリックしてプレビュー
3. **HTML プレビュー**: `.html` ファイルを開いて `Ctrl+Shift+V` を押す
4. **HTTP リクエスト**: `.http` ファイルを作成して API をテスト
5. **アーカイブ表示**: `.zip` やその他のアーカイブを開いて内容を閲覧

## 📖 Markdown サンプル

Mditor で何ができるか見てみたいですか？サポートされているすべての機能を紹介する包括的な Markdown サンプルファイルをご覧ください：

**[markdown-examples.md をダウンロード](https://raw.githubusercontent.com/dreamxwork/mditor-vs/main/markdown-examples.md)**

このサンプルファイルには以下が含まれます：
- 基本的なテキストフォーマット（見出し、太字、斜体、リスト）
- シンタックスハイライト付きコードブロック（C++、Java、Python、Shell、CMake、ログファイル）
- Mermaid 図表（フローチャート、シーケンス図、クラス図、ガントチャート、Git ブランチ図）
- 数式（LaTeX）
- 表とデータ可視化
- 楽譜記譜（ABC 記譜法）
- Graphviz 図表
- ECharts データ可視化
- その他多数の機能！

## 🛠️ 開発

```bash
# 依存関係をインストール
npm install

# 拡張機能をビルド
npm run build

# 開発モード（ホットリロード）
npm run dev

# 配布用にパッケージ化
npm run package
```

## 💖 このプロジェクトをサポート

Mditor が役に立つと思われた場合は、開発をサポートしてください：

### 国際寄付
[![PayPal](https://img.shields.io/badge/PayPal-Donate-blue.svg?logo=paypal)](https://www.paypal.me/howpigcanfly)

**PayPal アカウント**: howpigcanfly@outlook.com

### 中国本土での寄付
<p>
  <img src="images/alipay.jpg" alt="Alipay 寄付" width="200" style="display:inline-block;margin-right:16px;" />
  <img src="images/wechatpay.jpg" alt="WeChat Pay 寄付" width="200" style="display:inline-block;" />
</p>

**Alipay / WeChat Pay**: 上記の QR コードをスキャン

### 銀行振込
銀行振込での寄付については、こちらまでご連絡ください：dreamxwork@outlook.com

---

ご寄付はこのプロジェクトの維持と改善に役立ちます。ご支援ありがとうございます！

## 🙏 クレジット

このプロジェクトは以下の優れたオープンソースプロジェクトの上に構築されています：

- **PDF レンダリング**: [mozilla/pdf.js](https://github.com/mozilla/pdf.js/)
- **DOCX レンダリング**: [VolodymyrBaydalka/docxjs](https://github.com/VolodymyrBaydalka/docxjs)
- **XLSX 処理**:
  - [SheetJS/sheetjs](https://github.com/SheetJS/sheetjs) - Excel 解析
  - [myliang/x-spreadsheet](https://github.com/myliang/x-spreadsheet) - スプレッドシート UI
- **HTTP クライアント**: [Rest Client](https://github.com/Huachao/vscode-restclient)
- **Markdown エンジン**: [Vanessa219/vditor](https://github.com/Vanessa219/vditor)
- **アイコンテーマ**: [PKief/vscode-material-icon-theme](https://github.com/PKief/vscode-material-icon-theme)

## 📜 ライセンス

このプロジェクトは [LGPL-3.0-or-later ライセンス](LICENSE)の下でライセンスされています。

## 📞 連絡先とサポート

- **リポジトリ**: [https://github.com/dreamxwork/mditor-vs](https://github.com/dreamxwork/mditor-vs)
- **問題報告**: [GitHub Issues](https://github.com/dreamxwork/mditor-vs/issues)
- **メール**: dreamxwork@outlook.com

---

❤️ を込めて作成 by Mditor チーム | *最終更新：2026年*
