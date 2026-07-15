# life-os — a Claude Code skill

A personal **Life OS**: one offline-capable HTML file that is the living
registry/database of your whole life — career, finances, health habits,
family, learning, home admin, personal projects, purpose — rendered as an
interactive node graph, a value/effort matrix, a day-centered cockpit, a
second brain (zero-friction inbox + distilled memory), dated history and
anti-vanity metrics. LLM agents keep it updated daily; Python scripts do
everything mechanical for free.

## Install

```bash
# copy this folder into your Claude Code skills directory:
cp -r life-os ~/.claude/skills/
```

Then in any Claude Code session: **"crea mi life os"** (create) or
**"actualiza mi life os"** (daily loop). The skill is self-contained — the
`template/` folder bundles the engine (UI shell, builder, mechanical CLI), a
buildable seed, fake multi-domain examples, and the full didactic spec
(`template/GUIDE-CLEAN.html`, open it in a browser).

## Core ideas

- **Everything is a node** — themes, bets, tasks, people, topics; days and any
  derivable view are *virtual* nodes (computed from dated records, never stored).
- **Token economy** — mechanical writes go through `update_q3.py` (zero LLM);
  model tokens are spent only on judgment (advice, focus, memory triage).
- **Second brain** — one-line capture → daily triage → distilled memory →
  memory-first advice ("mom hates surprises" shapes the visit plan).
- **Two-kind metrics** — elemental (automatic: completions, streaks, times) +
  custom (LLM-derived from *your* goals); hard cap per domain (anti-vanity).
- **Register once, surface everywhere** — history, node detail, day view, search.

## License

MIT — see [LICENSE](LICENSE).
