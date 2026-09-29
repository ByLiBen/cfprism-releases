# cfprism v1.1.15

## 优选助手鉴权与会话恢复

- 对齐软件专用登录、会话校验和退出接口；按服务端返回的 `expires_in_sec` 约束令牌有效期，不使用刷新令牌或网站登录接口回退。
- 同账号在另一台优选助手登录后，旧会话需要重新登录。适配服务端独立的软件会话版本，使安卓 App 和 Windows Magic Cat 登录不再挤掉优选助手会话。
- Windows GUI 使用当前用户加密存储登录令牌，重启时必须在线校验后才恢复；主动退出清理本地凭据。
- 订阅或软件权限不足时停止受保护功能并提示前往网站处理；临时网络故障保留凭据，可稍后重试。订阅来源和请求错误不再回显订阅密钥。

## Windows AMD64 离线包

- 文件：`cfbest-sub-gui-offline-windows-amd64.zip`
- SHA-256：`152e8cecaac2c575089f315175cbc1a8702aaec14ff659cc59c646a67ab5968e`
- GUI SHA-256：`28b2d54b958a38e322319b9af27515866e083f6f3975607440ba8c27f0b1dee0`
- 随包 CloudflareSpeedTest：`v2.3.5`
- 随包 Mihomo：`v1.19.31`

请完整解压 ZIP 后运行 `cfbest-sub-gui.exe`。网站端的软件会话版本隔离须先完成部署。
