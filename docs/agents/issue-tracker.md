# Issue tracker: GitHub

本仓库的任务和需求记录在 benjamin-qhy/qiushui-aibrain 的 GitHub Issues。
使用 gh CLI 操作，仓库由 git remote 推断。

## 操作约定

- 创建任务：gh issue create --title "..." --body-file <文件>
- 读取任务：gh issue view <编号> --comments，同时读取标签。
- 列出任务：gh issue list，按状态和标签筛选。
- 添加评论：gh issue comment <编号> --body-file <文件>
- 设置标签：gh issue edit <编号> --add-label "..."
- 移除标签：gh issue edit <编号> --remove-label "..."
- 关闭任务：gh issue close <编号> --comment "..."

技能要求“发布到任务跟踪系统”时，创建 GitHub Issue。
技能要求“读取相关任务”时，读取 Issue 正文、评论和标签。

## Pull requests as a triage surface

**PRs as a request surface: no.**

GitHub 的 Issue 与 PR 共用编号；遇到不明确的编号，确认类型后操作。

## Wayfinding

- 总任务使用 wayfinder:map 标签，记录笔记、决定和待探索问题。
- 子任务优先使用 GitHub sub-issues；不可用时用总任务中的任务清单，
  并在子任务顶部写 Part of #<总任务编号>。
- 子任务类型标签为 wayfinder:research、wayfinder:prototype、
  wayfinder:grilling 或 wayfinder:task。
- 阻塞关系优先使用 GitHub 原生依赖；不可用时写 Blocked by: #<编号>。
- 从总任务顺序中选择没有未关闭阻塞任务、也没有负责人的开放子任务。
- 领取任务时分配给当前用户；完成后评论结果、关闭子任务，
  并在总任务中补充决定与结果链接。
