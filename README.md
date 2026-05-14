# papiflyfx-docking-core

Extracted from the PapiflyFX Docking monorepo.

## Modules

- `papiflyfx-docking-api`
- `papiflyfx-docking-docks`

## Build

Use the split-local Maven repository so cross-repo snapshots resolve from the extraction workspace:

```bash
./mvnw -Dmaven.repo.local=$HOME/github/papiflyfx/.m2-split -Dtestfx.headless=true clean verify
```

Lead agent: `@core-architect`.

## Notes

- `papiflyfx-docking-docks` keeps its same-repository dependency on `papiflyfx-docking-api` at `${project.version}`.
