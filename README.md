# 轻舟

轻量级 Windows 文件快捷工具。轻舟围绕当前选中的文件提供图片、PDF、压缩包、文档和数据处理工作台。

## 下载

请从本仓库的 [GitHub Releases](https://github.com/mengqy2022/LightOffice-Public/releases) 下载最新的 `LightOffice-*-windows.zip`，并核对同名 `.sha256` 文件。解压后运行 `LightOffice.exe`。运行需要 Windows 和 .NET Framework 4.8；LibreOffice 等可选组件不会包含在基础安装包中。

尚未发布 GitHub Release 时，此处不会提供可用下载链接。

## 主要功能

- 图片尺寸调整、格式转换、裁剪、旋转与批量处理。
- PDF 拆分、合并和按比例适配 A4 页面。
- ZIP 压缩与解压；可选外部压缩引擎需单独安装或导入。
- DOCX、XLSX、PPTX 转 PDF；转换后端取决于本机安装并配置的 Office 软件。
- CSV/TSV 数据筛选、汇总、合并与绘图。
- 屏幕截图、标注和桌面置顶贴图。
- Windows 本地中英文文字识别；可编辑、复制并主动打开网页翻译。

![截图文字识别工具栏](screenshots/capture-ocr.png)

参阅 [使用说明](docs/usage.md) 和 [发行版下载说明](releases/README.md)。桌面设置支持当前用户登录自启、保持紧凑花屿及三档尺寸。

功能依赖、格式限制和隐私说明以每个 Release 随附的用户文档为准。程序不会自动上传用户文件。

## 问题反馈

请在 GitHub Issues 描述 Windows 版本、软件版本、复现步骤和错误提示。提交前请移除文件名、路径及文件内容等个人信息。

## 许可

本仓库提供的品牌和说明文件采用 MIT License，详见 [LICENSE](LICENSE)。第三方组件许可随对应发行包提供。
