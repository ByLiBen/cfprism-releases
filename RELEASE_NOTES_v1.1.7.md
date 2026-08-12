# cfprism v1.1.7

## 定时订阅与局域网订阅中心

- 新增独立的“订阅中心”模块，可集中查看服务状态、订阅地址、计划摘要和下一次执行时间；通用订阅、Clash/Mihomo、sing-box 地址均可单独复制或一键复制。
- 支持多个订阅源：每行一个 URL、本地文件、Base64 内容或 `vmess://`、`vless://`、`hy2://` 链接；输入区会显示已填写的来源数量，Enter 仅换行，Ctrl+Enter 才开始任务。
- 支持智能开关式的计划任务：按间隔、每日指定时间或每周指定星期与时间执行。计划触发后复用正常任务链路并原子更新订阅产物。
- 内置局域网订阅 HTTP 服务，监听所有网卡并优先展示系统默认出网路由对应的 Wi-Fi/有线网卡地址，避免将代理、TUN、VMware 或 Hyper-V 虚拟网卡地址作为首选。
- 未登录、会话失效或退出登录时，会立即停止测速、计划任务和局域网订阅服务；订阅接口也会在每次请求时复核登录状态。
- 订阅结果支持通用 Base64、Clash/Mihomo YAML 和 sing-box JSON；VLESS/HY2 节点会保留并导出。

## Windows AMD64 离线包

- 文件：`cfbest-sub-gui-offline-windows-amd64.zip`
- SHA-256：`6bccaa924099fcbc45707c2515a6f2cac0107cd5070b72ebefbb5c3df434e5a1`

请完整解压 ZIP 后运行 `cfbest-sub-gui.exe`。
