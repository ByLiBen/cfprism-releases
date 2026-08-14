# cfprism v1.1.9

## VLESS 现代传输支持

- 新增 `VLESS + XHTTP + TLS + CDN` 节点识别、优选 IP 裂变、端口扫描、参数保留和 Mihomo 配置输出。
- 新增 `VLESS + HTTPUpgrade + TLS + CDN` 节点支持；Mihomo 兼容输出 HTTPUpgrade，sing-box 输出原生 `httpupgrade` 传输。
- 支持从 VLESS 分享链接、Clash/Mihomo YAML 和 sing-box JSON 导入节点，并在 `proxy-links.txt` 中混合导出 VMess、VLESS XHTTP 和 VLESS HTTPUpgrade 链接。
- 二次测速可使用 Mihomo 对 VLESS 节点进行延迟与吞吐复测；sing-box 不再生成当前内核无法使用的 XHTTP 出站。

## 稳定性改进

- 保留 VLESS 的 SNI、Host、路径、指纹、ALPN、XHTTP 模式和扩展参数，仅替换连接地址与测速端口。
- 优化 Linux Web 控制台的设置持久化、订阅访问和测试流量路由隔离。

## Windows AMD64 离线包

- 文件：`cfbest-sub-gui-offline-windows-amd64.zip`
- SHA-256：`92a51211e2349492dc33071d191ff97e923e28a06e315a4d10bc434bed0767af`
- 随包 Mihomo：`v1.19.29`，已验证可加载 XHTTP 与 HTTPUpgrade 节点配置。

请完整解压 ZIP 后运行 `cfbest-sub-gui.exe`。
