# cfprism v1.1.8

## 局域网订阅接口修复

- 修复局域网订阅链接被额外随机 Token 阻断的问题。现在生成的 `/sub/`、`/sub/clash`、`/sub/json` 地址可直接在浏览器和客户端中访问、导入。
- 修复 Clash/Mihomo 导入局域网 YAML 订阅时出现 `502 Bad Gateway` 的问题；接口现在正确返回 YAML 内容。
- 登录有效时允许订阅接口服务；退出登录或会话失效时，仍会立即停止运行任务、定时计划和订阅 HTTP 服务，防止绕过登录后持续使用。

## Windows AMD64 离线包

- 文件：`cfbest-sub-gui-offline-windows-amd64.zip`
- SHA-256：`cac499c9c550b634bb3be49b31bc53ea59f6692c8355130d019c008d9954e1a0`

请完整解压 ZIP 后运行 `cfbest-sub-gui.exe`。
