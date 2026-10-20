# AI Voice Cloning Skill

English | [简体中文](./README.zh-CN.md) | [日本語](./README.ja.md)

> 👉 See also [AI Voiceover Generator Skill](https://github.com/beatra-ai/ai-voiceover-generator-skill)

Create a reusable personal or brand voice from a clean audio sample, give it a memorable name, and hear it in a short test reading, from inside Claude Code, Cursor, Codex, Windsurf, Cline, or OpenClaw.

> [!IMPORTANT]
> Rendering needs a [Beatra](https://beatra.ai?utm_source=github&utm_medium=flagship&utm_campaign=ai-voice-cloning-skill) account and uses credits. The skill itself is free to install.

| Question | Answer |
| --- | --- |
| **What it does** | Create a reusable personal or brand voice from a clean audio sample, give it a memorable name, and hear it in a short test reading. |
| **Models** | MiniMax Voice Clone, MiniMax Speech 2.8 HD, MiniMax Speech 2.8 Turbo |
| **Requirements** | Python 3.10+ and an agent that loads `SKILL.md` |
| **Cost** | Free to install. Each render uses credits on your Beatra account, and paid steps run only when you ask for that exact render or approve its card. |
| **Works with** | Claude Code, Cursor, Codex, Windsurf, Cline, OpenClaw |

<p align="center"><img src="assets/cover.webp" width="800" alt="Abstract cover showing a single voice waveform passing through a ring and returning as a reusable layered voice. AI-generated with Beatra."></p>

*Abstract cover showing a single voice waveform passing through a ring and returning as a reusable layered voice. AI-generated with Beatra.*

| Skill | Entry point | Version |
| --- | --- | --- |
| [`voice-cloning-studio`](skills/voice-cloning-studio) | [SKILL.md](skills/voice-cloning-studio/SKILL.md) | 0.3.0 |

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
`~/.cursor/skills/` for Cursor, `~/.agents/skills/` for Codex, `~/.codeium/windsurf/skills/` for Windsurf,
`~/.cline/skills/` for Cline, or `~/.openclaw/skills/` for OpenClaw.

Or paste this into your agent:

```text
Install the voice-cloning-studio skill from https://github.com/beatra-ai/ai-voice-cloning-skill (folder skills/voice-cloning-studio), then follow its SKILL.md to connect my Beatra account.
```

## Examples

<p align="center"><img src="assets/cover.webp" width="800" alt="Abstract cover showing a single voice waveform passing through a ring and returning as a reusable layered voice. AI-generated with Beatra."></p>

[▶ Listen (MP3)](assets/sample.mp3)

*A 23-second synthetic preset-voice reading (first 8 seconds shown) was cloned into a reusable custom voice named Harbor Narrator, followed by an 11-second test reading in that new voice. AI-generated with Beatra.*

Ask your agent:

```text
Clone the voice in ./harbor-sample.mp3 into a reusable voice named Harbor Narrator, then read this test line in it: "The lighthouse keeps its own hours, and so does the tide."
```

Prompt:

```text
Source script: Every harbor town keeps its own kind of morning. The fishing boats slip out before sunrise, the gulls argue over the pier, and the café on the corner props its door open to let the bread smell drift toward the water. By eight o'clock, the tide has turned, the ferry horn sounds twice, and the whole waterfront settles into an easy, unhurried rhythm.

Test reading script: Hello, and welcome back to the Lantern Lane course. In today's lesson, we'll plan a simple weekly routine, one small step at a time. Let's begin.
```

## Technical Specifications & Output Limits

As of 2026-10-18. Live list: https://docs.beatra.ai/en/docs/models

- **Uploads** — up to 100 MB per file; the per-model input limits below also apply
- **Voice cloning** — 1 model (MiniMax Voice Clone); sample 10–300 s, up to 20 MB; consent attestation required
- **Text to speech** — 2 models (MiniMax Speech 2.8 HD, MiniMax Speech 2.8 Turbo); FLAC, MP3, OPUS, PCM, WAV; 40 languages; sample rates 8, 16, 22.05, 24, 32, 44.1 kHz; up to 50000 characters per request
  - Languages (ISO 639 codes): zh, yue, en, es, fr, ru, de, pt, ar, it, ja, ko, id, vi, tr, nl, uk, th, pl, ro, el, cs, fi, hi, bg, da, he, ms, fa, sk, sv, hr, fil, hu, no, sl, ca, nn, ta, af

## Why use Beatra instead of calling model APIs directly

- **One account for every model this skill uses** — Voice cloning 1; Text to speech 2 (MiniMax Voice Clone, MiniMax Speech 2.8 HD, MiniMax Speech 2.8 Turbo) (as of 2026-10-18), behind one Beatra sign-in; no keys from individual model providers to manage.
- **You decide what gets paid for** — Paid renders run only when you ask for that exact render or approve its card, which shows the live credit estimate.
- **Direction before rendering** — the skill plans, directs, and reviews the work, then renders it on Beatra.
- **Files you can verify** — every file under `skills/` matches the release archive on cdn.beatra.ai byte for byte, checked by SHA-256 before each push.
- **Updates you control** — no self-updater; update with the tool you installed it with.
- **Runs in your agent** — Claude Code, Cursor, Codex, Windsurf, Cline, OpenClaw.

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

## Updates and security

Since the 2026-10 release, this skill contains no self-updater: it runs only the
files you installed and never replaces them on its own. Update it with the tool
you installed it with — `npx skills update voice-cloning-studio` or `gh skill update voice-cloning-studio`.
Details: `references/updates-and-security.md` inside the skill.

## License

[MIT-0](LICENSE) — free to use, modify, and redistribute, including
commercially. No attribution required. Same terms as these skills carry on
ClawHub.

## Links

- Website — https://beatra.ai?utm_source=github&utm_medium=flagship&utm_campaign=ai-voice-cloning-skill
- Docs — https://docs.beatra.ai?utm_source=github&utm_medium=flagship&utm_campaign=ai-voice-cloning-skill
- Console — https://console.beatra.ai
- For AI agents — https://beatra.ai/llms.txt (index) · https://beatra.ai/llms-full.txt (every skill in one file)
