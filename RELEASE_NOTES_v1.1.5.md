# cfprism v1.1.5

## 并发复核可见化与日志体验优化

- Cloudflare 线路优选的实时输出面板已显著加高，运行中可查看更多命令输出并滚动回看。
- 下载复核阶段会明确展示当前批次、最大并发数和已取得的合格节点数。
- 宽带基线阶段会显示实测基线、85% 并发预算、并发管道数和公平速度份额。
- 保持 v1.1.4 的并发复核策略：默认最多 4 路候选下载复核，最终结果仍会串行复测确认单节点能力。

## Windows AMD64 离线包

- 文件：`cfbest-sub-gui-offline-windows-amd64.zip`
- SHA-256：`33d4af963884aaeabcd440adbad361a12eeeb48ebfe6c334ddb2103417675167`

请完整解压 ZIP 后运行 `cfbest-sub-gui.exe`。
