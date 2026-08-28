# cfprism v1.1.12

## Cloudflare 优选排序修复

- 每个端口会完整复核本端口候选池（默认最多 100 个），再按单连接实测速率、TTFB、丢包和初筛延迟排序并保留 Top N。
- 修复旧版在某一批次凑够 Top N 后提前停止、可能遗漏后续更快候选的问题。
- 多端口结果保持端口独立：每个端口分别保留 Top N，合并时不再跨端口二次淘汰相同 IP。
- 完整候选池复核会增加线路优选耗时和测试流量，但结果更稳定、更符合全量候选的实际排序。

## Windows AMD64 离线包

- 文件：`cfbest-sub-gui-offline-windows-amd64.zip`
- SHA-256：`25d0e71f812dce4776b63b69f349edcf31e05d8e32338d43d76118497ac540fc`
- GUI SHA-256：`5c5770da3688cbb09de26682289457c3a8fc7441846292d4371a09887bb71708`
- 随包 CloudflareSpeedTest：`v2.3.5`
- 随包 Mihomo：`v1.19.30`

请完整解压 ZIP 后运行 `cfbest-sub-gui.exe`。
