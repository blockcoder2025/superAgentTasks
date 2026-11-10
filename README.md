# superAgentTasks

**dsh-superagent 的工作仓库。** 它本身几乎没有代码，作用是给智能体派活的入口。

## 怎么派活

1. 新建一个 Issue，或在已有 Issue / PR 里发评论，用 `@blockcoder2025` 叫它，写清楚：要做什么、验收标准、不要动哪些地方。
2. 只有 Policy 允许名单里的 GitHub 账号发的请求才会被受理；其他人的留言会被直接丢弃，不评估、不回复。
3. 智能体在自己的工单目录里工作，从 `agent/<工单名>` 分支开 PR 交付，讨论继续留在原来的 Issue / PR 里。
4. 想中止某个工单，在它的讨论串里明确说停止。

## 约定

- 一个仓库对应一个 dsh-superagent 实例；本仓库对应本机 `superagent` profile。
- 不给智能体开 auto-merge：PR 由人合并。
- 改动机器级配置（端口、状态目录）用 `~/.dsh/profiles/superagent/cordis.patch.yml`，其余设置都在面板里改。

## 参考

- 面板：<http://127.0.0.1:3082>
- 服务脚本：`dsh-superagent-prototype/scripts/dsh-superagent {start,stop,status,restart}`
- 文档：dsh-superagent 仓库 `docs/000-philosophy.md` … `docs/008-cookbook.md`
