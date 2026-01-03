# Mditor

[English](README.md) | [简体中文](README-CN.md) | [繁體中文](README-TW.md) | [日本語](README-JA.md) | [한국어](README-KO.md) | [Français](README-FR.md) | [Deutsch](README-DE.md) | [Español](README-ES.md) | [Русский](README-RU.md)

WYSIWYG 기능과 포괄적인 파일 미리보기 지원으로 Markdown 편집 경험을 혁신하는 강력하고 우아한 VS Code 확장 프로그램입니다.

## ✨ 주요 특징

Mditor는 Visual Studio Code에 전문가급 편집 및 미리보기 기능을 제공합니다:

- 🎨 **아름다운 WYSIWYG Markdown 편집기** - 실시간 미리보기와 풍부한 서식
- 📊 **다중 형식 파일 뷰어** - Office 문서, PDF 등 미리보기
- 🌓 **다중 테마 지원** - 편안한 편집을 위한 화려한 라이트/다크 테마
- ⚡ **초고속** - 대용량 문서에 최적화된 성능
- 🎯 **개발자 친화적** - 풍부한 키보드 단축키와 직관적인 인터페이스

## 📸 스크린샷

### 라이트 테마
![라이트 테마](images/light.png)

### 다크 테마
![다크 테마](images/dark.png)

## 🚀 기능

### 뛰어난 Markdown 편집기

