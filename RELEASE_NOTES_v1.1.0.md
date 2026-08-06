## cfprism v1.1.0

这是新公开发布仓库中的首个版本，发行资产与原仓库的 `v1.1.0` 完全一致。

### 主要更新

- 自动刷新 Cloudflare 官方 IPv4/IPv6 地址段，支持 ETag、24 小时缓存和离线回退
- 渐进式下载候选补位：每批 20 个、最多 100 个，直到找到目标数量或候选耗尽
- 新增 TCP、TLS、TTFB 与固定字节下载速度分阶段指标
- 严格区分合格、降级与失败结果；降级候选不会进入订阅或地区 IP 池
- 新增每端口 `verified-results-端口.csv`，记录状态和淘汰原因
- GUI 显示质量状态、详细阶段指标、IP 池来源和降级候选
- 修复自定义 IP 文件兼容，支持单个 IP 与 CIDR

### 下载

下载 `cfbest-sub-gui-offline-windows-amd64.zip`，完整解压后运行 `cfbest-sub-gui.exe`。

资产 SHA-256：

```text
13f48a70ad4923dafb5dfb370e0f24e694e71e7b3143d30818b9498efa19bd26
```
