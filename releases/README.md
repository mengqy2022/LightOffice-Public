# 发行版下载说明

安装包在 GitHub 的 Releases 页面发布。本目录只保存下载和校验说明，不保存安装包、引擎包或源代码。

发布者需先上传经过验证的 `LightOffice-0.5.1.0-windows.zip` 和同名 `.sha256`，然后发布 Release。当前本地导出不等于已经公开发布；没有 Release 时无可下载资产。

Windows PowerShell 校验示例：

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath .\LightOffice-0.5.1.0-windows.zip
Get-Content -LiteralPath .\LightOffice-0.5.1.0-windows.zip.sha256
```

确认两个哈希一致后解压，运行 `LightOffice.exe`。保留同目录 DLL、配置文件与许可证。主程序需要 Windows 10/11 和系统 .NET Framework 4.8。LibreOffice、7-Zip 等可选组件单独安装，不包含在基础 ZIP 中。

更新前从托盘退出旧版，再解压到新目录。启用过开机自启的用户，应在旧版关闭启动项，在新目录运行后重新开启，避免 Windows 继续指向旧路径。
