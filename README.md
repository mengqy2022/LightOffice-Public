<div align="center">

<img src="assets/brand/lightoffice-128.png" width="88" alt="轻舟六瓣花图标" />

# 轻舟 · LightOffice

**选中文件，展开你的轻量办公花屿。**

图片 · PDF · 截图识别与翻译 · 压缩 · CSV 数据科学

**简体中文** · [English](README.en.md)

[![Release](https://img.shields.io/github/v/release/mengqy2022/LightOffice-Public?style=flat-square&color=508d7b)](https://github.com/mengqy2022/LightOffice-Public/releases/latest)
[![Windows](https://img.shields.io/badge/Windows-10%20%2F%2011-467a85?style=flat-square)](docs/usage.md)
[![Runtime](https://img.shields.io/badge/.NET_Framework-4.8-71856a?style=flat-square)](docs/faq.md)
[![Downloads](https://img.shields.io/github/downloads/mengqy2022/LightOffice-Public/total?style=flat-square&color=508d7b)](https://github.com/mengqy2022/LightOffice-Public/releases)

[**下载安装包**](https://github.com/mengqy2022/LightOffice-Public/releases/download/v0.7.4/LightOffice-0.7.4.0-Setup.exe) · [便携 ZIP](https://github.com/mengqy2022/LightOffice-Public/releases/download/v0.7.4/LightOffice-0.7.4.0-windows.zip) · [三分钟上手](docs/quickstart.md) · [操作教学](docs/getting-started.md) · [六个任务教程](docs/tutorials.md) · [全部功能导航](docs/catalog.md) · [演示图库](screenshots/README.md) · [许可说明](docs/licensing.md) · [反馈问题](https://github.com/mengqy2022/LightOffice-Public/issues/new/choose)

<img src="screenshots/hero.png" width="1080" alt="轻舟 0.6：花屿、数据科学与截图内翻译，合成演示数据的真实界面" />

</div>

轻舟是常驻托盘的 Windows 文件工具。单击选中文件后，六瓣花屿提供相关操作；处理窗口可以独立移动、关闭和置顶，选另一个文件时继续保留当前工作。

基础包使用 C# / WPF，不需要浏览器运行时。LibreOffice、7-Zip、Bandizip、Python 和 R 均不包含在基础包中；有需要时再配置对应组件。文档和图片处理在本机执行，在线翻译由用户主动触发。

> 此仓库提供产品展示、用户文档、问题反馈和二进制发行。完整开发源码与测试工程不在本仓库发布。演示图使用合成文件，不含用户实际文件内容。

README 提供简体中文与英文入口；**软件界面和安装向导目前为简体中文**，文档语言切换不改变软件语言。详细专题目前主要为中文。

## 功能导航与版本

**当前版本为 0.7.4.0。** 新增截图自由画笔、Enter 复制并完成、小屏高缩放布局补强、四步引导、真实 CSV 操作练习、可关闭的紧凑快捷键提示，以及重命名和设置保存成功后自动关闭；[本版操作教学与图示](docs/getting-started.md)。保留中文安装向导、自定义目录、独立卸载程序、经典 / 圆弧主题与工作台换色；[安装与卸载指南](docs/installation.md)。0.6 图片保留为历史功能基线。

| 想做什么 | 图文教程 |
|---|---|
| 第一次使用，完成一次另存 | [三分钟上手](docs/quickstart.md) |
| 跟着实际任务做，看输入与结果 | [六个任务、前后对比与步骤动图](docs/tutorials.md) |
| 查全部工具及工作台内部操作 | [全功能导航](docs/catalog.md) · [24 个工具手册](docs/features.md) |
| 清理数据、筛选和分组、流程复用、绘图 | [数据科学专题](docs/data-science.md) |
| 截图、标注、识别、软件内翻译和贴图 | [截图专题](docs/capture.md) |
| 主题、大小、多开、置顶、打开方式和改名 | [桌面与文件整理](docs/desktop.md) |
| 图片、PDF、文档转换、压缩和可选引擎 | [组件与文件处理](docs/components.md) |
| 下载数据自己试验，并核对真实输出 | [五分钟示例](examples/README.md) |
| 直接浏览所有功能图片 | [分类图片墙](screenshots/README.md) |
| 启动、F2、OCR、翻译或引擎出问题 | [故障排查](docs/troubleshooting.md) |
| 了解版本、升级、资源与数据去向 | [版本对照](docs/versions.md) · [测量与轻量边界](docs/performance.md) · [文件与网络说明](docs/privacy.md) |

## 从输入到结果，照着完成一次任务

混合纸张的 PDF 等比统一 A4，原图批量缩小后加水印，CSV 清理后汇总绘图，以及截图翻译、改名恢复、打开方式设置，均有[逐步教程](docs/tutorials.md)。下载合成输入，核对实际结果，先用样例熟悉操作。

| PDF 纸张处理前后 | 图片缩小与水印前后 |
|---|---|
| ![PDF纵向页面等比转A4](assets/demos/pdf-a4-before-after.png) | ![图片实际缩小和水印结果](assets/demos/image-before-after.png) |

PDF 与图片结果由 0.7.2实际处理；图示纸张不是扫描件，验证的是页面尺寸与比例。旧版有相同基础工具，0.7 新增界面和版本差异另有标注。

<img src="assets/demos/data-steps.gif" width="1000" alt="清理、组合筛选、重新打开源文件后汇总绘图的步骤图轮播，非操作录像" />

动图由真实界面的步骤图片组成，使用合成数据，**不是操作录像**。另有[截图识别翻译与主题轮播](docs/tutorials.md)，文字步骤可静态阅读。

## 24 个工具，六类入口

| 分类 | 全部工具 |
|---|---|
| 转换 | [图片格式转换](docs/features.md#image-convert) · [办公文档转 PDF](docs/features.md#document-convert) |
| 图片 | [调整尺寸](docs/features.md#resize) · [裁剪与旋转](docs/features.md#crop) · [图片批处理](docs/features.md#image-batch) · [图片 / PDF 水印](docs/features.md#watermark) |
| PDF | [拆分](docs/features.md#pdf-split) · [合并](docs/features.md#pdf-merge) · [统一 A4](docs/features.md#pdf-a4) · [添加水印](docs/features.md#pdf-watermark) · [移除已添加水印](docs/features.md#pdf-remove-watermark) |
| 截图 | [截图与识别翻译](docs/features.md#capture) · [桌面贴图](docs/features.md#pin-image) |
| 压缩 | [压缩文件](docs/features.md#compress) · [解压文件](docs/features.md#extract) · [预览 ZIP](docs/features.md#zip-preview) |
| 效率 | [打开文件](docs/features.md#open) · [常用打开方式](docs/features.md#open-with) · [定位文件](docs/features.md#locate) · [复制路径](docs/features.md#copy-path) · [重命名文件](docs/features.md#rename) · [批量重命名](docs/features.md#rename-batch) · [预览文本](docs/features.md#text-preview) · [数据科学](docs/features.md#data-science) |

每个入口都有输入、步骤、输出、边界和对应图片。工作台子操作和桌面设置在[全功能导航](docs/catalog.md)继续展开，不再只列按钮名称。

## 数据科学：看见条件，也看见结果

下图为 0.7.2界面，数据能力在 0.6 已提供。实际组合条件“地区等于华东，金额 ≥ 100”，预览只保留 A001。完整专题包含 16 种条件、AND / OR、列名、类型、清理、去重、五种汇总、追加和流程复用。

<img src="screenshots/data-combined-filters-0.7.2.png" width="1000" alt="真实组合筛选与单条匹配结果" />

| 类型、列名、去重与清理 | 全文件分组结果 |
|---|---|
| ![清理预览](screenshots/data-types-cleaning-0.7.2.png) | ![全量分组](screenshots/data-grouping-result-0.7.2.png) |

下载 [sales.csv](examples/sales.csv) 和[可复用流程](examples/east-over-100.json)，按[五分钟教程](examples/README.md)操作；实际导出的[清理结果](examples/cleaned.csv)和[地区汇总](examples/region-totals.csv)可直接核对。

当前不提供 XLSX 结构化编辑，也不承诺快速导入 500 MB–2 GB Excel。[数据科学完整图文 →](docs/data-science.md)

## 四种图表，直接另存 PNG

| 条形图 | 分类折线图 |
|---|---|
| ![条形图](screenshots/data-chart.png) | ![分类折线](screenshots/data-line-chart-0.7.2.png) |

| 直方图 | 散点图 |
|---|---|
| ![直方图](screenshots/data-histogram.png) | ![散点图](screenshots/data-scatter.png) |

汇总图区分样本与全量，包含完整标签和精确值表；数值图是固定种子的有限抽样，标明扫描、有效、空值及样本数量。全部用 C# 绘制，无需 R / Python。[图形规则与真实输出 →](docs/data-science.md#四种绘图不安装额外环境)

## 截图 → 标注 → OCR → GUI 内翻译

<img src="screenshots/capture-translation.png" width="1000" alt="原文和中文译文直接显示在截图工作台内" />

默认 `Ctrl+Alt+S` 截图，截图内 `Ctrl+Shift+O` 识别、`Ctrl+Shift+T` 翻译；快捷键可配置并检查冲突。OCR 使用 Windows 本地语言能力，翻译点击后才向 MyMemory 发送文字，结果显示在软件内。

<img src="screenshots/capture-annotation-options-0.7.2.png" width="1000" alt="0.7.2候选：箭头、色板、线宽和识别翻译工具栏" />

框选、窗口、全屏，自由画笔 / 矩形 / 箭头 / 文字 / 打码、六色色板与 2 / 3 / 6 px 线宽、手柄、整笔撤销和键盘微调。**Enter 复制包含标注的截图并关闭，到聊天框或 APP 按 Ctrl+V 即可粘贴，不必保存文件；Ctrl+S 另存 PNG。** 输入文字与选择语言时保留 Enter 原用途；复制失败保留编辑。结果也可保存并贴图或直接贴图；贴图支持移动、缩放与另存。0.7 系列增加 [LibreTranslate 服务配置](screenshots/translation-service-0.7.2.png)。

| 经典主题画笔 | 圆弧主题画笔 |
|---|---|
| ![经典主题画笔与 Enter 复制](screenshots/capture-pen-classic-0.7.4.png) | ![圆弧主题画笔与 Enter 复制](screenshots/capture-pen-circular-0.7.4.png) |

两图来自当前真实控件的离屏渲染，使用合成内容。画笔在「框选」右侧，按住鼠标绘制；Ctrl+Z 整笔撤销，绘制中 Esc 取消本笔。

[完整操作、快捷键与隐私 →](docs/capture.md)

## 图片、PDF、压缩和文件整理

| 图片批处理 | PDF 等比例 A4 |
|---|---|
| ![图片批处理](screenshots/image-batch.png) | ![PDF检查与A4](screenshots/pdf-a4.png) |

| 多源压缩与增强选项 | 批量改名规则与恢复入口 |
|---|---|
| ![压缩](screenshots/archive-compress.png) | ![改名](screenshots/rename-rules-0.7.2.png) |

尺寸、格式、质量、裁剪、水印、拆分、合并、解压、预览、打开方式、组件配置及各操作入口，在[分类图片墙](screenshots/README.md)全部内嵌展示。PDF 去水印仅支持轻舟恢复标记，不自动删除任意扫描水印。

## 经典与圆弧，两种风格保留

以下功能已随 0.7.2 正式发布。默认经典，圆弧可选；0.7.2 功能窗口、输入框、表格和工具栏即时同步，切换时保留参数与数据。

| 经典花屿 | 圆弧花屿 |
|---|---|
| ![经典](screenshots/theme-classic-0.7.1.png) | ![圆弧](screenshots/theme-circular-0.7.1.png) |

<img src="screenshots/capture-toolbar-dark-0.7.2.png" width="1000" alt="圆弧主题下的截图工具栏" />

三档尺寸、保持紧凑、收起小花心、多开、工作台置顶、登录自启、暂停自动展开和目录排除分别可设置。0.7.4 按工作区与 DPI 限制窗口，低于设计最小尺寸时提供滚动，移回大屏恢复布局；截图工具栏换行并可滚动。[桌面功能说明 →](docs/desktop.md) · [候选变化 →](docs/preview-0.7.md)

## 安装与更新

1. 在 [Releases](https://github.com/mengqy2022/LightOffice-Public/releases/latest) 下载 `LightOffice-0.7.4.0-Setup.exe` 或便携 ZIP，同时取得对应 `.sha256`。
2. 按[下载校验说明](releases/README.md)核对 SHA-256。安装器仅安装到当前用户目录，无需管理员权限；也可解压 ZIP 后运行 `LightOffice.exe`。
3. 从托盘设置紧凑尺寸、登录自启、置顶与可选组件。开始菜单 / 桌面快捷方式使用同一品牌图标。

需要 Windows 10 / 11 和系统 .NET Framework 4.8。基础包不含外部办公 / 压缩引擎；0.6 正式版需手动移除；0.7 系列已有标准卸载及版本回退，差异见[组件和安装说明](docs/components.md#安装与卸载的版本差异)。

## 验证与功能边界

截图来自真实 WPF 窗口与合成文件，界面展示与实际导出验证分别记录。PDF 水印通过独立引擎比对文字、纸张、旋转及移除后的页面像素；7z / RAR 检查包含真实外部引擎。当前保护构建通过 165 项画笔 / Enter / 小屏专项，剪贴板使用隔离接口，未改动用户剪贴板。此前候选完成真实双屏 DPI、Windows 缩放设置、桌面截图及 112 项人工窗口操作；短时 S0 进退有系统记录。2026-11-12 用户已实测确认画笔绘制、整笔撤销及 Enter 复制后聊天框 Ctrl+V 粘贴正常；此确认仅覆盖实际使用环境。真实登录、长期待机 / 休眠和干净系统组合仍需验收。

当前安装包采用同一正式 ZIP 制作隔离测试，38 项真实安装 / 卸载通过，89 项程序 / 文档载荷逐文件哈希匹配。程序与安装器目前未做代码签名，下载后请核对 `.sha256`。

请阅读[功能边界与常见问题](docs/faq.md)、[验证说明](docs/validation.md)和[已有测量](docs/performance.md)。历史启动 / 内存数据标明构建与条件，不作为所有机器或新版的性能保证。

## 参与反馈

**开发者：Mengqy · 开发平台：Codex · 软件：轻舟 / LightOffice。** 当前公开正式版本见页面顶部；软件内「关于轻舟」显示实际运行版本。

[轻舟博客与许可说明](https://www.mqymmb.com/posts/lightoffice/#license-note) · [博客文章评论反馈](https://www.mqymmb.com/posts/lightoffice/#license-note) · 邮箱：**15877464851@163.com**。可在文章评论区留言，或自行发邮件；请附版本、复现步骤和错误文字。

[报告问题](https://github.com/mengqy2022/LightOffice-Public/issues/new?template=bug_report.yml) · [提出建议](https://github.com/mengqy2022/LightOffice-Public/issues/new?template=feature_request.yml) · [后续路线](docs/roadmap.md)

提交前可先查[故障排查](docs/troubleshooting.md)。请附版本、Windows 版本、复现步骤和错误提示，并移除私人文件内容、账号与路径，参阅[文件与网络说明](docs/privacy.md)。自有程序和新材料采用[专有许可](docs/licensing.md)，保留[先前 MIT 授权](LICENSE-LEGACY-MIT.txt)，完整条款见 [LICENSE](LICENSE)；第三方组件通知与许可证随发行包提供。
