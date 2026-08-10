# cfprism v1.1.3

本版本修复了订阅导入时一个不可用端口会中断整个裂变任务的问题，并提高了候选 IP 下载复核的效率。

## 主要更新

- 订阅中的端口现在独立测速：某个端口失败或没有严格合格 IP 时，其他成功端口仍会继续裂变和导出。
- 保留原节点时，失败端口节点会保持原样；仅导出优选节点时，失败端口节点会被排除。
- 输出目录新增 `port-summary.json`，记录每个端口的成功、跳过状态、合格 IP 数和失败原因。
- 候选 IP 下载复核支持默认最多 4 路并发，可在 `configs/default.yaml` 中通过 `verify_concurrency` 调整。
- 复核日志增加批次聚合吞吐；优选排序仍使用单连接实测速率，不会把速率简单按并发数倍增。

## 使用说明

1. 下载 `cfbest-sub-gui-offline-windows-amd64.zip`。
2. 完整解压 ZIP 后运行 `cfbest-sub-gui.exe`。
3. 导入包含多个 Cloudflare HTTPS 端口的订阅时，可在输出目录查看 `port-summary.json` 了解被跳过端口的原因。

## 下载资产

资产名称：`cfbest-sub-gui-offline-windows-amd64.zip`

SHA-256：

```text
57b00113cd530c02929f882cf762761b83948b5893c71a833f0a3ec0ea199d02
```
