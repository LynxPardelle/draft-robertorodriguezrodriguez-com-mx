# Roberto Rodriguez Rodriguez Draft

Portable Zoolandingpage draft config for `robertorodriguezrodriguez.com.mx`.

## Workflow

- Work on `dev`.
- Promote `dev -> test` to publish the test environment.
- Promote `test -> main` to publish production.
- Do not commit secrets, credentials, local source documents, private notes, logs, or generated reports.

## Preview

Test preview uses the shared testing host:

```text
https://test.zoolandingpage.com.mx/?draftDomain=test.robertorodriguezrodriguez.zoolandingpage.com.mx&debugWorkspace=false
```

The `test.robertorodriguezrodriguez.zoolandingpage.com.mx` value is a runtime test alias declared in `site-config.json`; it lets the shared testing host resolve the test published pointer without publishing production.

CTAs stay neutral until a public contact channel is explicitly approved.
