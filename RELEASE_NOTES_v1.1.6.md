# cfprism v1.1.6

## 回退为可复现的串行下载复核

- 取消候选 IP 的并发下载复核，所有候选均逐个串行测速，不再共享本地带宽。
- 移除带宽基线、公平份额和批次聚合吞吐对优选流程的影响，恢复稳定的单连接测速筛选。
- 保留端口独立容错：单个端口不可用不会中断其它端口的订阅裂变。
- 保留 v1.1.5 的大尺寸实时输出面板，便于查看完整测速过程。

## Windows AMD64 离线包

- 文件：`cfbest-sub-gui-offline-windows-amd64.zip`
- SHA-256：`3ca9b2554cbe1a91e8ad4079ed2119c9c6ccc730d2fcfb2b8e61e1df325cbb64`

请完整解压 ZIP 后运行 `cfbest-sub-gui.exe`。
