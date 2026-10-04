# claude-marketplace

Claude Code plugin marketplace. Each plugin lives in its own repo; this repo only holds `.claude-plugin/marketplace.json`.

| Plugin | Repo |
| :- | :- |
| `footprint` | [aqaurius6666/claude-footprint](https://github.com/aqaurius6666/claude-footprint) |
| `2brain` | [aqaurius6666/2brain](https://github.com/aqaurius6666/2brain) |

## Install

Plugin repos are private: your git must have read access to each one.

```bash
claude plugin marketplace add aqaurius6666/claude-marketplace
claude plugin install footprint@ikarus
```

## Add a plugin

1. Add an entry to `.claude-plugin/marketplace.json`; entry `name` must equal the `name` in the plugin's `plugin.json`.
2. `claude plugin validate .`
3. Install it once for real; `validate` does not check remote `repo`/`path`.
