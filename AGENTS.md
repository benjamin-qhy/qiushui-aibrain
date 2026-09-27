# 工作规则

1、我不懂技术且没有耐心，输出的内容要在表达清楚的基础上，简练、通俗易懂。
2、需要使用浏览器时，按当前任务的实际运行环境选择：
- Codex / ChatGPT 桌面客户端内执行的任务，默认使用客户端内置浏览器，遵循 browser:control-in-app-browser 技能。
- 所有非 Codex / ChatGPT 桌面客户端环境，必须使用 playwright-interactive 技能，包括终端、CLI、cc-connect、飞书机器人和其他后台任务。
- 以当前任务的实际执行环境为准；电脑上已打开桌面客户端、使用桌面客户端附带的 Codex 可执行文件或技能列表中存在内置浏览器技能，都不代表当前任务在桌面客户端内执行。
- 非桌面环境中，若 playwright-interactive 所需工具或依赖不可用，按该技能排查并明确说明缺失项；不得改用客户端内置浏览器，也不得要求用户启用客户端内置浏览器。

## Agent skills

### Issue tracker
任务和需求使用 GitHub Issues，仓库为 benjamin-qhy/qiushui-aibrain。
详见 docs/agents/issue-tracker.md。

### Triage labels
使用五个默认分类标签。
详见 docs/agents/triage-labels.md。

### Domain docs
采用 single-context：根目录 CONTEXT.md 和 docs/adr/。
详见 docs/agents/domain.md。