[Vditor](https://github.com/Vanessa219/vditor)를 기반으로 구축된 WYSIWYG 편집기는 다음을 제공합니다:

- **실시간 미리보기** - 입력하는 대로 서식이 적용된 콘텐츠 확인
- **풍부한 서식** - 표, 코드 블록, 다이어그램(Mermaid), 수식(LaTeX) 지원
- **스마트 붙여넣기** - 자동 이미지 업로드 및 경로 해석
- **어디서나 내보내기** - 원클릭으로 PDF, DOCX, HTML로 변환
- **다양한 테마** - 스타일에 맞는 여러 아름다운 편집기 테마

#### 강력한 키보드 단축키

[Vditor 단축키](shortcut.md)를 기반으로 생산성 기능 강화:

- **목록 위로 이동**: `Ctrl+Alt+I` / `⌘+^+I`
- **목록 아래로 이동**: `Ctrl+Alt+J` / `⌘+^+J`
- **VS Code에서 편집**: `Ctrl+Alt+E` / `⌘+^+E`
- **향상된 붙여넣기**: `Ctrl+V` / `Cmd+V` 자동 이미지 처리

#### 스마트 기능

- `Ctrl/Cmd + 마우스 휠`로 편집기 확대/축소
- `Ctrl/Meta + 클릭` 또는 더블클릭으로 하이퍼링크 열기
- 드래그 앤 드롭으로 이미지 삽입
- 자동 이미지 경로 해석
- 여러 테마 옵션의 구문 강조

### 포괄적인 파일 미리보기

VS Code에서 일반적인 파일 형식을 직접 미리보기:

- 📊 **스프레드시트**: .xls, .xlsx, .csv (편집 및 저장 가능)
- 📝 **문서**: .docx
- 🖼️ **그래픽**: .svg
- 📄 **PDF**: .pdf (PDF.js 기반)
- 🔤 **폰트**: .ttf, .otf, .woff, .woff2
- 📋 **Markdown**: .md, .markdown
- 🌐 **HTTP**: .http, .rest (통합 HTTP 클라이언트)
- ⚙️ **레지스트리**: .reg (Windows 레지스트리 파일)
- 📦 **아카이브**: .zip, .jar, .vsix, .rar

### 추가 기능

- **Material 아이콘** - Material Icon Theme의 아름다운 파일 아이콘
- **HTML 라이브 미리보기** - `Ctrl+Shift+V`로 HTML 즉시 미리보기
- **HTTP 클라이언트** - .http 파일에서 직접 API 요청 전송
- **레지스트리 편집기** - Windows 레지스트리 파일의 구문 강조

## 🔧 설정

VS Code 설정에서 Mditor 미세 조정:

| 설정 | 설명 |
|------|------|
| `mditor.enabled` | 확장 프로그램 활성화/비활성화 |
| `mditor.previewCode` | 미리보기에서 코드 구문 강조 활성화 |
| `mditor.previewCodeStyle` | 기본 구문 강조 스타일 |
| `mditor.previewCodeHighlight.showLineNumber` | 코드 블록에 줄 번호 표시 |
| `mditor.editorLanguage` | 편집기 UI 언어 |
| `mditor.workspacePathAsImageBasePath` | 작업 공간 경로를 이미지 기본 경로로 사용 |
| `mditor.pasterImgPath` | 이미지 붙여넣기 경로 템플릿 |
| `mditor.chromiumPath` | PDF 내보내기용 Chromium 경로 |

### 네이티브 Markdown 편집기로 전환

VS Code의 기본 markdown 편집기를 사용하려면 `settings.json`에 추가:

```json
{
    "workbench.editorAssociations": {
        "*.md": "default",
        "*.markdown": "default"
    }
}
```

## 📋 요구 사항

- Visual Studio Code `^1.64.0`
- 인터넷 연결 (일부 미리보기 기능에 필요)

## 📥 설치

### 마켓플레이스에서 설치
1. VS Code 열기
2. 확장 프로그램으로 이동 (`Ctrl+Shift+X`)
3. "Mditor" 검색
4. 설치 클릭

### VSIX에서 설치
1. 최신 .vsix 파일 다운로드
2. VS Code 열기
3. 확장 프로그램 → `...` → VSIX에서 설치
4. 다운로드한 파일 선택

## 🎯 빠른 시작

1. **Markdown 편집**: 아무 `.md` 파일 열기 - WYSIWYG 편집기가 자동 실행
2. **Office 미리보기**: `.xlsx`, `.docx`, `.pdf` 파일 클릭하여 미리보기
3. **HTML 미리보기**: `.html` 파일 열고 `Ctrl+Shift+V` 누르기
4. **HTTP 요청**: `.http` 파일 생성하여 API 테스트
5. **아카이브 보기**: `.zip` 또는 기타 아카이브 열어 내용 탐색

## 📖 Markdown 예제

Mditor로 무엇을 할 수 있는지 보고 싶으신가요? 지원되는 모든 기능을 보여주는 포괄적인 Markdown 예제 파일을 확인하세요:

**[markdown-examples.md 다운로드](https://raw.githubusercontent.com/dreamxwork/mditor-vs/main/markdown-examples.md)**

이 예제 파일에는 다음이 포함됩니다:
- 기본 텍스트 서식 (제목, 굵게, 기울임, 목록)
- 구문 강조가 있는 코드 블록 (C++, Java, Python, Shell, CMake, 로그 파일)
- Mermaid 다이어그램 (순서도, 시퀀스 다이어그램, 클래스 다이어그램, 간트 차트, Git 브랜치 그래프)
- 수학 공식 (LaTeX)
- 표 및 데이터 시각화
- 악보 표기법 (ABC 표기법)
- Graphviz 다이어그램
- ECharts 데이터 시각화
- 그 외 더 많은 기능!

## 🛠️ 개발

```bash
# 종속성 설치
npm install

# 확장 프로그램 빌드
npm run build

# 개발 모드 (핫 리로드)
npm run dev

# 배포용 패키징
npm run package
```

## 💖 이 프로젝트 지원하기

Mditor가 도움이 되었다면 개발을 지원해 주세요:

### 국제 기부
[![PayPal](https://img.shields.io/badge/PayPal-Donate-blue.svg?logo=paypal)](https://www.paypal.me/howpigcanfly)

**PayPal 계정**: howpigcanfly@outlook.com

### 중국 본토 기부
<p>
  <img src="images/alipay.jpg" alt="Alipay 기부" width="200" style="display:inline-block;margin-right:16px;" />
  <img src="images/wechatpay.jpg" alt="WeChat Pay 기부" width="200" style="display:inline-block;" />
</p>

**Alipay / WeChat Pay**: 위 QR 코드 스캔

### 은행 송금
은행 송금 기부는 다음으로 문의하세요: dreamxwork@outlook.com

---

여러분의 기부는 이 프로젝트를 유지하고 개선하는 데 도움이 됩니다. 지원해 주셔서 감사합니다!

## 🙏 크레딧

이 프로젝트는 다음의 훌륭한 오픈소스 프로젝트를 기반으로 구축되었습니다:

- **PDF 렌더링**: [mozilla/pdf.js](https://github.com/mozilla/pdf.js/)
- **DOCX 렌더링**: [VolodymyrBaydalka/docxjs](https://github.com/VolodymyrBaydalka/docxjs)
- **XLSX 처리**:
  - [SheetJS/sheetjs](https://github.com/SheetJS/sheetjs) - Excel 파싱
  - [myliang/x-spreadsheet](https://github.com/myliang/x-spreadsheet) - 스프레드시트 UI
- **HTTP 클라이언트**: [Rest Client](https://github.com/Huachao/vscode-restclient)
- **Markdown 엔진**: [Vanessa219/vditor](https://github.com/Vanessa219/vditor)
- **아이콘 테마**: [PKief/vscode-material-icon-theme](https://github.com/PKief/vscode-material-icon-theme)

## 📜 라이선스

이 프로젝트는 [LGPL-3.0-or-later 라이선스](LICENSE)에 따라 라이선스가 부여됩니다.

## 📞 연락처 및 지원

- **저장소**: [https://github.com/dreamxwork/mditor-vs](https://github.com/dreamxwork/mditor-vs)
- **이슈**: [GitHub Issues](https://github.com/dreamxwork/mditor-vs/issues)
- **이메일**: dreamxwork@outlook.com

---

❤️로 제작, Mditor 팀 | *최종 업데이트: 2026년*
