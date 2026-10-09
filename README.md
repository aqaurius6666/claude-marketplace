# claude-marketplace

Claude Code plugin marketplace. Each plugin lives in its own repo; this repo only holds `.claude-plugin/marketplace.json`.

| Plugin | Repo |
| :- | :- |
| `footprint` | [safeinfra/claude-footprint](https://github.com/safeinfra/claude-footprint) |
| `2brain` | [safeinfra/2brain](https://github.com/safeinfra/2brain) |
| `env-badge` | [safeinfra/claude-env-badge](https://github.com/safeinfra/claude-env-badge) |
| `blast-radius` | [safeinfra/claude-blast-radius](https://github.com/safeinfra/claude-blast-radius) |

Each plugin repo also keeps its own single-plugin marketplace; this repo is the aggregate.

## Install

`footprint` and `2brain` are private repos: your git must have read access to them.

```bash
claude plugin marketplace add safeinfra/claude-marketplace
claude plugin install footprint@safeinfra
```

## Add a plugin

1. Add an entry to `.claude-plugin/marketplace.json`; entry `name` must equal the `name` in the plugin's `plugin.json`.
2. `claude plugin validate .`
3. Install it once for real; `validate` does not check remote `repo`/`path`.
