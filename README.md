# Draft: robertorodriguezrodriguez.com.mx

<!-- zoolanding-hub-routing:start -->
## Zoolanding Knowledge Router

Shared procedures are routed through the Zoolandingpage hub. Start with [AGENTS.md](AGENTS.md) and open only the document needed for the current task.

| Task | Read |
| --- | --- |
| Edit draft content or routes | Local `site-config.json`, page JSON, and task-specific local docs |
| Create or bootstrap a draft | [ai-notes/how-to/create-secure-draft-repo.md](https://github.com/LynxPardelle/zoolandingpage/blob/main/ai-notes/how-to/create-secure-draft-repo.md) |
| Promote, deploy, or configure branches | [Hub lifecycle guide and local `.github/workflows/`](https://github.com/LynxPardelle/zoolandingpage/blob/main/docs/11-draft-lifecycle.md) |
| Upload public assets | [docs/12-public-assets-and-file-uploads.md](https://github.com/LynxPardelle/zoolandingpage/blob/main/docs/12-public-assets-and-file-uploads.md) |
| Configure domains or aliases | [docs/13-managed-alias-front-door.md](https://github.com/LynxPardelle/zoolandingpage/blob/main/docs/13-managed-alias-front-door.md) |
| Work across repositories | [docs/repository-map.md](https://github.com/LynxPardelle/zoolandingpage/blob/main/docs/repository-map.md) |

Critical repository-specific safety, deployment, and rollback rules remain local.
<!-- zoolanding-hub-routing:end -->

Sanitized public source for the Zoolanding draft at `drafts/robertorodriguezrodriguez.com.mx`.

## Start Here

| Task | Source |
| --- | --- |
| Safety, workflow, and closeout | [AGENTS.md](AGENTS.md) |
| Domain, environments, endpoint, and GitHub variables | [draft-repo.config.json](draft-repo.config.json) |
| Routes, canonical origin, and runtime settings | [site-config.json](site-config.json) |
| Page content | `{pageId}/page-config.json`, `{pageId}/components.json`, `{pageId}/variables.json`, and `{pageId}/i18n/` |
| Approved visual mascot guidance | [docs/brain-mascot-prompt-template.md](docs/brain-mascot-prompt-template.md) |
| Deployment implementation | [tools/deploy-draft.mjs](tools/deploy-draft.mjs) and [.github/workflows/](.github/workflows/) |
| Repository chronology | [changelog/README.md](changelog/README.md) |

Shared authoring, safety, asset, and alias guidance lives in the [Zoolandingpage documentation hub](https://github.com/LynxPardelle/zoolandingpage/blob/main/docs/README.md).

## Domain And Release Contract

The [fleet registry](https://github.com/LynxPardelle/zoolandingpage/blob/main/docs/drafts-registry.json) verifies `robertorodriguezrodriguez.com.mx` as this repository's canonical domain. Registry version 1 has no production- or test-alias fields, and `site-config.json` currently declares an empty alias list. No test alias is declared; do not reuse or infer an unregistered hostname.

`draft-repo.config.json` retains the existing Lambda authoring endpoint. This repository owns that configured value, but changing or normalizing it requires verified service ownership and environment evidence.

Work lands on `dev`; it does not deploy. Separate merged PRs promote `dev -> test -> main`. GitHub Actions use OIDC; do not add long-lived AWS credentials. CTAs stay neutral until a public contact channel is explicitly approved.

Local-only notes, findings, logs, environment files, private source material, and agent state remain ignored. Documentation-only changes do not require visual QA; payload or rendered changes do.
