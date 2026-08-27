# AGENTS.md

This is a **personal** Mason registry. It follows the same package definition format as the
upstream [mason-registry](https://github.com/mason-org/mason-registry).

## Layout

- `packages/<package-name>/package.yaml` — one file per package.

## Package definition syntax

Do **not** rely on memory for the exact schema. The authoritative specification is the upstream
[mason-registry](https://github.com/mason-org/mason-registry).

If `refs/mason-registry` is not present, clone it first:

```bash
git clone https://github.com/mason-org/mason-registry.git refs/mason-registry
```

Then consult its `CONTRIBUTING.md` for the full package definition spec, field requirements, and
per-ecosystem examples (npm, cargo, GitHub release assets, PyPI, etc.). Follow the same
field names/types as upstream so `mason.nvim` can consume this registry via the `file:` protocol.

## Notes for this personal registry

- Unlike the upstream, the popularity requirements (stars/downloads) do **not** apply; add whatever
  packages you personally need.
- Keep packages in `packages/<name>/package.yaml` and use the same field names/types as upstream so
  `mason.nvim` can consume them via the `file:` protocol.
