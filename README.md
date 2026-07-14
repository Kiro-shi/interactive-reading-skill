# Interactive Reading Skill

Codex skill for turning books, chapters, papers, courses, transcripts, meeting notes, and other static material into an interactive mastery workflow.

## Quick Start

Give this repository link to your Codex agent and ask it to install the skill:

```text
Please install this Codex skill:
https://github.com/Kiro-shi/interactive-reading-skill

Use $skill-installer. The skill path inside the repo is interactive-reading.
```

The agent should install the `interactive-reading` folder from this repository into your local Codex skills directory. After installation, start a new turn or restart Codex if the skill does not appear immediately.

Then invoke it with:

```text
$interactive-reading
```

Example:

```text
Use $interactive-reading to turn this book into an interactive study workflow.
```

## Installer Command

In Codex, ask:

```text
Use $skill-installer to install the interactive-reading skill from Kiro-shi/interactive-reading-skill, path interactive-reading.
```

If you want to pin an exact version, ask your agent to install a specific commit hash:

```text
Use $skill-installer to install the interactive-reading skill from Kiro-shi/interactive-reading-skill, path interactive-reading, ref <commit-hash>.
```

## Manual Install

Copy the `interactive-reading` folder into your Codex skills directory:

```text
~/.codex/skills/interactive-reading
```

The skill folder must contain `SKILL.md` at its root.
