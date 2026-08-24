# cfprism v1.1.11

## 统一功能与授权保护

- 合并 Windows 桌面端、CLI 与 Linux Web 控制台的最新源码，避免发布分支间的功能回退。
- 桌面端软件登录会严格校验订阅套餐和到期时间；授权失效、订阅过期或离线会话超过 12 小时会要求重新登录。
- CLI 现同样要求软件登录，并在运行期间持续检查授权状态。

## 节点与配置能力

- 保留 VLESS XHTTP、HTTPUpgrade、Reality 和 Trojan 分享链接的导入、优选 IP 替换、端口扫描与配置导出能力。
- 合并局域网订阅、并发验证稳定性、Linux Web 控制台和软路由模板管理等更新。

## Windows AMD64 离线包

- 文件：`cfbest-sub-gui-offline-windows-amd64.zip`
- SHA-256：`941bfd9d2d91d31b00d622e69e2042dd09642a5bcf816b4fcee725976a6559b2`
- 随包 CloudflareSpeedTest：`v2.3.5`
- 随包 Mihomo：`v1.19.30`

请完整解压 ZIP 后运行 `cfbest-sub-gui.exe`。
