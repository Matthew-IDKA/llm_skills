# Medical Research Thinking Partner

A Claude Code skill that turns AI into a structured thinking partner for navigating medical information. It loads evidence-based medicine frameworks into the conversation so you can evaluate research, understand statistics, and prepare for appointments more effectively.

**This is not a diagnosis tool.** It helps you ask better questions — it doesn't replace a doctor.

## What's included

```
medical-research/
├── SKILL.md                          # Main skill file (orchestrator)
└── references/
    ├── evidence-hierarchy.md         # How to evaluate study quality (systematic reviews → case reports)
    ├── statistics-primer.md          # Translating medical statistics (relative vs. absolute risk, NNT, p-values)
    ├── source-routing.md             # Trusted sources by condition type (NIH, Cochrane, NCCN, etc.)
    └── appointment-prep.md           # Appointment prep scaffold, teach-back method, second opinion guidance
```

## Installation

Copy this directory into your Claude Code skills folder:

```bash
cp -r medical-research ~/.claude/skills/medical-research
```

## Usage

The skill activates automatically when you bring a medical question to Claude Code, or invoke it directly:

```
/medical-research statin risks and benefits
```

### Modes

The skill adapts its approach based on your situation:

1. **New diagnosis** — understand what it means, severity, treatment landscape
2. **Chronic condition** — management goals, monitoring, quality of life
3. **Acute symptom** — red flags vs. watchful waiting, when to escalate
4. **Research a treatment** — evaluate evidence quality, translate statistics
5. **Appointment prep** — build a prioritized question list, teach-back prompts
6. **Interpret results** — translate test results and imaging reports

### Key frameworks

- **PICO** — structures your question into Patient, Intervention, Comparison, and Outcome so you can research it precisely
- **Evidence hierarchy** — ranks sources from systematic reviews (strongest) to expert opinion (weakest)
- **NNT/NNH** — Number Needed to Treat / Harm — how many people take a treatment for one to benefit or be harmed
- **Cognitive traps** — flags common reasoning errors: relative risk inflation, anecdote over evidence, surrogate endpoint confusion

## Example

> "My doctor wants to put me on a statin. How do I think about whether that's right for me?"

The skill will:
1. Reframe using PICO (what's your specific risk profile? which statin? compared to what? what outcome matters to you?)
2. Help you find the relevant evidence tier
3. Translate the statistics (what's the NNT for your risk level?)
4. Build a question list for your next appointment
5. Coach you on how to present your research collaboratively

## License

- `SKILL.md` — [MIT License](../../LICENSE-MIT)
- `references/*` — [CC BY 4.0](../../LICENSE-CC-BY-4.0)
