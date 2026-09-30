<div align="center">

<img src="assets/readme-banner.svg" width="100%" alt="GitHub Level" />

# GitHub Level

个人公开活动归档 · 自动增量记录 · 项目入口

[活动记录](activity.txt) · [刷新日志](daily_log.txt) · [个人网站](https://cngyzzh.github.io) · [工作流](https://github.com/CnGyZzh/Level/actions)

</div>

## 这个仓库做什么

保存 CnGyZzh 的公开 GitHub 活动快照，方便回看提交、讨论等事件。可视化个人网站位于 [CnGyZzh.github.io](https://github.com/CnGyZzh/CnGyZzh.github.io)，本仓库主要保存文本记录和更新工作流。

## 从这里开始

| 文件 | 用途 |
| :--- | :--- |
| [activity.txt](activity.txt) | 公开活动记录；新增事件去重后放在文件前面。 |
| [daily_log.txt](daily_log.txt) | 发现新活动时追加的刷新时间记录。 |
| [update-activity.yml](.github/workflows/update-activity.yml) | 拉取公开事件、更新文件并提交的 GitHub Actions 工作流。 |

## 更新方式

- **定时刷新**：工作流设置为每天 02:17 UTC（北京时间 10:17），实际启动时间由 GitHub Actions 调度决定。
- **手动刷新**：打开 Actions → **Refresh activity logs** → **Run workflow**。
- **增量保存**：每次读取最多 100 条公开事件，按生成的记录行去重；没有新记录时不会新增提交。

工作流使用仓库自带的 GITHUB_TOKEN，并需要 contents: write 权限。Fork 后如需记录自己的活动，请修改工作流中的 GITHUB_OWNER，并启用 Actions。

> 这是公开事件的快照归档，不等同于 GitHub 贡献日历，也不保证覆盖完整历史。刷新日志表示抓取时间，不代表当天的贡献次数。

## 项目导航

| 项目 | 方向 |
| :--- | :--- |
| [WeType Monet](https://github.com/CnGyZzh/WeType_Monet-Gy) | 微信输入法动态配色。 |
| [HyperMax](https://github.com/CnGyZzh/HyperMax) | Xiaomi 17 Pro 刷新率、触控与温控整合适配。 |
| [个人网站](https://github.com/CnGyZzh/CnGyZzh.github.io) | 项目索引与发布记录。 |
| [个人主页](https://github.com/CnGyZzh/CnGyZzh) | GitHub Profile README 与贡献动画。 |

## 反馈与维护

记录异常时，请在 [Issues](https://github.com/CnGyZzh/Level/issues) 提供记录行、日期和对应 GitHub 事件链接。仓库当前未声明单独的开源许可证。
