# Hiring Council (Claude Code prototype)

A multi-agent hiring council. Six evaluator seats with declared biases argue
about a candidate; a Fact Checker keeps citations honest; a Chair rules.
The main Claude Code session is the orchestrator and the turn-selector.

## Run

1. Put a transformed role in `roles/` (see roles/README.md).
2. Put a candidate packet in `candidates/<name>.md` (see candidates/README.md).
3. `/council roles/<role>.md candidates/<name>.md`
4. Read `sittings/<name>/<timestamp>/transcript.md` and `ruling.json`.

Rerun after new evidence:
`/council-rerun sittings/<name>/<timestamp> candidates/<name>-answers.md`

## Files

- `COMMON_RULES.md` — rules every evaluator seat reads first. Edit here, not in seats.
- `.claude/agents/*.md` — one subagent per seat.
- `.claude/commands/council.md` — the orchestration loop (run as /council).
- `sittings/` — one folder per sitting: transcript.md, state.json, ruling.json.
