# Roberto Rodriguez Rodriguez Draft Workflow

Mandatory local entrypoint. Read [README.md](README.md), then [draft-repo.config.json](draft-repo.config.json), [site-config.json](site-config.json), and only task-relevant page JSON. For visual work, read [docs/brain-mascot-prompt-template.md](docs/brain-mascot-prompt-template.md). Open [changelog/README.md](changelog/README.md) only for history. `Codex.md` is a compatibility pointer.

## Workflow

- Treat this as an independent repository. Pull with `--ff-only` only when clean; report dirty, detached, or unexpected branch state before changes.
- Work on `dev`; promote with separate PRs `dev -> test -> main`. `dev` does not deploy; merged `test` and `main` do.
- Runtime JSON is authoritative. Do not alter clinical claims, content, imagery, routes, analytics, or app code without task-specific evidence.
- Registry version 1 verifies only canonical `robertorodriguezrodriguez.com.mx`; it has no production/test alias fields. `site-config.json` currently has no aliases. Never infer or copy them.
- `draft-repo.config.json` owns the current authoring endpoint. Do not normalize, replace, or copy its legacy Lambda URL without verified service ownership and environment evidence.

## Safety And Validation

- Roberto does not authorize AI-generated images depicting his face or likeness. Use approved stock/abstract imagery or the linked brain mascot template; do not add generic copied AI assets.
- Treat this repository as public. Run hub public-safety with full history before PR, merge, visibility changes, or publication; resolve every blocker.
- Never commit secrets, signed URLs, raw environment values, PII, private source material, databases, logs, credentials, or agent state. Public contact details must be intentionally client-facing.
- Keep `ai_notes/`, `findings/`, `errors-reports/`, and `.superpowers/` ignored. Keep GitHub OIDC and environment-scoped roles; never add long-lived AWS keys or weaken release guards.
- Documentation-only changes require links, workflows, JSON, and public-safety checks. Payload or rendered changes also require desktop/mobile browser QA on every affected route.
- Audit, fix, and rerun relevant checks three times.

Shared procedures: [lifecycle](https://github.com/LynxPardelle/zoolandingpage/blob/main/docs/11-draft-lifecycle.md), [assets](https://github.com/LynxPardelle/zoolandingpage/blob/main/docs/12-public-assets-and-file-uploads.md), [aliases](https://github.com/LynxPardelle/zoolandingpage/blob/main/docs/13-managed-alias-front-door.md), and [fleet ownership](https://github.com/LynxPardelle/zoolandingpage/blob/main/docs/repository-map.md). Keep chronology in `changelog/`, not here.
