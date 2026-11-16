# 轻舟 LightOffice 0.8.0.0

[下载](../releases/README.md) · [中文任务教程](task-center.md) · [English task guide](task-center.en.md) · [验证范围](validation.md)

## 本版重点

统一批量任务中心：图片、批量改名与恢复、PDF拆分/合并/A4、压缩/解压以及CSV/TSV读取、预览、导出和追加统一排队，显示阶段、结果、错误及取消入口。重型处理复用已有单工作线程，无新运行依赖。

最近100条任务元数据本地保存。重启后查看历史，上次未完成任务标记已中断，**不会自动重放或断点续跑**。关闭任务窗口不会停止后台操作；有活动任务时须等待或取消，再退出轻舟。清理历史不删除输出。

不同文件可以同时使用独立重命名窗口，同一文件复用；Enter成功后关闭，失败保留。文件夹连续分页复用枚举与排序缓存；CSV样本读取、预览和导出准备在后台进行，可取消；任务列表按变化刷新，隐藏/最小化时暂停界面更新。

## 安装与更新

需要Windows 10/11及系统.NET Framework 4.8。安装向导支持自定义可写目录、许可说明、运行中提示、开始菜单与原生卸载程序。识别Inno旧版后沿用原目录与卸载身份，跳过哈希相同文件，保留设置、历史及可选引擎；升级前从托盘正常退出。

更新仍是完整离线下载，不是网络差分包。便携ZIP请保留同目录DLL和许可文件。程序及安装器未代码签名，从官方Release下载并核对SHA-256。

## 验证与限制

受保护EXE的SHA-256为 `CD064CCE36458548E084F03ADF6D6DA03D5FDA6E77E82C589520D93079FA0CD1`。本轮进行了集中定向回归、隔离真实安装/升级/卸载、完整Main生命周期、进程终止恢复、大CSV/图片资源测量、三主题实际DPI检查及短时现代待机验证。全部范围与测量定义见[验证说明](validation.md)和[性能记录](performance.md)。

没有验证所有Windows版本、低配/干净系统、长时间睡眠、休眠、磁盘满、真实断电或全部安全软件组合。截图和示例使用合成输入。基础包不捆绑LibreOffice、7-Zip、Bandizip、Python/R；无结构化XLSX编辑、任意PDF去水印或超大Excel快速导入承诺。

## English release notes

**0.8.0.0 introduces a unified batch task center.** Image batches, rename/recovery, PDF operations, archives and CSV/TSV workflows report queue state, stages, cancellation and results. The existing single heavy worker is reused, with no new runtime engine.

Up to 100 local metadata records survive restart. Unfinished jobs become Interrupted; work is never automatically replayed or resumed. Closing the task window leaves work running. Clear completed removes history, preserving outputs. Wait for or cancel active jobs before exiting.

Independent rename windows, Enter-to-finish, cached folder paging, background CSV preparation and event-driven refresh improve interaction. The installer retains existing Inno installation identity, skips unchanged files and protects user data. Updates are full downloads. Both EXE and installer are unsigned; verify the official SHA-256 files.

Validation includes focused regressions on the protected EXE, isolated installation/upgrade/uninstallation, production Main lifecycle, forced termination recovery, synthetic 100/500 MiB CSV and 30-image measurements, actual mixed-DPI windows in three themes and user-triggered short S0 standby. This is not proof of all hardware, clean systems, prolonged standby, hibernation or power-loss behavior. The application/installer remain Chinese; the task guide and overview are bilingual.

Developer: **Mengqy** · Development platform: **Codex** · [Product blog](https://www.mqymmb.com/posts/lightoffice/) · Feedback: **15877464851@163.com**. Licensing details: [license note](https://www.mqymmb.com/posts/lightoffice/#license-note).
