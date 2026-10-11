# 本地文件格式转换器 · Local File Converter

一个单文件 HTML 的浏览器端文件格式转换工具。**所有转换都在你的浏览器本地完成，文件不会上传到任何服务器**；网络只用于首次从 CDN 加载第三方库。

A single-file, in-browser file converter. **All conversions run locally in your browser — files are never uploaded.** The network is only used to load libraries from a CDN the first time.

**在线使用 / Use online:** https://greatgoldaxe.github.io/local-file-converter/

## 使用 / Usage

- 打开上面的链接，或下载 `index.html` 后双击用浏览器打开。
- 左侧选择功能 → 拖拽 / 点击 / 粘贴添加文件 → 选择输出格式 → 开始转换 → 在右侧下载或打包 ZIP。
- 推荐最新版 Chrome / Edge / Firefox。

Open the link above, or download `index.html` and double-click it. Pick a feature, add files (drag, click or paste), choose the output, convert, then download or ZIP the results.

## 功能 / Features

| 类别 | 功能 |
|---|---|
| PDF | 合并、拆分、提取/删除/旋转页面、转图片、提取文本、转 Word、图片转 PDF |
| Word / 文档 | DOCX → HTML / Markdown / TXT / PDF；TXT / Markdown / HTML 互转并可生成 DOCX、PDF |
| Excel / CSV | XLSX / XLS / ODS / CSV / TSV / JSON / HTML / Markdown 互转，多工作表、GBK 编码、长数字保护、日期格式；转 PDF |
| 图片 | JPG / PNG / WebP / AVIF / GIF / BMP / ICO / TIFF / HEIC / SVG / PSD 互转，压缩、调整尺寸、旋转、透明背景处理 |
| OCR | 图片 / 扫描 PDF → TXT / Word（Tesseract.js，中英文等） |
| 数据 / 编码 | JSON / XML / YAML / CSV / Excel 互转，格式化与校验，文本编码转换（GBK / UTF-8 / Big5…），Base64 |
| 电子书 | EPUB → TXT / HTML / Markdown / Word / PDF；TXT / Markdown / HTML → EPUB |
| 音视频 | 基于 ffmpeg.wasm 的视频格式转换、提取音频、转 GIF、剪切；无需 ffmpeg 的轻量音频转 WAV / MP3 |
| PPT | PPTX → PDF / 图片 / 文本；图片 / PDF → PPTX |
| 其它 | ZIP 解压与打包；iWork / Sketch 预览提取；AI → PDF / PNG |

每个功能都在页面中标注了支持程度（完全可用 / 部分可用 / 仅提取文本 / 需后端 / 不支持）和限制说明。无法在浏览器中实现的格式（DOC、PPT 旧格式、RAR/7z、DWG、Figma 等）会给出推荐的外部工具。

## 注意 / Notes

- Word / Excel / EPUB 转出的 PDF 为图像页面（支持中文，但文字不可选中）。
- OCR 首次使用需下载语言包（中文约 20MB），音视频引擎约 31MB，之后浏览器会缓存。
- 浏览器内存有限，超大文件（尤其视频 > 500MB）建议使用桌面软件。
- 若依赖库加载失败，可在“设置”中切换 CDN 源（国内可选 npmmirror）。

## 第三方库 / Libraries

pdf-lib · pdf.js · jsPDF · html2canvas · mammoth · SheetJS · PapaParse · JSZip · js-yaml · marked · turndown · Tesseract.js · heic2any · PptxGenJS · UTIF.js · pako · lamejs · ffmpeg.wasm
