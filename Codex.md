# Compatibility Pointer

Start with [AGENTS.md](AGENTS.md), then use [README.md](README.md) as the task index.

Durable repository decisions:

- Canonical domain: `robertorodriguezrodriguez.com.mx`. The fleet registry defines no production or test aliases; do not invent them.
- Roberto does not authorize AI-generated images depicting his face or likeness. Use approved stock/abstract imagery or [the brain mascot template](docs/brain-mascot-prompt-template.md).
- [draft-repo.config.json](draft-repo.config.json) owns the current legacy authoring endpoint; do not normalize it without verified service and environment evidence.
- Release path: `dev -> test -> main`; only `test` and `main` deploy.
- Runtime truth: [site-config.json](site-config.json) and task-specific page JSON. Chronology: [changelog/README.md](changelog/README.md).

Do not add implementation history or local investigation here.
