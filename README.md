# codexport

`codexport` exports Codex session `.jsonl` logs to Markdown.

## Install

No installation is required. The script is directly executable:

```bash
./codexport --help
```

## Usage

Default mode exports only chat messages:

```bash
./codexport /path/to/session.jsonl -o session.md
```

Export all records (`reasoning`, tool calls/outputs, events, turn contexts):

```bash
./codexport --all /path/to/session.jsonl -o session_full.md
```
