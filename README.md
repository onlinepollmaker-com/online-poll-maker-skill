# Online Poll Maker — AI agent skill

Let your AI agent create polls for you on [Online Poll Maker](https://onlinepollmaker.com): free, no sign-up, 1–100 single-choice questions, share a link and see results.

You tell the agent what you want to ask. It writes the questions and options, creates a **draft**, and gives you a link. You open the link, adjust anything, verify and publish in your browser. The agent never publishes for you and never gets the management link.

[中文说明](#中文)

## Install

**Easiest: let your agent do it.** Send this to an agent that supports skills (for example Claude Code):

> Install the online-poll-maker skill from https://github.com/onlinepollmaker-com/online-poll-maker-skill (the file is `skills/online-poll-maker/SKILL.md`).

**Manually:** copy the `skills/online-poll-maker` folder into your agent's skills directory. For Claude Code that is `~/.claude/skills/online-poll-maker/`.

**Apps where you upload skills in settings:** download [online-poll-maker.zip](https://onlinepollmaker.com/skill/online-poll-maker.zip) and upload it.

**No install needed:** you can also just paste this prompt into any agent that can browse the web:

> Read and follow https://onlinepollmaker.com/agents.md to help me create a poll on Online Poll Maker. Ask me what the poll is about.

## Use

After installing, just ask: *"Make a poll for my team: where should we eat on Friday — tacos, sushi or pizza?"*

## What the agent can and can't do

- **Can:** create a draft, read the edits you make in the browser, and update the draft.
- **Can't:** publish, skip the human verification, get the management link, or change a published poll.
- Draft links work for 24 hours. Polls stay open for 30 days, and results are kept for 90 days after closing.

## How it works

The skill is a thin pointer. It tells the agent to read the official [agent guide](https://onlinepollmaker.com/agents.md) and the [OpenAPI document](https://onlinepollmaker.com/api/openapi.json) every time, so rule and API changes reach your agent without updating the skill. The skill contains no credentials.

## Links

- Website: https://onlinepollmaker.com
- Agent guide: https://onlinepollmaker.com/agents.md
- Contact: hi@onlinepollmaker.com

---

## 中文

让 AI 助手帮你在 [在线投票制作（Online Poll Maker）](https://onlinepollmaker.com/zh/) 上创建投票：免费、无需注册，支持 1～100 道单选题，分享链接即可收集投票、查看结果。

你告诉助手想问什么，它会整理题目和选项，创建一份**草稿**并给你链接。你打开链接检查、修改，完成验证后在浏览器里发布。助手不能替你发布，也拿不到管理链接。

### 安装

**最简单：让助手自己装。** 把这句话发给支持 Skill 的助手（例如 Claude Code）：

> 请从 https://github.com/onlinepollmaker-com/online-poll-maker-skill 安装 online-poll-maker 这个 Skill（文件是 `skills/online-poll-maker/SKILL.md`）。

**手动安装：** 把 `skills/online-poll-maker` 文件夹复制到助手的 Skill 目录。Claude Code 是 `~/.claude/skills/online-poll-maker/`。

**只能在设置里上传 Skill 的应用：** 下载 [online-poll-maker.zip](https://onlinepollmaker.com/skill/online-poll-maker.zip) 后上传。

**不安装也能用：** 把下面这句提示词粘贴给任何能上网的助手：

> 请阅读并按照 https://onlinepollmaker.com/agents.md 帮我在 Online Poll Maker 上创建一个投票。先问我想做什么投票。

### 使用

安装后直接说：*"帮我做个投票：周五团建吃什么，火锅、烧烤还是日料？"*

### 助手能做什么

- **能：** 创建草稿、读取你在网页上的修改、更新草稿。
- **不能：** 发布投票、跳过人机验证、取得管理链接、修改已发布的投票。
- 草稿链接 24 小时有效；投票开放 30 天，关闭后结果保留 90 天。

### 工作方式

Skill 只是一个很薄的入口：它让助手每次都去读官方 [Agent 指引](https://onlinepollmaker.com/agents.md) 和 [OpenAPI 文档](https://onlinepollmaker.com/api/openapi.json)，所以规则和接口更新后，不需要更新 Skill。Skill 不包含任何凭证。

## License

MIT
