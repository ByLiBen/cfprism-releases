# cfprism v1.1.13

## 更新检查可靠性修复

- 修复 GitHub 未认证 API 达到每小时限额后，客户端检查更新直接报 `403 Forbidden` 的问题。
- 保留 GitHub Releases API 为主通道；接口限流、网络失败或响应异常时，自动切换到公开静态更新清单。
- 回退通道仍强制校验 Windows AMD64 离线包名称和 GitHub SHA-256 digest，不降低更新包完整性要求。

## Windows AMD64 离线包

- 文件：`cfbest-sub-gui-offline-windows-amd64.zip`
- SHA-256：`11b15b86194bb7cede6fb0742e7bd2d888a3396d7d17cc9db0ddfea0c9e846e1`
- GUI SHA-256：`01ad5b0b8c9c7f93231e376d10730a8376b1738bab15003ec6ca7f2fddb4a59b`
- 随包 CloudflareSpeedTest：`v2.3.5`
- 随包 Mihomo：`v1.19.30`

请完整解压 ZIP 后运行 `cfbest-sub-gui.exe`。
