# gws vs. gog for agents

A field report comparing two Google Workspace CLIs for long-running AI agents, including a safe multi-account OAuth setup using Firefox containers.

The published article uses fictional companies and `.example` domains. It contains no real employer names, email addresses, OAuth identifiers, or credentials.

## Local preview

```sh
uv run python -m http.server 8000
```

Then open <http://localhost:8000>.

## Benchmark snapshot

The article reports local Apple Silicon measurements from July 2026:

| Test | gws 0.22.5 | gog 0.34.0 |
|---|---:|---:|
| CLI startup | 3.4 ms | 33.4 ms |
| Gmail `users.getProfile` | 402 ms | 417 ms |
| Peak startup memory | 8.9 MB | 43.3 MB |
| Binary size | 15 MB | 37 MB |

Results are local observations rather than universal performance guarantees.
