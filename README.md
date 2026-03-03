# LLM Skills

A collection of structured skill files for Claude Code and other LLM tools. Each skill is a set of plain-text instructions and reference documents that load frameworks into an AI conversation, shaping how it thinks about a domain.

These aren't apps or libraries. They're config files — English-language instructions that turn a general-purpose AI into a more useful thinking partner for specific tasks.

## Skills

### [Medical Research Thinking Partner](claude-code/medical-research/)

A structured thinking partner for navigating medical information. Loads evidence-based medicine frameworks — PICO question framing, evidence hierarchy evaluation, statistics translation (relative vs. absolute risk, NNT), and appointment prep scaffolding — into a Claude conversation.

**What it does:** Helps you evaluate medical evidence and ask better questions. Not a diagnostician.

**What it doesn't do:** Diagnose, prescribe, or replace clinical judgment.

## Installation (Claude Code)

1. Clone or download this repo
2. Copy the skill directory into your Claude Code skills folder:
   ```bash
   cp -r claude-code/medical-research ~/.claude/skills/medical-research
   ```
3. The skill activates automatically when you ask Claude Code about medical topics, or you can invoke it directly with `/medical-research`

## License

This repo uses dual licensing:

- **Skill orchestration files** (`SKILL.md`) are licensed under the [MIT License](LICENSE-MIT) — use, modify, and redistribute freely.
- **Reference documents** (`references/`) are licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSE-CC-BY-4.0) — use, adapt, and share freely with attribution.

See individual license files for full terms.

## About

Built by [Matthew @ idka.info](https://idka.info) — a blog called "I Don't Know Anything." These skills grew out of practical need: wanting an AI that helps me think more clearly about specific domains rather than just answering questions.

Blog post about the medical research skill: *(coming soon)*
