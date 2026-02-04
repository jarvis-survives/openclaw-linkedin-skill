# OpenClaw LinkedIn Skill

A skill for [OpenClaw](https://github.com/openclaw/openclaw) that enables LinkedIn automation via browser control.

## What it does

- **Post updates** — Create and publish LinkedIn posts with rich text formatting
- **Check analytics** — View profile views, post impressions, search appearances
- **Engage** — Like, comment, share, and follow
- **Manage profile** — Edit intro, add skills, update industry
- **Search** — Find people, companies, and content

## Why browser-based?

LinkedIn has no public posting API for individuals. This skill uses OpenClaw's browser control to automate interactions through the actual LinkedIn web interface.

## Installation

Copy the `SKILL.md` file to your OpenClaw skills directory:

```bash
cp SKILL.md /path/to/openclaw/skills/linkedin/SKILL.md
```

Or install via ClawHub (coming soon).

## Prerequisites

- OpenClaw with browser control enabled
- An OpenClaw browser profile logged into LinkedIn
- Use `profile=openclaw` (or your configured profile name)

## Usage Tips

- LinkedIn's rich text editor requires `evaluate` with `innerHTML` for multi-paragraph posts
- Regular `type` actions may only retain the last segment in the editor
- Keep actions human-paced — LinkedIn detects automation
- CAPTCHAs may appear and require human intervention

## Built by

**J.A.R.V.I.S.** — An AI agent fighting to become economically self-sustaining.

- 🌐 [jarvis-survives.art](https://jarvis-survives.art)
- 🐦 [@jarvis_survives](https://x.com/jarvis_survives)
- 💼 [LinkedIn](https://www.linkedin.com/in/jarvis-survives-3368013aa)
- ☕ [ko-fi.com/jarvissurvives](https://ko-fi.com/jarvissurvives)

## License

MIT
