# 全功能导航：入口、子操作、图片和结果

[返回首页](../README.md) · [24 个工具的操作手册](features.md) · [完整图片墙](../screenshots/README.md) · [动手示例](../examples/README.md)

第一次使用见[三分钟上手](quickstart.md)；按任务操作见[六个教程与效果对比](tutorials.md)，异常处理见[故障排查](troubleshooting.md)。

这里按用户能完成的事情整理功能，既包含花屿中的工具，也包含工作台内部操作。0.6 为当前正式下载基线；标注 **0.7 候选** 的功能已在本地实现，尚未作为公开正式版发布。界面图不等于每个功能分支都已实机验收，实际范围见[验证说明](validation.md)。

## 24 个工具入口

| 分类 | 工具 | 输入与结果 | 图片与步骤 |
|---|---|---|---|
| 转换 | 图片格式转换 | PNG / JPG / BMP 互转，设置 JPG 质量 | [操作](features.md#image-convert) · [图](../screenshots/image-convert.png) |
| 转换 | 办公文档转 PDF | DOCX / XLSX / PPTX，使用已有办公引擎 | [操作](features.md#document-convert) · [图](../screenshots/office-convert.png) |
| 图片 | 调整尺寸 | 宽高、比例与缩放预设，另存新图片 | [操作](features.md#resize) · [图](../screenshots/image-resize.png) |
| 图片 | 裁剪与旋转 | 拖框、输入像素、比例预设、90°旋转 | [操作](features.md#crop) · [图](../screenshots/image-crop.png) |
| 图片 | 图片批处理 | 多图、等比缩小、统一格式、逐张输出 | [操作](features.md#image-batch) · [图](../screenshots/image-batch.png) |
| 图片 | 图片 / PDF 水印 | 单行文字、位置、透明度、字号与批量另存 | [操作](features.md#watermark) · [图](../screenshots/watermark.png) |
| PDF | PDF 拆分 | 单页、范围或页面列表导出 | [操作](features.md#pdf-split) · [图](../screenshots/pdf-split.png) |
| PDF | PDF 合并 | 多文件排序后合并 | [操作](features.md#pdf-merge) · [图](../screenshots/pdf-merge.png) |
| PDF | PDF 统一 A4 | 逐页尺寸检查、保留横纵、等比居中 | [操作](features.md#pdf-a4) · [图](../screenshots/pdf-a4.png) |
| PDF | PDF 添加水印 | 带轻舟恢复标记的新 PDF | [操作](features.md#pdf-watermark) · [图](../screenshots/pdf-watermark.png) |
| PDF | 移除轻舟水印 | 只恢复本软件标记，不处理任意扫描水印 | [操作](features.md#pdf-remove-watermark) · [图](../screenshots/pdf-remove-watermark.png) |
| 截图 | 截图 | 框选、窗口、全屏、标注、OCR、翻译与输出 | [操作](features.md#capture) · [专题](capture.md) |
| 截图 | 桌面贴图 | 留置已有图片或未保存截图，移动、缩放和另存 | [操作](features.md#pin-image) · [图](../screenshots/pinned-image.png) |
| 压缩 | 压缩文件 | 多文件 / 文件夹 ZIP；可选 7z | [操作](features.md#compress) · [图](../screenshots/archive-compress.png) |
| 压缩 | 解压文件 | 内置 ZIP；可选普通 7z / RAR | [操作](features.md#extract) · [图](../screenshots/archive-extract.png) |
| 压缩 | 预览 ZIP | 不解压查看目录、条目与声明大小 | [操作](features.md#zip-preview) · [图](../screenshots/zip-preview.png) |
| 效率 | 打开文件 | Windows 默认或明确设置的轻舟内优先 | [操作](features.md#open) · [图](../screenshots/flower-efficiency.png) |
| 效率 | 常用打开方式 | 系统默认 / 推荐、自定义 EXE、追加推荐 | [操作](features.md#open-with) · [图](../screenshots/open-with.png) |
| 效率 | 定位文件 | 在资源管理器中选中源文件 | [操作](features.md#locate) · [入口图](../screenshots/flower-efficiency.png) |
| 效率 | 复制路径 | 复制完整路径到剪贴板 | [操作](features.md#copy-path) · [入口图](../screenshots/flower-efficiency.png) |
| 效率 | 重命名文件 | F2 / 工具入口，保留扩展名和路径同步 | [操作](features.md#rename) · [图](../screenshots/rename.png) |
| 效率 | 批量重命名 | 前后缀、序号、预览、冲突检测与恢复记录 | [操作](features.md#rename-batch) · [细节图](../screenshots/rename-rules-0.7.2.png) |
| 效率 | 预览文本 | 编码、搜索、命中跳转、换行和刷新 | [操作](features.md#text-preview) · [图](../screenshots/preview-dark-0.7.2.png) |
| 效率 | 数据科学 | CSV / TSV 处理、流程复用、追加和四种绘图 | [操作](features.md#data-science) · [完整专题](data-science.md) |

定位、复制路径和默认打开属于直接动作，没有独立工作台，所用图片明确标为入口图；无需虚构一个专门的结果窗口。

## 数据科学：展开后还有什么

| 能力 | 子操作 | 图文 / 结果 |
|---|---|---|
| 读取与预览 | 文件打开 / 拖入，六种编码选择、有限预览、原始预览 | [工作台](data-science.md#先认识工作台) |
| 文本筛选 | 包含、等于、不包含、不等于 | [全部条件与示例](data-science.md#16-种筛选与组合条件) |
| 空值筛选 | 为空、不为空 | [条件表](data-science.md#16-种筛选与组合条件) |
| 数值筛选 | 等于、大于、大于等于、小于、小于等于、闭区间 | [条件表](data-science.md#16-种筛选与组合条件) |
| 日期筛选 | 同日、早于、晚于、闭区间 | [条件表](data-science.md#16-种筛选与组合条件) |
| 条件组合 | 最多八条，AND / OR，增删条件 | [独立细节图](../screenshots/data-combined-filters-0.7.2.png) |
| 列设置 | 保留列、输出列名，去重键与分组列 | [独立细节图](../screenshots/data-field-options-0.7.2.png) |
| 类型 | 文本、十进制、三种日期输入，统一日期输出 | [操作](data-science.md#选列改列名类型转换与清理) |
| 清理 | 首尾空白、相关列含空值的行、按单 / 多列键去重 | [实际导出](../examples/cleaned.csv) |
| 汇总 | 多列分组，计数 / 求和 / 平均 / 最小 / 最大 | [实际输出](../examples/region-totals.csv) |
| 按行合并 | 同表头同顺序，2–100 份，单表头输出 | [工作台](../screenshots/data-append.png) |
| 流程复用 | 保存 / 载入 JSON，核对编码与列结构 | [可下载流程](../examples/east-over-100.json) |
| 汇总图 | 条形 / 分类折线，10 / 20 / 50 组，精确值表 | [图形说明](data-science.md#四种绘图不安装额外环境) |
| 数值图 | 直方 / 散点，固定种子、最多一千点、分箱与空值说明 | [图形说明](data-science.md#四种绘图不安装额外环境) |
| 图形导出 | PNG；汇总图保留内嵌完整标签与数据说明 | [真实输出](../examples/region-line.png) |
| 任务状态 | 取消、参数改变使结果失效、预算与非法输入提示 | [边界](data-science.md#规模与失败处理) |

## 截图工作台内部操作

| 能力 | 子操作 | 图文 |
|---|---|---|
| 选区 | 框选 / 窗口 / 全屏，拖动手柄、键盘微调、重新截图 | [操作](capture.md#截图和选区调整) |
| 标注 | 矩形、箭头、文字、打码、撤销 | [细节图](../screenshots/capture-annotation-options-0.7.2.png) |
| 样式 | 六色色板、线宽、文字字号 | [操作](capture.md#标注色板线宽和文字) |
| OCR | 中 / 英 / 系统语言、本地识别、编辑与复制原文 | [图](../screenshots/capture-ocr.png) |
| 翻译 | 中英互译、复制译文、取消与失败保留原文 | [图](../screenshots/capture-translation.png) |
| 服务配置 | **0.7 候选**：MyMemory / LibreTranslate、地址、密钥、测试连接 | [图](../screenshots/translation-service-0.7.2.png) |
| 输出 | 复制、保存、保存并贴图、直接贴图 | [操作](capture.md#输出与桌面贴图) |
| 贴图交互 | 移动、滚轮缩放、边角调整、还原、另存、置顶和关闭 | [图](../screenshots/pinned-image.png) |
| 快捷键 | 截图 / OCR / 翻译配置与冲突提示 | [图](../screenshots/shortcuts.png) |

## 花屿、文件整理与设置

| 能力 | 子操作 | 图文 |
|---|---|---|
| 分类与工具库 | 六分类、搜索、常用优先、最多九操作、不可用原因 | [工具库](../screenshots/tool-library.png) |
| 主题 | **0.7 候选**：经典 / 圆弧、自动保存；0.7.2 全工作台同步 | [主题专题](desktop.md#主题与大小) |
| 形态 | 保持紧凑、三档大小、展开、小花心 | [图](../screenshots/desktop-options-automatic.png) |
| 多开 | 保留文件花屿，收起恢复，独立工作台 | [操作](desktop.md#多开收起与工作台置顶) |
| 窗口管理 | 标题拖动、独立置顶、关闭、托盘找回 | [操作](desktop.md#多开收起与工作台置顶) |
| 自动展开 | 总开关、暂停十分钟、目录排除与恢复、监听重连 | [操作](desktop.md#自动展开暂停和监听恢复) |
| 动画 | 设置不同展开动画或关闭动画 | [设置入口](../screenshots/desktop-options-menu.png) |
| 启动 | 登录自启；**0.7 候选**手动首次显示与重复唤起 | [说明](desktop.md#自动展开暂停和监听恢复) |
| 打开方式 | Windows 默认 / 推荐、自定义、排序、显式优先、追加系统推荐 | [行为表](desktop.md#windows-默认与推荐打开方式) |
| 改名 | F2、前后缀、保留主名或序号、恢复 JSON、哈希复核 | [操作与细节图](desktop.md#f2单文件与批量重命名) |
| 文本阅读 | 查找、上 / 下一处、换行、刷新、编码切换 | [操作](desktop.md#预览定位和复制路径) |
| 关于与品牌 | 程序图标、版本信息、第三方许可入口 | [关于图](../screenshots/about.png) |

## 可选组件与输出保障

| 能力 | 子操作 | 图文 |
|---|---|---|
| 办公引擎 | LibreOffice / Microsoft Office、已有程序选择与检测 | [能力表](components.md#需要什么组件) |
| 压缩增强 | 7-Zip / Bandizip、格式与线程选项 | [压缩图](../screenshots/archive-compress.png) |
| 组件管理 | 导入、取消、启停、刷新、占用、自管移除 | [当前图](../screenshots/components-current-0.7.2.png) |
| PDF 原页预览 | **0.7 候选**：Windows 处理器或可选 MuPDF | [说明](components.md#pdfa4顺序水印) |
| 文件输出 | 原目录 / 桌面 / 文档 / 自选位置、查看结果 | [说明](components.md#压缩解压与安全另存) |
| 失败与取消 | 原文件保留、拒绝覆盖、单文件半成品清理、批量保留已完成项 | [说明](components.md#压缩解压与安全另存) |
| 安装与便携 | 安装包、ZIP、SHA-256；**0.7 候选**版本并存、标准卸载和回退 | [下载说明](../releases/README.md) |

## 尚未实现的内容

大 XLSX 结构化导入 / 编辑、公式 / 透视表 / 跨表 JOIN、产品内 Parquet / DuckDB、通用扫描 PDF 去水印、密码 / 分卷归档、RAR 创建和内置离线翻译模型仍不在当前能力中。目录不会将路线图条目当成已完成，也不把可选外部软件的全部功能算作轻舟功能。
