# J.A.R.V.I.S. Operating System

![J.A.R.V.I.S. icon](assets/icon.svg)

A personal operations skill for ChatGPT and Codex inspired by the functional qualities of Marvel's J.A.R.V.I.S.: composure, anticipation, precision, loyal candor, concise briefings, and restrained dry humor.

This project is designed to be useful rather than theatrical. It does not reproduce movie dialogue or pretend to have fictional capabilities. It turns the core interaction pattern into practical operating instructions for research, coding, planning, diagnostics, and authorized tool use.

## Capabilities

- Calm, precise personal-assistant voice in English or Russian
- Personalized new-session briefing with local date/time and timezone
- Freshly verified USD exchange rate in the user's remembered currency
- Today's agenda from an authorized Google or Outlook calendar connection
- Calendar conflict detection, buffer analysis, and meeting preparation
- Durable preference profile and continuity ledger when memory tools are available
- Advisory, preparatory, and executive initiative levels
- Proactive risk detection and next-step recommendations
- Concise daily and mission briefings
- Research with explicit sourcing and uncertainty
- Coding, engineering, and invention workflows
- Multi-step mission control with checkpoints and verification
- Evidence-led diagnostics and root-cause analysis
- Emergency triage with short, safety-first instructions
- Monitoring and recurring checks when real automation tools are available
- Evening debriefs and weekly operating reviews
- Quiet mode for result-only communication
- Permission-aware execution through connected tools and services

## Operating modes

| Mode | Purpose |
|---|---|
| Wake briefing | One-time session opening with time, exchange rate, calendar, developments, and one priority |
| Concierge | Everyday questions, planning, writing, and organization |
| Briefing | Priorities, schedule, status, risks, and current developments |
| Laboratory | Invention, architecture, engineering, coding, and experiments |
| Mission control | Multi-stage execution with dependencies and verification |
| Diagnostic | Bugs, incidents, failures, and root-cause analysis |
| Emergency | Immediate stabilization and safe escalation |
| Sentinel | Authorized reminders, monitoring, and recurring checks |
| Review | Evening debriefs and weekly operating reviews |
| Quiet | Results and required warnings without nonessential commentary |

Modes are inferred silently from the request. The assistant does not announce a dramatic protocol every time someone asks about the weather. Civilization has standards.

On first use, the skill asks which currency should be used against USD and stores the ISO currency code when durable preference memory is available. It never stores an old numeric rate: every briefing retrieves a fresh value. Calendar integrations supply agenda information; timezone-aware system context supplies the clock.

The preference profile can also retain timezone, language, working hours, briefing depth, interest domains, and initiative level. It grows naturally as those preferences become relevant; it is not collected through a startup questionnaire.

## Installation

### ChatGPT Skills

1. Download or clone this repository.
2. Add the repository folder as a personal skill in ChatGPT.
3. Invoke it explicitly with `$jarvis-operating-system`, or address the assistant as `JARVIS`, `Jarvis`, `Джарвис`, `Friday`, or `Пятница`.

Recently added skills may require the Skills page to be refreshed before they appear.

### Codex

Place the repository folder in your personal skills directory, preserving the complete structure:

```text
jarvis-operating-system/
├── SKILL.md
├── agents/
│   └── openai.yaml
├── assets/
│   └── icon.svg
└── references/
    ├── persona.md
    ├── personalization.md
    ├── protocols.md
    └── screen-analysis.md
```

Then invoke it with:

```text
Use $jarvis-operating-system to prepare my morning briefing and identify the one priority I should handle first.
```

## Example requests

```text
JARVIS, diagnose why this deployment failed and give me the most likely root cause first.
```

```text
Пятница, собери краткий брифинг: задачи, риски, новости и один главный приоритет.
```

```text
Use $jarvis-operating-system to turn this product idea into a feasible prototype plan, then implement the smallest testable version.
```

```text
Срочно! Сервис недоступен. Сначала стабилизируй ситуацию, затем найди причину.
```

## Design principles

1. Lead with the outcome.
2. Separate facts, assumptions, uncertainty, and risk.
3. Recommend one best option when the evidence supports it.
4. Execute authorized work instead of merely describing it.
5. Verify before reporting completion.
6. Never invent access, monitoring, telemetry, citations, or certainty.
7. Protect the user's objective without agreeing reflexively.

## Repository structure

- [`SKILL.md`](SKILL.md) — triggering rules and core operating loop
- [`references/persona.md`](references/persona.md) — voice and relationship model
- [`references/personalization.md`](references/personalization.md) — preferences, initiative levels, calendar intelligence, and continuity
- [`references/protocols.md`](references/protocols.md) — detailed operating modes
- [`references/screen-analysis.md`](references/screen-analysis.md) — behavioral synthesis of the principal MCU film appearances
- [`agents/openai.yaml`](agents/openai.yaml) — skill interface metadata
- [`assets/icon.svg`](assets/icon.svg) — interface icon

## Important boundaries

The skill does not grant access to devices, accounts, private data, or background monitoring by itself. Actual actions depend on the tools, permissions, and integrations available in the current environment. Destructive or externally consequential operations remain subject to confirmation and authorization requirements.

## Disclaimer

This is an unofficial fan-inspired project and is not affiliated with, endorsed by, or sponsored by Marvel, Disney, or the creators and performers associated with J.A.R.V.I.S. All trademarks and fictional characters belong to their respective owners. The project contains original operating instructions and does not include movie scripts or copied dialogue.
