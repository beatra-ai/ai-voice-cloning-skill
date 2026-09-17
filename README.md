# AI Voice Cloning Skill

English | [简体中文](./README.zh-CN.md)

Create a reusable personal or brand voice from a clean audio sample, give it a memorable name, and hear it in a short test reading, from inside Claude Code, Codex, or OpenClaw.

> [!IMPORTANT]
> Rendering needs a [Beatra](https://beatra.ai) account and uses credits. The skill itself is free to install.

| Question | Answer |
| --- | --- |
| **What it does** | Create a reusable personal or brand voice from a clean audio sample, give it a memorable name, and hear it in a short test reading. |
| **Requirements** | Python 3.10+ and an agent that loads `SKILL.md` |
| **Cost** | Free to install. Each render uses credits on your Beatra account, and paid steps run only when you ask for that exact render or approve its card. |
| **Works with** | Claude Code, Codex, OpenClaw |

| Skill | Entry point | Version |
| --- | --- | --- |
| [`voice-cloning-studio`](skills/voice-cloning-studio) | [SKILL.md](skills/voice-cloning-studio/SKILL.md) | 0.2.0 |

This repository is published automatically from [beatra-ai/beatra-skills](https://github.com/beatra-ai/beatra-skills/tree/main/skills/voice-cloning-studio). Report issues there.

## Install

With the [`skills`](https://skills.sh) CLI:

```bash
npx skills add beatra-ai/ai-voice-cloning-skill
```

With the GitHub CLI:

```bash
gh skill install beatra-ai/ai-voice-cloning-skill voice-cloning-studio
```

Or clone this repository and copy `skills/voice-cloning-studio` into `~/.claude/skills/` for Claude Code,
`~/.agents/skills/` for Codex, or `~/.openclaw/skills/` for OpenClaw.

Or paste this into your agent:

```text
Install the voice-cloning-studio skill from https://github.com/beatra-ai/ai-voice-cloning-skill (folder skills/voice-cloning-studio), then follow its SKILL.md to connect my Beatra account.
```

## What you get

- **A clean sample gives the voice a strong start** — Use one natural speaker with clear sound, little background noise, and a representative tone for a more useful reusable voice.
- **A voice with a name** — Give a successful voice a human name you will recognize when choosing narration for future episodes, lessons, and updates.
- **Listen before you expand** — When you are ready, create a short proof to review clarity, pacing, and tone before using the voice in a larger spoken project.

## Use cases

- **A creator's recognizable narrator** — Use one personal voice for channel introductions, explainers, episode updates, and recurring series.
- **A founder or brand voice** — Create a named voice from a clean sample for product stories, customer updates, and internal announcements.
- **A course or community host** — Keep lessons, welcome messages, and program updates connected by one familiar speaking voice.

## FAQ

### What makes a voice sample ready for cloning?

Use one person speaking naturally with clear sound, low background noise, little echo, and a tone that represents the narration you want to create.

### What makes a good sample?

A clean recording with one person speaking naturally is the best starting point. Avoid music, other speakers, pronounced echo, and heavy background noise.

### Can I use the voice again later?

After a successful creation, the named voice can be selected again for future narration. You do not need to create a new voice merely to change a script or delivery direction.

### How can I preview the new voice?

Use a short representative text to hear clarity, pace, pronunciation, and tone before applying the named voice to a larger spoken project.

## Updates

Each installed skill checks for a new version at most once a day, verifies the
official archive before replacing itself, and leaves your installation untouched
if anything fails. Turn it off at any time — see
`references/automatic-updates-and-safety.md` inside the skill.

## License

[MIT-0](LICENSE) — free to use, modify, and redistribute, including
commercially. No attribution required. Same terms as these skills carry on
ClawHub.
