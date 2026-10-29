## KAERIS

Locale files checked in CI and translated into 46 languages.

KAERIS compares your source locale file with its translations and fails the build when a key is
missing, a key is left over, or a placeholder was lost or renamed. When new strings need
translating, it translates only the keys you added, keeps placeholders and markup intact, and
checks each line by translating it back. It reads and writes 13 formats: JSON, YAML, `.strings`,
`.xcstrings`, `.po`, ARB, Android XML, CSV, XLIFF, `.properties`, `.resx`, Fluent and Markdown.

### Install

```bash
npx kaeris check --source locales/en.json --langs de,fr,ja   # the check only: offline, Node 18+
pip install kaeris                                            # check and translate: Python 3.8+
```

### Repositories

| Repository | What it is | Start with |
|---|---|---|
| [kaeris-cli](https://github.com/kaeris-io/kaeris-cli) | Command-line tool: `check`, `translate`, `fix`, `quota` | `pip install kaeris` |
| [kaeris-action](https://github.com/kaeris-io/kaeris-action) | GitHub Action: a CI gate on locale files, or translations as a pull request | `uses: kaeris-io/kaeris-action@v2` |
| [kaeris-mcp](https://github.com/kaeris-io/kaeris-mcp) | MCP server for Claude, Cursor and other MCP clients | `pip install kaeris-mcp` |

### Plans

The check is free and needs no account. Translation: Free (8 languages per run, no account),
Pro $19/month with 12M characters, Team/API $79/month with 60M characters, Lifetime $79 once
with your own OpenRouter key. Details on [kaeris.dev/pricing](https://kaeris.dev/pricing.html).

### Links

[Website](https://kaeris.dev) ·
[Docs](https://kaeris.dev/docs) ·
[Pricing](https://kaeris.dev/pricing.html) ·
[Status](https://kaeris.dev/status.html) ·
[Security](https://kaeris.dev/security.html) ·
Contact: [support@kaeris.dev](mailto:support@kaeris.dev)
