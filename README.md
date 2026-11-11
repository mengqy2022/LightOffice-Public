<div align="center">

<img src="assets/brand/lightoffice-128.png" width="88" alt="轻舟六瓣花图标" />

# 轻舟 · LightOffice

**选中文件，展开你的轻量办公花屿。**

图片 · PDF · 截图识别与翻译 · 压缩 · CSV 数据科学

[![Release](https://img.shields.io/github/v/release/mengqy2022/LightOffice-Public?style=flat-square&color=508d7b)](https://github.com/mengqy2022/LightOffice-Public/releases/latest)
[![Windows](https://img.shields.io/badge/Windows-10%20%2F%2011-467a85?style=flat-square)](docs/usage.md)
[![Runtime](https://img.shields.io/badge/.NET_Framework-4.8-71856a?style=flat-square)](docs/faq.md)
[![Downloads](https://img.shields.io/github/downloads/mengqy2022/LightOffice-Public/total?style=flat-square&color=508d7b)](https://github.com/mengqy2022/LightOffice-Public/releases)

[**下载安装包**](https://github.com/mengqy2022/LightOffice-Public/releases/download/v0.6.0/LightOffice-0.6.0.0-Setup.exe) · [便携 ZIP](https://github.com/mengqy2022/LightOffice-Public/releases/download/v0.6.0/LightOffice-0.6.0.0-windows.zip) · [功能手册](docs/features.md) · [演示图库](screenshots/README.md) · [反馈问题](https://github.com/mengqy2022/LightOffice-Public/issues/new/choose)

<img src="screenshots/hero.png" width="1080" alt="轻舟 0.6：花屿、数据科学与截图内翻译，合成演示数据的真实界面" />

</div>

轻舟是常驻托盘的 Windows 文件工具。单击选中文件后，六瓣花屿提供相关操作；处理窗口可以独立移动、关闭和置顶，选另一个文件时继续保留当前工作。

基础包使用 C# / WPF，不需要浏览器运行时。LibreOffice、7-Zip、Bandizip、Python 和 R 均不包含在基础包中；有需要时再配置对应组件。文档和图片处理在本机执行，在线翻译由用户主动触发。

> 此仓库提供产品展示、用户文档、问题反馈和二进制发行。完整开发源码与测试工程不在本仓库发布。演示图使用合成文件，不含用户实际文件内容。

## 0.6 新变化

- **更完整的分类操作区**：常用项优先，补齐当前分类已实现的工具，最多九项；叶片按钮与花瓣的曲线和配色统一。
- **更直接的 F2 改名入口**：常驻进程收到 F2 时读取当前选择，跳过花屿显示的双击等待和缩略图加载。
- **保留 Windows 打开方式**：始终保留系统默认入口，读取系统推荐；自定义程序另外添加，明确设置后才作为轻舟内优先项。
- **数据流程与绘图**：保存 / 载入 JSON 流程，新增直方图和有限抽样散点图。
- **批量改名与恢复**：预览、冲突拒绝、记录校验、恢复，并同步文件花屿路径。
- **图片 / PDF 水印**：文字、位置、透明度和字号；带轻舟恢复标记的 PDF 水印可以另存移除。
- **按需高级解压**：配置 7-Zip 后处理普通 7z / RAR；加密、分卷和链接项明确拒绝。

[完整更新记录 →](docs/changelog.md)

## 一朵花，六类工作

| 分类 | 已实现的操作 | 演示 |
|---|---|---|
| 转换 | PNG / JPG / BMP 互转；DOCX / XLSX / PPTX 转 PDF（可选本机 Office 引擎） | [界面](screenshots/flower-format.png) |
| 图片 | 调整尺寸、裁剪 / 90°旋转、批处理、图片或 PDF 文字水印 | [界面](screenshots/flower-image.png) |
| PDF | 拆分、合并、检查 / 等比例统一 A4、添加水印、移除轻舟水印 | [界面](screenshots/flower-pdf.png) |
| 截图 | 框选 / 窗口 / 全屏、标注 / 打码、复制 / 保存、贴图、本地 OCR、GUI 内中英翻译 | [界面](screenshots/capture-translation.png) |
| 压缩 | ZIP 目录预览、安全解压、多源 ZIP；可选 7z 压缩及 7z / RAR 解压 | [界面](screenshots/flower-archive.png) |
| 效率 | 打开 / 推荐应用、定位 / 复制路径、单文件和批量改名、CSV / TSV 数据科学 | [界面](screenshots/flower-efficiency.png) |

功能手册逐项列出入口、输入、步骤、输出、限制与测试演示图：[查看全部 24 个工具和数据操作](docs/features.md)。

## 数据科学，先从轻量表格处理开始

<img src="screenshots/data-science.png" width="1000" alt="CSV 数据科学：预览、筛选、选列和处理参数" />

CSV / TSV 逐记录读取，有限预览后全文件执行，支持筛选、选列、列名调整、清理空白 / 空值、按键去重、多列分组汇总和同表头按行追加。流程可保存复用，输出为新文件。

汇总结果可画条形图与分类折线图；数值数据可画直方图和散点图。抽样图会标出有效行、空值、样本数和固定种子，避免把样本图当成全量统计。

| 汇总图 | 数值散点图 |
|---|---|
| ![分组汇总图](screenshots/data-chart.png) | ![固定种子抽样散点图](screenshots/data-scatter.png) |

当前不提供 XLSX 结构化编辑，也不承诺快速导入 500 MB–2 GB 的 Excel。需要文档转 PDF 时，可另外配置 LibreOffice 或 Microsoft Office。

## 截图到文字，再到翻译

<img src="screenshots/capture-translation.png" width="1000" alt="原文和中文译文直接显示在截图工作台内" />

默认 `Ctrl+Alt+S` 截图，截图内 `Ctrl+Shift+O` 识别、`Ctrl+Shift+T` 翻译；快捷键可配置并检查冲突。OCR 使用 Windows 本地语言能力，翻译点击后才向 MyMemory 发送文字，结果显示在软件内。

[快捷键与隐私说明 →](docs/usage.md#截图文字识别和翻译)

## 安装与更新

1. 在 [Releases](https://github.com/mengqy2022/LightOffice-Public/releases/latest) 下载 `LightOffice-0.6.0.0-Setup.exe` 或便携 ZIP，同时取得对应 `.sha256`。
2. 按[下载校验说明](releases/README.md)核对 SHA-256。安装器仅安装到当前用户目录，无需管理员权限；也可解压 ZIP 后运行 `LightOffice.exe`。
3. 从托盘设置紧凑尺寸、登录自启、置顶与可选组件。开始菜单 / 桌面快捷方式使用同一品牌图标。

需要 Windows 10 / 11 和系统 .NET Framework 4.8。基础包不含外部办公 / 压缩引擎；安装器没有控制面板卸载项，删除及更新目录处理见[使用说明](docs/usage.md)。

## 验证与功能边界

截图来自真实 WPF 窗口与合成文件，界面展示与实际导出验证分别记录。PDF 水印通过独立引擎比对文字、纸张、旋转及移除后的页面像素；7z / RAR 检查包含真实外部引擎。Windows 登录自启、休眠、多显示器 DPI 切换仍需对应实机环境验收，不能仅凭截图判定通过。

请阅读[功能边界与常见问题](docs/faq.md)和[验证说明](docs/validation.md)。

## 参与反馈

[报告问题](https://github.com/mengqy2022/LightOffice-Public/issues/new?template=bug_report.yml) · [提出建议](https://github.com/mengqy2022/LightOffice-Public/issues/new?template=feature_request.yml) · [后续路线](docs/roadmap.md)

提交时请附版本、Windows 版本、复现步骤和错误提示，并移除私人文件内容、账号与路径。文档和品牌许可见 [LICENSE](LICENSE)；第三方组件通知与许可证随发行包提供。
