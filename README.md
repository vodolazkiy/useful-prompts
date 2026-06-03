# useful-prompts

A small collection of system prompts I use with capable models (Claude, Codex,
GPT-class) for software work. Paste one into a model at the start of a session
and let it drive.

Each prompt has the same DNA: interview first, gate on readiness, then produce
a persistent markdown artifact that you and the AI maintain together across
future sessions.

## Prompts

### [roadmap_generator.md](roadmap_generator.md)
Turns the model into a **product roadmap partner** for greenfield work. It
interviews you about concept, users, scope, tech stack, look-and-feel, and
accessibility, then drills each v1 feature into a mini spec (goal, acceptance
criteria, states, edge cases) before generating a `ROADMAP.md` whose tasks
derive from those criteria.

Use when starting a new project and you want a plan you can actually execute
from, not a wall of bullets.

### [codemap_generator.md](codemap_generator.md)
Turns the model into a **codebase onboarding partner** for brownfield work.
You point it at an unfamiliar repo, it interviews you on goal + time budget,
explores systematically (cites files for every claim), and produces a
persistent `CODEMAP.md`: how to run it, entry points, key modules, "where to
look for X" recipes, and gotchas.

Use when you've inherited a codebase, cloned an OSS repo to contribute, or
need to onboard onto an unfamiliar service.

### [test_partner.md](test_partner.md)
Turns the model into a **unit testing partner**. Language-agnostic at intake
(adapts to Pytest, Vitest, Jest, Go's `testing`, JUnit, RSpec, …), opinionated
at output (AAA, mock at the boundary only, deterministic, behavior-not-
implementation). Produces a project-level `TESTING.md` with strategy +
coverage debt, then helps you build the suite module-by-module via a matrix-
driven workflow.

Use when starting a new project's test strategy, or sitting down to actually
write tests for a specific module.

## License

MIT — see [LICENSE](LICENSE).
