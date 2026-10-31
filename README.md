# GCP 永久免费小鸡全流程部署

这是一份实测跑通的 GCP Always Free VPS 部署技能：从先领 300 美元试用金和每月 10 美元额度开始，到建 e2-micro 免费机、预算告警、CDN 出站屏蔽、流量只限流、Debian 换源、dae 出站，一直到测试页验收。

## 给 Muse 用

把下面这个页面的链接直接发给你的 Muse，告诉它按里面的步骤帮你配置部署 Google VPS：

https://github.com/pierpont-morgan/gcp-free-vps-skill/blob/main/SKILL.md

也可以把 `SKILL.md` 全文发给 Muse，或者把这个仓库的 `SKILL.md` 放进 Muse 的 custom-skills 目录使用。

## 注意

- 只用免费边界：e2-micro、30GB pd-standard、标准网络层，不开静态 IP、快照、GPU。
- 节点链接、订阅链接、UUID、WS 路径等凭证不要写进这个仓库，只直接写进机子上的 dae 配置文件（权限 0600）。
- 预算告警只提醒、不自动停机；流量超 180GB 只限流、不关机。
