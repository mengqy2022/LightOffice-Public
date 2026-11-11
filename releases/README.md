# 下载、校验与更新

正式入口：[GitHub Releases](https://github.com/mengqy2022/LightOffice-Public/releases/latest)。安装文件作为 Release 资产分发，此目录只保存说明，不保存源码。

当前正式发布为 **0.6.0.0**。文档中带 0.7 / 0.7.2 标记的图片来自本地候选，尚未作为 Release 资产发布，不能通过下载下表文件获得候选功能，详见[候选说明](../docs/preview-0.7.md)。

| 文件 | 用途 |
|---|---|
| `LightOffice-0.6.0.0-Setup.exe` | 当前用户安装、创建品牌快捷方式、可选完成后运行 |
| `LightOffice-0.6.0.0-windows.zip` | 便携包，解压后运行 EXE |
| 对应的 `.sha256` | SHA-256 校验值 |

需要 Windows 10 / 11 和 .NET Framework 4.8。基础包不含 LibreOffice、7-Zip、Bandizip、Python / R；按需配置已有引擎。程序及安装器目前未做代码签名，请从上述发布页取得文件并核对校验值。

PowerShell 校验示例：

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath .\LightOffice-0.6.0.0-Setup.exe
Get-Content -LiteralPath .\LightOffice-0.6.0.0-Setup.exe.sha256
```

对 ZIP 同样操作。计算结果应与 `.sha256` 第一列完全一致。不要只复制便携包中的 EXE，保留同目录 DLL、配置和第三方许可。

更新前从托盘退出旧版并关闭工作台。登录自启按实际运行路径注册，换目录前在旧版关闭，新版启动后重新开启。安装器不申请管理员权限，相同版本目录存在时只做校验，不覆盖修改过的文件。

0.6 没有控制面板卸载入口。先关闭自启、退出，再删除版本目录与快捷方式即可；已有导出文件和用户设置不会自动删除。0.7 候选安装版已实现当前用户的按版本卸载项，卸载保留个人设置与可选组件；其干净系统验收和正式发布仍待完成。

[使用说明](../docs/usage.md) · [功能手册](../docs/features.md) · [更新记录](../docs/changelog.md)

第一次安装可按[三分钟上手](../docs/quickstart.md)操作；遇到启动或引擎问题先看[故障排查](../docs/troubleshooting.md)。不同版本与回退步骤集中在[版本说明](../docs/versions.md)。
