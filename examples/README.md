# 可下载、可核对的演示文件

全部数据为合成内容，可用来体验[数据科学专题](../docs/data-science.md)。没有私人文件、密钥或本地源路径。CSV / JSON 是示例数据，不是程序源码；无需安装开发环境。

[从三分钟上手开始](../docs/quickstart.md) · [六个完整任务与效果对比](../docs/tutorials.md)

| 文件 | 用法 |
|---|---|
| [sales.csv](sales.csv) | 6 条销售记录，A003 故意重复一次，日期使用斜杠格式 |
| [cleaned.csv](cleaned.csv) | 真实 UI 另存：订单去重、金额改名、日期标准化，保留 5 条 |
| [east-over-100.json](east-over-100.json) | 轻舟真实保存并重新载入过的流程：华东且金额 ≥ 100 |
| [region-totals.csv](region-totals.csv) | 真实全文件汇总：先按订单去重，再按地区求和 |
| [region-line.png](region-line.png) | 从真实全文件汇总图窗口另存的分类折线 PNG |

## 五分钟操作

1. 下载 `sales.csv`。在 GitHub 文件页选择 Raw / Download raw file，保存原始文件；不要把网页 HTML 保存成 CSV。
2. 在轻舟「数据科学」打开，编码保持「自动 / BOM」。初始预览有 6 条记录。
3. 将「金额」设为十进制、「日期」设为「日期 yyyy/MM/dd」，把金额输出列名改成「销售额」。
4. 在「订单」列勾选去重键，开启「按键去重（保留首条）」，点击「预览处理」；得到 5 条，日期统一为横杠格式。点击「处理并另存」后可对照 `cleaned.csv`。
5. 要复用筛选：重新打开原始 `sales.csv`，下载并载入 `east-over-100.json`，再点「预览处理」。结果应只有 A001、华东、120、2026-11-01。
6. 要看汇总：重新打开原始文件，按订单去重、勾选地区分组，选择「分组求和」和金额数值列，另存。华东 180、华南 175、华北 110，与 `region-totals.csv` 一致。
7. 另存成功后点「查看图表」，分别查看条形图与折线图，尝试保存 PNG。分类折线的横轴是分类顺序，不表示时间连续。

分享自己的流程前请检查筛选词和列名；轻舟的改名恢复记录含真实完整路径，与这里的无路径数据流程不同。

## PDF 与图片真实输入输出

以下结果由轻舟 0.7.2处理。基础能力在 0.6 已有，本次不据此宣称旧版的逐字节输出完全一致。

| 文件 | 用途 |
|---|---|
| [mixed-pages.pdf](pdf/mixed-pages.pdf) | 三页合成 PDF，160×240、300×180、210×297 mm；前两页不是 A4 |
| [a4-pages.pdf](pdf/a4-pages.pdf) | 实际转换结果，纵 / 横 / 纵三页 A4；文字保留、X/Y 等比 |
| [landscape.png](images/landscape.png) · [portrait.png](images/portrait.png) · [small.png](images/small.png) | 1200×800、800×1200、320×240 三张合成原图 |
| [landscape_batch.jpg](images/landscape_batch.jpg) · [portrait_batch.jpg](images/portrait_batch.jpg) · [small_batch.jpg](images/small_batch.jpg) | 最长边 600、JPG 质量 90 的实际结果；小图不放大 |
| [landscape-watermark.png](images/landscape-watermark.png) | 在横图结果上添加「轻舟演示」的实际 PNG |
| [rename-result.csv](rename-result.csv) | 两份合成文件真实改名 / 恢复后的名称表，不含恢复路径 |
| [performance-0.6.json](performance-0.6.json) | 历史本地构建的脱敏采样，非当前候选 / 正式包性能基准，见[测量说明](../docs/performance.md) |

共 16 个示例 / 测量文件。PDF 含可下载的实际二进制文档，不是软件程序；图片也可直接保存后体验。GitHub 预览网页不等于文件本身，下载请使用 Raw / Download raw file。
