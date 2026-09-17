# AI Voice Cloning Skill

[English](./README.md) | 简体中文

用干净的语音样本创建可复用的个人或品牌声音，为音色命名，并通过短句试听清晰度、节奏与语气，在 Claude Code、Codex 或 OpenClaw 里直接完成。

> [!IMPORTANT]
> 生成需要 [Beatra](https://beatra.ai) 账号并消耗积分，安装本身不收费。

| 问题 | 回答 |
| --- | --- |
| **能做什么** | 用干净语音样本创建可复用的个人或品牌声音，为音色命名，并通过短句试听清晰度、节奏与语气。 |
| **运行要求** | Python 3.10+，以及能加载 `SKILL.md` 的 Agent |
| **费用** | 安装免费。每次生成消耗 Beatra 账号积分，只有你明确要求这次生成或批准确认卡后才会付费。 |
| **支持的 Agent** | Claude Code、Codex、OpenClaw |

| Skill | Entry point | Version |
| --- | --- | --- |
| [`voice-cloning-studio`](skills/voice-cloning-studio) | [SKILL.md](skills/voice-cloning-studio/SKILL.md) | 0.2.0 |

本仓库由 [beatra-ai/beatra-skills](https://github.com/beatra-ai/beatra-skills/tree/main/skills/voice-cloning-studio) 自动发布，问题请到那里反馈。

## 安装

使用 [`skills`](https://skills.sh) CLI：

```bash
npx skills add beatra-ai/ai-voice-cloning-skill
```

使用 GitHub CLI：

```bash
gh skill install beatra-ai/ai-voice-cloning-skill voice-cloning-studio
```

也可以克隆本仓库，把 `skills/voice-cloning-studio` 复制到 `~/.claude/skills/`（Claude Code）、`~/.agents/skills/`（Codex）或 `~/.openclaw/skills/`（OpenClaw）。

或者把下面这段话发给你的 Agent：

```text
从 https://github.com/beatra-ai/ai-voice-cloning-skill 安装 voice-cloning-studio skill（目录 skills/voice-cloning-studio），然后按它的 SKILL.md 连接我的 Beatra 账号。
```

## 你能得到什么

- **干净样本带来更好的声音起点** — 选择单人自然说话、背景安静、回声较少且语气有代表性的录音，方便创建更实用的可复用音色。
- **给声音取一个认得出的名字** — 为成功创建的音色命名，之后为节目、课程和更新选择旁白时更容易找到它。
- **先听短句，再决定下一步** — 准备好时，用一段简短口播检查清晰度、节奏和语气，再用到更大的内容项目里。

## 适用场景

- **创作者的固定旁白** — 为频道开场、讲解视频、节目更新和系列内容保留一个熟悉的个人声音。
- **创始人或品牌声音** — 用干净样本创建有名字的音色，用于产品故事、客户更新和内部通知。
- **课程与社群主持人** — 让课程讲解、欢迎词和活动更新都由同一个熟悉的声音表达。

## 常见问题

### 什么样的语音样本适合声音克隆？

选择一位说话者自然表达、声音清楚、背景噪音低、回声少，并能代表未来旁白语气的录音。

### 什么样的样本更合适？

单人自然说话、声音清晰的录音更合适。请避开音乐、其他人声、明显回声和重度背景噪音。

### 以后还可以继续使用这个音色吗？

成功创建后，可以在后续旁白中再次选择这个有名字的音色。修改文案或表达方式时，不需要重新创建同一种声音。

### 怎样试听刚创建的音色？

用一段有代表性的短文案试听清晰度、读音、节奏与语气，再把有名字的音色用于更大的口播项目。

## 更新

安装后的 skill 每天最多检查一次新版本，替换前先校验官方归档，任何一步失败都不会动你已安装的版本。
随时可以关闭，见 skill 内的 `references/automatic-updates-and-safety.md`。

## 许可证

[MIT-0](LICENSE)：可自由使用、修改和再分发，包括商用，无需署名；与这些 skill 在 ClawHub 上的条款一致。
